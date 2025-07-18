## IDE
* [~~VSCode~~](https://code.visualstudio.com/) replaced by [VSCodium](https://github.com/VSCodium/vscodium/releases/download/1.57.0/VSCodium-win32-x64-1.57.0.zip) - how to debug PHP with [Felix Becker.PHP Debug](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-debug) -- how to [install extension](https://github.com/VSCodium/vscodium/issues/733#issuecomment-863576784)
* [(17mb) SharpDevelop](https://sourceforge.net/projects/sharpdevelop/) - C# with visual designer [ref](https://steemit.com/utopian-io/@dorodor/programming-with-sharpdevelop-creating-a-project-adjusting-properties-and-adding-event-handlers)
* [DevSense.PHP Tools for Visual Studio](https://www.devsense.com/) - dotnetcore required
* [Ironman.PowerShell for Visual Studio / Code](https://ironmansoftware.com/powershell-pro-tools)
* [CodeLobster](http://www.codelobster.com/)  
* [VS Code to web](https://vscode.dev/)  
* [twinBasic](https://twinbasic.com/) - for VB6 and VBA projects. [github](https://github.com/twinbasic/twinbasic)

## server
* [XAMPP](https://sourceforge.net/projects/xampp/)
* [WampServer](https://sourceforge.net/projects/wampserver/)
* by PHP v5.4, you can run a webserver! using the following `php -S localhost:80 -t ../htdocs/`
* [Laragon](https://laragon.org/)  

## database
* [DB Browser for SQLite](https://sqlitebrowser.org/)
* [MySQL-Front](https://www.softpedia.com/get/Internet/Servers/Database-Utils/MySQL-Front.shtml)
* [Ming.Universal SQL Editor](http://www.mingsoftware.com/UniversalSQLEditor/overview.html) - all DB flavors
* [fishlib.Database .NET](https://fishcodelib.com/Database.htm) - all DB flavors
* [devart.dbForge](https://www.devart.com/dbforge/) - all DB flavors
* [HeidiSQL](https://www.heidisql.com/) - all DB flavors
* [SqlDbx](http://www.sqldbx.com/) - all DB flavors
* (SSMS addon) [Redgate.SQL Prompt](https://www.red-gate.com/products/sql-development/sql-prompt/) - Write, format, analyze and refactor your SQL effortlessly
* (SSMS addon) [SSMSBoost](https://www.ssmsboost.com/)
* (SSMS addon) [sqlmash](https://sqlsmash.com/)
* [SoftTree.SQL Assistant](http://www.softtreetech.com/sqlassist/index.htm) - For all DB flavors, also offers addon.
* [Fill Database](http://filldb.info/) - Dummy Data for MYSQL Database  
* [DbGate](https://github.com/dbgate/dbgate) - Database manager for MySQL, PostgreSQL, SQL Server, MongoDB, SQLite and others. Runs under Windows, Linux, Mac or as web application  
* [DbVisualizer](https://www.dbvis.com/)  - (JRE) MySQL, PostgreSQL, SQLite, Oracle, DB2, SQL Server, Sybase, MS Access, Teradata, Firebird, Apache Hive, Phoenix, Presto++  
  * (replica) [DBeaver](https://dbeaver.io/)
* [dblab](https://github.com/danvergara/dblab) - interactive terminal client (go)
* [qstudio](https://github.com/timeseries/qstudio) - SQL Tool (java)
* [MDB Viewer Plus](http://www.alexnolan.net/software/mdb_viewer_plus.htm)
* [ERD](https://erdplus.com/) - online database modeling tool

## git
* [git minimal](https://www.nuget.org/packages/Git-Windows-Minimal/) - Git-Bash, Git-Gui, PERL, Python, and Tcl are excluded. Download rename it to rar, copy the **tools** folder. Add to environment path the **cmd** folder. Behind firewall ? whitelist @ **g**it-http-fetch.exe **g**it-http-push.exe **g**it-remote-https.exe exist @ mingw64\bin.  Use the following :  

```bash
#store credentials as plain text (wincred decrecated) by default to C:\Users\%username%\.git-credentials
git config --global credential.helper store

#disable every time 'enter credentials' form
git config --global credential.interactive never
```  

* [git.MinGit](https://github.com/git-for-windows/git/releases/tag/v2.32.0.windows.1)
* [Fork](https://fork.dev/)
* [sourcegit](https://github.com/sourcegit-scm/sourcegit) [[2](https://github.com/sourcegit-scm/sourcegit-theme)] - same as Fork
* [gitahead](https://github.com/gitahead/gitahead) - same as Fork
* [GitKraken](https://www.gitkraken.com/)
* [Git-Tower](https://www.git-tower.com/windows)
* [Plastic SCM](https://www.plasticscm.com/)
* (chrome addon) [PR-tree-viewer](https://github.com/Pewww/pr-tree-viewer) - View GitHub Pull Requests as a tree
* [Binder](https://mybinder.org/) - Git repo into a collection of interactive notebooks & Docker
	* [Jupyter](https://jupyter.org/) - next-generation notebook interface
* like git - https://githacks.org/vmp2/vmassembler
* like git - https://git.nixnet.services/Narsil/desktop_user.js
* like git - https://git.nolog.cz/mdivecky/headline
* like git - https://gitee.com/vcs-all-in-one/git-repo-go
* [gitstack](https://gitstack.com/) - git server for windows, warning [vulnerability](https://www.exploit-db.com/exploits/43777) &nbsp; ([issue](https://github.com/smart-mobile-software/gitstack/issues/181))  
* [CVS](http://cvs.nongnu.org/) - concurrent versions system  
* [First Pull Request](https://firstpr.me/)  
* [Active GitHub Forks](https://techgaun.github.io/active-forks/)
* [Find latest GitHub fork of a project](https://useful-forks.github.io/)
* [gitignore](https://github.com/github/gitignore) - collection of useful .gitignore templates  
* [GrepAPP](https://grep.app/) - Search across a half million Git repos  

## misc
* [Free for developers](https://free-for.dev/)
* [C# to IL](https://sharplab.io/) - decompiler
* [Compiler Explorer](https://godbolt.org/) - decompiler
* [mathjs](https://api.mathjs.org/)
* [VSCELicense](https://github.com/1Dimitri/VSCELicense) - Visual Studio Community adjust license expiration date (vs2015-2019)
* [java - Recaf](https://github.com/Col-E/Recaf)
* [java - JD GUI](http://java-decompiler.github.io/)  
* [JPEXS Flash Decompiler](https://github.com/jindrapetrik/jpexs-decompiler)
* [Cryptpad](https://cryptpad.fr/) - Real-time collaborative kanban, whiteboard, docs, polls, todos  
* [kan.bn](https://github.com/kanbn/kan) - open source Trello alternative
* [bitrix24](https://www.bitrix24.com/) - collaborate  
* [WinAPI Search](https://dennisbabkin.com/winapisearch/)  
* [PuTTY + PuTTY Key Generator](https://www.puttygen.com/download-putty) - ref [SuperPuTTY](https://www.puttygen.com/superputty) (frontend to provide tabbed PuTTY)
* [NPOI](https://github.com/nissl-lab/npoi) - read/write Office formats without Microsoft Office installed. No COM+, no interop (v2.5.6 is framework)
* [Vanara](https://github.com/dahall/Vanara) - A set of .NET libraries for Windows implementing PInvoke calls to many native Windows APIs
* [ZXing](https://github.com/micjahn/ZXing.Net) - barcode decoder & generator  
* [BarcodeLib](https://github.com/barnhill/barcodelib) - [nuget](https://www.nuget.org/packages/BarcodeLib/)  
* [GtkSharp](https://www.mono-project.com/docs/gui/gtksharp/) - Is a Graphical User Interface Toolkit for mono and .Net. The project binds the gtk+ toolkit and assorted GNOME libraries, enabling fully native graphical Gnome application development using the Mono and .Net development frameworks.  

## web templates
* https://themeforest.net
* https://elements.envato.com/web-templates/
* https://www.templatemonster.com
* https://codecanyon.net/
   * wordpress only
     * https://woocommerce.com/product-category/themes
     * https://templatic.com/
     * https://www.elegantthemes.com/
     * https://themify.me/

## java
* [Javatar](https://www.youtube.com/watch?v=9QFK1cLhytY)
  * [2](https://www.dailymotion.com/video/xowxkz)
* [VSCode - Oracle Java Platform Extension](https://inside.java/2023/10/18/announcing-vscode-extension/)
  * [marketplace](https://marketplace.visualstudio.com/items?itemName=Oracle.oracle-java)
  * [github](https://github.com/oracle/javavscode)

## Visual Studio
```js
//TargetFramework must exists to
//C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework

msbuild test.sln /p:TargetFrameworkVersion=v4.7 /p:DeployOnBuild=true /p:WebPublishMethod=FileSystem /p:DeleteExistingFiles=True /p:SkipInvalidConfigurations=true /p:PrecompileBeforePublish=true /p:ExcludeApp_Data=True /p:EnableUpdateable=True /p:WDPMergeOption="DonotMerge" /p:DebugSymbols=False /p:PublishProvider=FileSystem /p:SkipInvalidConfigurations=true
```

## SQL Server Express
* [2014x86x64](https://www.microsoft.com/en-US/download/details.aspx?id=42299)

```sql
--download only the **LocalDB 64BIT\SqlLocalDB.msi (43mb)**

--install it > then connect using as server
(localdb)\MSSQLLocalDB 

--create a batch file for silent installation :
echo this will install LocalDB2014 silently
pause
msiexec /i SqlLocalDB.msi /qn IACCEPTSQLLOCALDBLICENSETERMS=YES
pause
```  

* [2008R2x64 with SP2](https://www.microsoft.com/en-us/download/details.aspx?id=30438)

```sql
refs
https://docs.microsoft.com/en-us/previous-versions/sql/sql-server-2008/dd981032(v=sql.100)
https://docs.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-from-the-command-prompt?view=sql-server-ver15

unattended with :
sa password - 12
authentication - mixed mode
TCP eanbled

--sqlserver 2008
setup.exe /QS /Action=Install  /IAcceptSQLServerLicenseTerms=1 /SAPWD=12 /SECURITYMODE=SQL /TCPENABLED=1 /Features=SQL /InstanceName=SQLExpress /SQLSYSADMINACCOUNTS="Builtin\Administrators"  

--sqlserver 2012, to disable the check for update add also  
/UpdateEnabled=0  

--sqlserver uninstall  
setup.exe /action=uninstall  

--SSMS w/o Azure references  -- download latest https://aka.ms/ssmsfullsetup  
SSMS-Setup-ENU.exe /Passive DoNotInstallAzureDataStudio=1  

--sql server + SSMS versions  
https://sqlserverbuilds.blogspot.com/2018/01/sql-server-management-studio-ssms.html  

---  

sqlcmd path : 
C:\Program Files\Microsoft SQL Server\100\Tools\Binn

--restore backup file
sqlcmd -E -S .\sqlexpress -Q "RESTORE DATABASE test FROM DISK='c:\demo.bak'"  

--execute sql file - https://docs.microsoft.com/en-us/sql/ssms/scripting/sqlcmd-run-transact-sql-script-files?view=sql-server-ver15  
sqlcmd -E -S .\sqlexpress -i a.sql  
sqlcmd -S.\sqlexpress -i c:\testDB.sql -Ppasswordur -o c:\output.txt -U sa -d testDB  

--

alter SA password 

--https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/change-server-authentication-mode?view=sql-server-ver15

ALTER LOGIN sa ENABLE ;  
GO  
ALTER LOGIN sa WITH PASSWORD = '12' ;  
GO  

```

### create a database
```sql
CREATE DATABASE [test2] ON  PRIMARY 
( NAME = N'test2', FILENAME = N'c:\Program Files\Microsoft SQL Server\MSSQL10_50.SQLEXPRESS\MSSQL\DATA\test2.mdf' , SIZE = 2048KB , FILEGROWTH = 1024KB )
 LOG ON 
( NAME = N'test2_log', FILENAME = N'c:\Program Files\Microsoft SQL Server\MSSQL10_50.SQLEXPRESS\MSSQL\DATA\test2_log.ldf' , SIZE = 1024KB , FILEGROWTH = 10%)
GO
ALTER DATABASE [test2] SET COMPATIBILITY_LEVEL = 100
GO
ALTER DATABASE [test2] SET ANSI_NULL_DEFAULT OFF 
GO
ALTER DATABASE [test2] SET ANSI_NULLS OFF 
GO
ALTER DATABASE [test2] SET ANSI_PADDING OFF 
GO
ALTER DATABASE [test2] SET ANSI_WARNINGS OFF 
GO
ALTER DATABASE [test2] SET ARITHABORT OFF 
GO
ALTER DATABASE [test2] SET AUTO_CLOSE OFF 
GO
ALTER DATABASE [test2] SET AUTO_CREATE_STATISTICS ON 
GO
ALTER DATABASE [test2] SET AUTO_SHRINK OFF 
GO
ALTER DATABASE [test2] SET AUTO_UPDATE_STATISTICS ON 
GO
ALTER DATABASE [test2] SET CURSOR_CLOSE_ON_COMMIT OFF 
GO
ALTER DATABASE [test2] SET CURSOR_DEFAULT  GLOBAL 
GO
ALTER DATABASE [test2] SET CONCAT_NULL_YIELDS_NULL OFF 
GO
ALTER DATABASE [test2] SET NUMERIC_ROUNDABORT OFF 
GO
ALTER DATABASE [test2] SET QUOTED_IDENTIFIER OFF 
GO
ALTER DATABASE [test2] SET RECURSIVE_TRIGGERS OFF 
GO
ALTER DATABASE [test2] SET  DISABLE_BROKER 
GO
ALTER DATABASE [test2] SET AUTO_UPDATE_STATISTICS_ASYNC OFF 
GO
ALTER DATABASE [test2] SET DATE_CORRELATION_OPTIMIZATION OFF 
GO
ALTER DATABASE [test2] SET PARAMETERIZATION SIMPLE 
GO
ALTER DATABASE [test2] SET  READ_WRITE 
GO
ALTER DATABASE [test2] SET RECOVERY SIMPLE 
GO
ALTER DATABASE [test2] SET  MULTI_USER 
GO
ALTER DATABASE [test2] SET PAGE_VERIFY CHECKSUM  
GO
USE [test2]
GO
IF NOT EXISTS (SELECT name FROM sys.filegroups WHERE is_default=1 AND name = N'PRIMARY') ALTER DATABASE [test2] MODIFY FILEGROUP [PRIMARY] DEFAULT
GO
```  

### create a user  

```sql
USE [master]
GO
CREATE LOGIN [papa] WITH PASSWORD=N'papa', DEFAULT_DATABASE=[master], CHECK_EXPIRATION=OFF, CHECK_POLICY=ON
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'bulkadmin'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'dbcreator'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'diskadmin'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'processadmin'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'securityadmin'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'serveradmin'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'setupadmin'
GO
EXEC master..sp_addsrvrolemember @loginame = N'papa', @rolename = N'sysadmin'
GO
USE [test]
GO
CREATE USER [papa] FOR LOGIN [papa]
GO
USE [test]
GO
EXEC sp_addrolemember N'db_accessadmin', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_backupoperator', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_datareader', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_datawriter', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_ddladmin', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_denydatareader', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_denydatawriter', N'papa'
GO
USE [test]
GO
EXEC sp_addrolemember N'db_securityadmin', N'papa'
GO
```  

### change authentication through registry

restart of services required 

```sql
Windows Registry Editor Version 5.00

# src - https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/change-server-authentication-mode?view=sql-server-ver15
#2 = mixed login
#1 = win auth only
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Microsoft SQL Server\MSSQL10_50.SQLEXPRESS\MSSQLServer]
"LoginMode"=dword:00000002
```


### restart services  

```
@echo off

REM src - https://www.mssqltips.com/sqlservertip/6307/how-to-stop-and-start-sql-server-services/

echo "Stopping services"

net stop MSSQL$SQLEXPRESS
net stop SQLBrowser

pause

echo "Starting services"

net start MSSQL$SQLEXPRESS
net start SQLBrowser

pause
```  

## MySQL  


### backup dbase via cmd  

```sql
--backup tables schema
mysqldump --no-data -u root -ppassword dbasename > dbaseSchema.sql

--backup tables schema and view & procs
mysqldump.exe --routines --no-data -u root -ppassword dbasename > dbaseSchema_W_routines.sql

--backup schema & data for specific tables
mysqldump.exe -u root -ppassword dbasename tablename1 tablename2 tablename3 tablename4 > dbaseDefaultTables.sql
```  

### restore dbase via cmd  

```sql
mysql -u root -ppassword dbasename < c:\localhost.sql
-- OR
mysql -u root -ppassword < c:\localhost.sql 
```  

### dbases size  

```sql
SELECT table_schema "DB Name",
        ROUND(SUM(data_length + index_length) / 1024 / 1024, 1) "DB Size in MB" 
FROM information_schema.tables 
GROUP BY table_schema; 
```  

### table size  

```sql
SELECT
  TABLE_NAME AS `Table`,
  ROUND((DATA_LENGTH + INDEX_LENGTH) / 1024 / 1024) AS `Size (MB)`
FROM
  information_schema.TABLES
WHERE
  TABLE_SCHEMA = "dbase_name"
ORDER BY
  (DATA_LENGTH + INDEX_LENGTH)
DESC;
```  

### table rows  

```sql
SELECT    TABLE_NAME,    TABLE_ROWS
FROM
    `information_schema`.`tables`
WHERE
    `table_schema` = 'dbase_name';
```  

### add foreign key  

```sql
ALTER TABLE `leagueseasons` 
ADD CONSTRAINT `leagueID` FOREIGN KEY (`league_id`) 
REFERENCES `leagues`(`id`);
```  

### add UNIQUE with multiple fields  

```sql
ALTER TABLE `standings` ADD UNIQUE `unique_index`(`league_id`, `season`, `rank`);
```  

### last queries ran 

```sql
--https://stackoverflow.com/a/678310
SET GLOBAL log_output = 'TABLE';
SET GLOBAL general_log = 'ON';
SELECT * FROM  mysql.general_log  order by 1 desc
```  

### disable keys validation  

```sql
SET FOREIGN_KEY_CHECKS = 0;

--your SQL here

SET FOREIGN_KEY_CHECKS = 1;
```  

### reset auto_increment seed 

```sql
ALTER TABLE table_name AUTO_INCREMENT = 1

--TRUNCATE also reset it
TRUNCATE TABLE table_name;
```

### configure mysql with my.ini - compatibility mode + server timezone to UTC

```sql
[mysqld]
port=3306
sql-mode="NO_ZERO_IN_DATE,NO_ZERO_DATE,NO_ENGINE_SUBSTITUTION"
default-time-zone='+00:00'

--then you can see the changes
SELECT @@SQL_MODE, @@GLOBAL.SQL_MODE;
SELECT @@time_zone, @@GLOBAL.time_zone;
```