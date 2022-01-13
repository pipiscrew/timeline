## why?
Most of us, maintaining a blog for years, currently mine has 15k articles. Needed a free solution to archive it and continue on new things. Heroku free plan, **restore** the branch every X time, the possibilities are two, use Postgre or sqlite. When sqlite, the deploy (last push) should be fine, meaning no other configuration should be made on server side, as it will be lost after X time. On the other side Postgre limitation is the 10k rows (count of all rows on all tables). In this article explaining how to sqlite on heroku. 

## bring the online data, locally

* **Backup** the dbase (phpmyadmin), choose compression.
* Go to webspace control panel > Filemanager > **Compress whole Wordpress** folder.

now we have a **dbase.zip** & **wp.zip** locally.

**Restore** the dbase to your local **phpmyadmin**.

## download & setup of nginx

Download [nginx](https://nginx.org/en/download.html) (currently stable-v1.18), extract it to `C:\nginx\ `  

find ready to use [nginx.conf](https://raw.githubusercontent.com/pipiscrew/timeline/main/assets/nginx.conf.txt) for php.  

## download & setup of php

Download [PHP Non Thread Safe x86](https://windows.php.net/download/#php-8.0-nts-vs16-x86), extract it at `C:\nginx\php`.  

* add **php folder** to system/user **environment path**. (Control panel > System > Advanced system settings > Advanced > Environment variables.  

* rename the **php.ini-development** & **edit** the **php.ini**, uncomment  
	* extension_dir = "ext"  
* enable the following extensions :
	* extension=curl
	* extension=mbstring
	* extension=mysqli
	* extension=pdo_mysql
	* extension=pdo_pgsql
	* extension=pdo_sqlite
	* extension=openssl  

## composer
Once you are on PHP dir (C:\nginx\php), you have to download the latest composer, follow the CMDs by [homepage](https://getcomposer.org/download/).  
  
    php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
    // this will download the composer-setup.php to php dir. Execute it :
    
    execute the setup, to download the composer.phar
    php composer-setup.php

Delete the **composer-setup.php**, no needed anymore. In **php dir**, create a batch file called **composer.bat**, this will be our **shortcut** for **composer commands** :  

    @php C:\nginx\php\composer.phar %*


Go to **C:\nginx\html**, create a **composer.json** file, like (to enable **PDO SQLITE** extension), this will take place on **HEROKU** side.  

    {
	    "require": {
	    	  "ext-pdo_sqlite": "*"
	    	}
    }

(**C:\nginx\html**) save & run from cmd  

    composer update

> Tip :: Now it will run the composer.bat (aka shortcut) we created on previous step  

## First try to browse locally wp
Delete the default html files & copy the wordpress files to **C:\nginx\html**, browse at localhost, if you get  
> Fatal error: __autoload() is no longer supported, use spl_autoload_register() instead in C:\nginx\html\wp-includes...  

You are on **old wordpress** version, **php v8** doesn’t support it, has some deprecated functions, download [wordpress](https://wordpress.org/download/releases/) (currently stable-v5.7)!!  (download the distro zip and extract it there (**C:\nginx\html**) excluding **wp-config.php**.  

## Configure VA points
We have to establish database connection, edit `c:\nginx\html\wp-config.php` alter :  

```javascript
    /** MySQL database username */
    define('DB_USER', 'root');
    
    /** MySQL database password */
    define('DB_PASSWORD', 'password');
    define( 'DB_CHARSET', 'utf8mb4' );
    
    define( 'WP_POST_REVISIONS', 0 ); //disable store revisions for posts at dbase.
```  

Next on the top of the same file (c:\nginx\html\**wp-config.php**), set strictly **SSL** (otherwise in the end will get multiple protocols error)  

```javascript
    define('FORCE_SSL_ADMIN', true);
    define('FORCE_SSL_LOGIN', true);
    if (isset($_SERVER['HTTP_X_FORWARDED_PROTO']) && $_SERVER['HTTP_X_FORWARDED_PROTO'] == 'https'){ $_SERVER['HTTPS']='on'; }
```  

If finally, you used a new version of wordpress and not the one you download from your server, you have to make sure that the following hashes are the same on **wp-config.php** fix the following properties :  
  
```javascript
    define('AUTH_KEY',
    define('SECURE_AUTH_KEY', 
    define('LOGGED_IN_KEY',   
    define('NONCE_KEY',   
    define('AUTH_SALT',   
    define('SECURE_AUTH_SALT',
    define('LOGGED_IN_SALT',  
    define('NONCE_SALT',  
```  
    

and also make sure the tables prefix  

    $table_prefix = 'w_';

* Browse localhost! Wordpress is alive! With your **local MYSQL**


## SQLite addon

Download it [here](https://github.com/aaemnnosttv/wp-sqlite-integration).

1. Download the plugin & extract it.
1. Move **sqlite-integration** (rename it) folder to **wordpress/wp-content/plugins** folder.
1. Copy **db.php**, exists in **sqlite-integration** folder to **wordpress/wp-content** folder.

The addon is **outdated** fixes needed,  tested versus **php v8.0.3**  

```javascript
    C:\nginx\html\wp-content\plugins\sqlite-integration\pdoengine.class.php : 788 + 791
    		if (in_array($param[strlen($param)-1], array("'",'"'))) {
    		if (in_array($param[0], array("'",'"'))) {
    // https://stackoverflow.com/a/59158549
    
    C:\nginx\html\wp-content\plugins\sqlite-integration\pdoengine.class.php : 340 (replace function declaration  came with PHP v8)
    public function query(string $query, ?int $fetchMode = null, ...$fetchModeArgs) {
    // https://stackoverflow.com/a/64727356  
```  

## Define sqlite dbase filename 
**Not  required step**, go back to **wp-config.php** and
 
    define('DB_FILE', 'dbase.db3');

if no set, the default will be **.ht.sqlite** inside `C:\nginx\html\wp-content\database`.

Browse localhost! Wordpress is alive with **SQLITE**!!

You getting wordpress installation screen! **You must proceed** with the installation till end (aka create the admin user).

## Migrate MySQL2SQLITE
Use any **client application** to browse the SQLITE dbase ([such](https://sqlitebrowser.org/)).

The following tables **should not transfered** from MYSQL, as containing information by current installation!!  

* wp_usermeta
* wp_users


Use any application ([such](https://www.dbsofts.com/)), to **transfer** wordpress MySQL to SQLITE just **created**!!  

>TIP : on sqlite dbase, delete any records exist, to the tables you gonna transfer from MySQL.

All Wordpress, **baseURL** read by **wp_options** table fields :  

* siterul  
* home  
 
, (please adjust it to **heroku URL** or **localhost** (if u like to configure it, before upload it))

>TIP : Any time you **go to push** to heroku, you have to change it! Or **better** use/**define** the variables described below in **wp-config.php**

Alternatively, **without change** the dbase, for **testing purposes** as  

```javascript
    define( 'WP_SITEURL', 'http://localhost' );
    define( 'WP_HOME','http://localhost' );
```  

at the beginning of **wp-config.php**.


> TIP : if not changing the URLS, you **cant** access WP_ADMIN!! (is all about https & http)

The sets are: 

* when localhost  
```javascript
    /*
    define('FORCE_SSL_ADMIN', true);
    define('FORCE_SSL_LOGIN', true);*/
    
    define( 'WP_SITEURL', 'http://localhost' );
    define( 'WP_HOME','http://localhost' );  
```  

* when going to heroku  
```javascript
    define('FORCE_SSL_ADMIN', true);
    define('FORCE_SSL_LOGIN', true);
    /*
    define( 'WP_SITEURL', 'http://localhost' );
    define( 'WP_HOME','http://localhost' );
    */
```  

## Normalize URLS at dbase 
Before push dbase to heroku, mostly needed to fix links point to **C:\nginx\html\wp-content\uploads**. Normalize means to change at **sqlite dbase** the **links** from production to **heroku** via :  

```javascript
    a)
    update w_posts set 
      post_content = replace(post_content, 'www.pipiscrew.com', 'test.heroku.com')
    where
      post_content like '%www.pipiscrew.com%';
    
    
    update w_posts set 
      guid = replace(guid, 'www.pipiscrew.com', 'test.heroku.com')
    where
      guid like '%www.pipiscrew.com%'; 

    b)
    update w_posts set 
      post_content = replace(post_content, 'pipiscrew.com', 'test.heroku.com')
    where
      post_content like '%pipiscrew.com%';
    
    update w_posts set 
      guid = replace(guid, 'pipiscrew.com', 'test.heroku.com')
    where
      guid like '%pipiscrew.com%';    
    
 
```  


and of course, dont forget to read the heroku official [howto](https://help.heroku.com/58GWW5CQ/can-i-use-wordpress-on-heroku) `#haha`