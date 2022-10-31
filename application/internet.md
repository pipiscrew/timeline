## Browser

### Blink  

* [Brave](https://brave.com/) -- [the false sensation of privacy](http://ebin.city/~werwolf/posts/brave-is-shit/) -- [features they disable or remove](https://github.com/brave/brave-browser/wiki/Deviations-from-Chromium-(features-we-disable-or-remove)/)
  * [individual components update (adblock explained)](https://www.pipiscrew.com/2021/06/brave-individual-components-update-adblock-explained/)
* [SRWare](https://www.srware.net/iron/) - removed all telemetry
* [Beacon](https://github.com/imperviousinc/beacon) - decentralized
* [ungoogled](https://github.com/Eloston/ungoogled-chromium) -- sans integration with Google
  * [bin mirror](https://chromium.woolyss.com/#windows-64-bit) ([ref](https://github.com/Eloston/ungoogled-chromium/issues/1519#issuecomment-852119889))
* [Marmaduke](https://github.com/mtslzr/homebrew-marmaduke-chromium) -- homebrew tap
* [Hibbiki](https://github.com/Hibbiki/chromium-win64) -- homebrew tap
* [Google Chrome Offline](https://google.com/intl/en/chrome/?standalone=1) -- warning fingertips

Automatically open Chrome DevTools debug - `"c:\chrome.exe" -auto-open-devtools-for-tabs`.  

To find the profile currently is use navigate to `chrome://version`.  

To start with specific profile, `chrome.exe --user-data-dir=c:\foo`  

* [CRXcavator](https://crxcavator.io/) 
* [CRXextractor](https://crxextractor.com/)  

### Gecko 

* [Mozilla.Firefox](https://www.mozilla.org/en-US/firefox/all/#product-desktop-release) 
  * [Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)
* Unofficial windows, [IceCat](https://github.com/muslayev/icecat-win64) for ultra privacy. The official Linux [here](https://www.gnu.org/software/gnuzilla/).
* [LibreWolf](https://librewolf.net/) - focused on privacy, security and freedom.
* [waterfox](https://www.waterfox.net/) - [waterfox web browser sold to System1](https://www.waterfox.net/blog/waterfox-has-joined-system1/)
* [Dot Browser](https://www.dothq.co/) – privacy-conscious web browser
* [Basilisk](https://basilisk-browser.org/features.shtml) - Replaced Gecko with Goanna (single-process mode) engine, interface as-carried by Firefox between v29 and v56, more read at features page.  

To find the profile currently is use navigate to `about:support` or `about:profiles`.  
 * [profile manager](https://support.mozilla.org/en-US/kb/profile-manager-create-remove-switch-firefox-profiles) - to start with specific profile, `firefox.exe -P "<profile name>" `  

To load temporary addon or to see what is loaded goto `about:debugging` ([ref](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension))  

----------


both **IceCat** & **Brave** & **Firefox w/ arkenfox** when restarted getting new fingerprint.  

Tested with :

  * [FingerprintJS](https://fingerprintjs.com/demo)
    * [cross-browser tracking](https://fingerprintjs.com/blog/external-protocol-flooding/)
    * [bot detection](https://github.com/fingerprintjs/BotD)
  * [Unique Machine](http://uniquemachine.org/) 
  * [TLS Fingerprint](https://tlsfingerprint.io/) - appears on first page
  * [No-JS fingerprinting](https://noscriptfingerprint.com/)  
  --
  * [WebRTC Local IP Leak Test](https://niespodd.github.io/webrtc-local-ip-leak/) - Chromium based browsers leak user local IP via WebRTC foundation attribute  

test browser [permissions](https://permission.site/).

[See what JavaScript commands get injected through an in-app browser](https://krausefx.com/blog/announcing-inappbrowsercom-see-what-javascript-commands-get-executed-in-an-in-app-browser) [[2](https://inappbrowser.com/)]


----------

**Mozilla.Firefox** v86 Introduces [Total Cookie Protection](https://blog.mozilla.org/security/2021/02/23/total-cookie-protection/) (you have to enable **strict mode** on privacy setings)  
**Mozilla.Firefox** v87 Introduces [SmartBlock](https://blog.mozilla.org/security/2021/03/23/introducing-smartblock/) (NoScript and uBlock Origin teams helping this approach)  
**Mozilla.Firefox** v88 isolates [window.name](https://www.mozilla.org/en-US/firefox/88.0/releasenotes/) data  
[Site Isolation](https://blog.mozilla.org/security/2021/05/18/introducing-site-isolation-in-firefox/) in **Firefox** - `about:config > fission.autostart > true`  
[Mozilla integrates Firefox offline Translations into Firefox](https://www.ghacks.net/2021/05/29/mozilla-integrates-firefox-translations-into-firefox/) - `about:config > extensions.translations.disabled > turn to false > restart`  
**Mozilla.Firefox** v89 - redesigned and modernized, [private browsing](https://blog.mozilla.org/security/2021/06/01/total-cookie-protection-in-private-browsing/) changed & explained  
[Mozilla.Firefox v89 Tab Appearance](https://amitp.blogspot.com/2021/06/firefox-89-tab-appearance.html)
* [2](https://color.firefox.com)
* [3](https://firefoxcss-store.github.io/)
* [4](https://github.com/black7375/Firefox-UI-Fix)
* If you don't like the new look of Firefox 89, then set `browser.proton.enabled` to `false` in `about:config`    

[Mozilla.Firefox DNS-over-HTTPS rollout](https://blog.mozilla.org/en/mozilla/news/firefox-by-default-dns-over-https-rollout-in-canada/) -  in Canada (with local DoH provider CIRA)

**Mozilla.Firefox** [v90](https://www.mozilla.org/en-US/firefox/90.0/releasenotes/) - supports [Fetch Metadata Request Headers](https://blog.mozilla.org/security/2021/07/12/firefox-90-supports-fetch-metadata-request-headers/)  
  * `about:third-party` - identify compatibility issues caused by third-party applications  
  * introduces [background updates](https://support.mozilla.org/en-US/kb/enable-background-updates-firefox-windows) :(, disable it via  `about:config` > `app.update.background.scheduling.enabled`

[Mozilla: *Privacy Not Included](https://foundation.mozilla.org/en/privacynotincluded/)  

**Mozilla.Firefox** v91 - [enables](https://www.mozilla.org/en-US/firefox/91.0/releasenotes/) cookie jar per site, makes easier to delete all cookie for a site.

[Improve memory usage](https://www.reddit.com/r/firefox/comments/p8g5zd/why_does_disabling_accessibility_services_improve/) - by set the `accessibility.force_disabled` to **1** at `about:config`  

[Mozilla - uBlock Origin review](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/)  

**Mozilla.Firefox** [v93](https://www.mozilla.org/en-US/firefox/93.0/releasenotes/) &nbsp; ([Shadow DOM](https://hacks.mozilla.org/2021/10/lots-to-see-in-firefox-93/))

&nbsp;

#### Using Firefox **user.js** settings file

* settings made in `about:config` are saved only to `prefs.js` [ref](https://mkaz.blog/misc/using-firefox-user-js-settings-file/)
* `user.js` file stores user settings, the file is loaded each time Firefox starts. This a convenient way to save your browser customizations and apply them on different machines. Ready to use `user.js` copy it near `prefs.js` :  
  * [arkenfox](https://github.com/arkenfox/user.js)  ([ref](http://ebin.city/~werwolf/posts/firefox-hardening-guide/)) - tested with v87, generates new fingerprint on restart++.  
    * [12bytes.org - user-overrides.js](https://codeberg.org/12bytes.org/Firefox-user.js-supplement) suppliment for the 'arkenfox'. Is an optional supplement intended to be appended to the arkenfox `user.js`. Use the 'arkenfox' `updater.bat` to append the `user-overrides.js` file to the `user.js` file.
    * [powerman/user-overrides.js](https://gist.github.com/powerman/b90f3a63fa2f3583d3e89b2468f95388) - alternative user-overrides.js.
  * [pyllyukko](https://github.com/pyllyukko/user.js/)
  * [narsil](https://git.nixnet.services/Narsil/desktop_user.js)

#### Addons

  * [uBlock Origin](https://github.com/gorhill/uBlock) - efficient blocker for Firefox and Chromium
  * [NoScript](https://noscript.net/) - extra protection for Firefox  
  * [JShelter](https://jshelter.org/) - mitigate potential threats, fingerprinting, tracking, and data collection
  * [Anti-Adblock Killer](https://github.com/reek/anti-adblock-killer)
  * [EMNISoft](https://help.emsisoft.com/en/1974/emsisoft-browser-security/) - from the company writes decryption application for ransomwares
  * [Super Custom Blocker](https://supercustomblocker.com)
  * [Mullvad Privacy Companion](https://mullvad.net/en/blog/2022/3/22/mullvad-privacy-companion-now-open-source/)
  * [Privacy Badger](https://privacybadger.org/) - learns to block invisible trackers
  * [Vytal](https://github.com/z0ccc/Vytal) -  spoofs your location data [tester](https://vytal.io/)
  * [AdGuard AdBlocker MV3 Experimental](https://chrome.google.com/webstore/detail/adguard-adblocker-mv3-exp/apjcbfpjihpedihablmalmbbhjpklbdf)
  * [Ghostery](https://www.ghostery.com/) - Block Ads, Stop Trackers, and Speed Up Websites [firefox](https://addons.mozilla.org/en-US/firefox/addon/ghostery/) / [chrome](https://chrome.google.com/webstore/detail/ghostery-%E2%80%93-privacy-ad-blo/mlomiejdfkolichcflejclcbmpeaniij)
  * [magnolia.Bypass Paywalls Clean](https://gitlab.com/magnolia1234/bypass-paywalls-chrome-clean/-/issues/45) - Allows you to read articles from websites that implement a paywall. [chrome](https://gitlab.com/magnolia1234/bypass-paywalls-chrome-clean) / [firefox](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean)
    * [how to](https://www.youtube.com/channel/UCeDuSy0mmE-3bEDJVINA3-g/videos)
      * [Disable Cookies](https://chrome.google.com/webstore/detail/disable-cookies/lkmjmficaoifggpfapbffkggecbleang)
      * [I don't care about cookies](https://chrome.google.com/webstore/detail/i-dont-care-about-cookies/fihnjjcciajhdojfnbdddfaoknhalnja)
  * [Cookie AutoDelete](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete) [firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-autodelete/) / [chrome](https://chrome.google.com/webstore/detail/cookie-autodelete/fhcgjolkccmbidfldomjliifgaodjagh)
  * Chrome-like [translate](https://github.com/FilipePS/Traduzir-paginas-web/) functionality (aka on the fly) to Firefox - Filipe Ps.Translate Web Pages
  * Browsec [VPN](https://addons.mozilla.org/en-US/firefox/addon/browsec/) free & fast.
  * [Mullvad VPN](https://mullvad.net/) - seems the father of VPN, paid firefox service using this. [available on Amazon](https://mullvad.net/en/blog/2022/7/26/mullvad-is-now-available-on-amazon-us-se/)
  * [Remove Google Redirection on google results](https://addons.mozilla.org/en-US/firefox/addon/remove-google-redirections/)
  * [RESTClient](https://addons.mozilla.org/en-US/firefox/addon/restclient/) - use request header as `Content-Type application/x-www-form-urlencoded`
  * [SingleFile](https://addons.mozilla.org/en-US/firefox/addon/single-file/) - Save an entire web page (including images and styling) as a single HTML file.
    * [github](https://github.com/gildas-lormeau/SingleFile) - has also chrome
  * [Highlight This](https://highlightthis.net/) - highlights words from your predefined list. [firefox](https://addons.mozilla.org/en-US/firefox/addon/highlightthis) / [chrome](https://chrome.google.com/webstore/detail/highlight-this/fgmbnmjmbjenlhbefngfibmjkpbcljaj?hl=en-US)
  * [Buster: Captcha Solver for Humans](https://github.com/dessant/buster)  
  * [Copy ShortURL](https://addons.mozilla.org/en-US/firefox/addon/copy-shorturl/)
  * [Copy True Link for Google](https://github.com/dandanua/copy-true-link) ([ref](https://gist.github.com/radiantly/e1c7319214c77fa007f323fc56cd0239))
  * [DownAlbum](https://chrome.google.com/webstore/detail/downalbum/cgjnhhjpfcdhbhlcmmjppicjmgfkppok) - Download Facebook, Instagram, Pinterest, Twitter, Ask.fm, Weibo album  
  * [Hypersearch](https://github.com/abhinavsharma/hypersearch) - browser extension for improving search  
  * [BrainTool - Organizing Bookmarks](https://braintool.org/)  
  * [LibRedirect](https://github.com/libredirect/libredirect) Redirect YouTube, Twitter, Instagram to privacy friendly services  

----------

Chrome.[Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey-beta/gcalenpjmijncebpfijmoaglllgpjagf) / Firefox.[Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) -- [Youtube - dismiss sign-in script](https://greasyfork.org/de/scripts/412178-youtube-dismiss-sign-in)

[Mozilla.Monitor](https://monitor.firefox.com/) - See if you’ve been part of an online data breach. #pwned  
[Mozilla.Rally](https://rally.mozilla.org/) - Donate your data to studies.  
[SponsorBlock](https://sponsor.ajay.app/) - Blocking Unwanted YouTube Video Segments.

### Mozilla.Firefox - Cache Memory reduction  
`about:cache` - see the cache settings  
`about:performance` - browser process manager  
`about:config` > `browser.cache.memory.capacity` - user can modify to an actual value instead of -1 (unlimited) it's in kilobytes. Or disable [browser.cache.memory.enable](http://kb.mozillazine.org/Browser.cache.memory.enable) entirely.  
To disable multiple running processes of the browser, you can set `browser.tabs.remote.autostart` to `false`. But be aware, now when a tab crashes it will kill your whole browser, but it will use less RAM.   


## Minimal Browser
* [NetSurf](https://www.netsurf-browser.org/)
* [Nessie](https://www.radsix.com/)
* [Otter Browser - Controlled by the user, not vice versa](https://github.com/OtterBrowser/otter-browser)
    * [2](https://otter-browser.org/)  

## Password Manager

* KeePassXC

	I dont like the online systems, never use it.
	
	In case you still use the Roboform desktop edition export the existing logins by using the [following](https://www.pipiscrew.com/2015/08/app-roboform-to-keepass/) method.
	
	Use [Keepass v2.x](https://keepass.info/download.html) to import it. Then use the dbase with [KeePassXC](https://keepassxc.org/).
	
	**KeePassXC vs KeePass**
	
	Is a community-developed open-source fork of KeePass, one of the best password managers for Windows. KeePassXC differs from KeePass because it works on Linux, Mac, and Windows, but it also lacks some of the original software's features, such as plug-in support. [src](https://www.techradar.com/reviews/keepassxc)
	
	Then install the **KeePassXC-Browser addon** for [firefox](https://addons.mozilla.org/en-US/firefox/addon/keepassxc-browser/) or [chrome](https://chrome.google.com/webstore/detail/keepassxc-browser/oboonakemofpalcgghocfoadofidjkkk). 
	
	--
	
	The browser addons on [github](https://github.com/keepassxreboot/keepassxc-browser).
	
	WARNING the browser addon from github repository, has different signature by the one is on the marketplace… Possible when use the one by repository you have to download also the [KeePassXC](https://github.com/keepassxreboot/keepassxc) from the repository(?).. otherwise user getting something like “cant connect” error.
	
	--
	
	Connecting the application and extension, any adjustment made to tools > settings > browser integration, it saves the configuration under
	
	C:\Users\\%username%\AppData\Local\KeePassXC	
	
	official guide on [how to](https://keepassxc.org/docs/KeePassXC_GettingStarted.html#_setup_browser_integration)

  --

  Carrying the passwords to android with [KeePassDroid](https://play.google.com/store/apps/details?id=com.android.keepass), just copy your *.kdbx to android and open it.  

  

* [bitwarden](https://bitwarden.com/) - the free online solution 
* [RoboForm](https://www.roboform.com/) - the well known
* [Mozilla.Firefox Lockwise](https://www.mozilla.org/en-US/firefox/lockwise/)  

## FTP
* [FileZilla](https://filezilla-project.org/)
* [WinSCP](https://winscp.net/eng/index.php)

## Download Manager
* [eric.HTTP Downloader](https://erickutcher.github.io/#HTTP_Downloader)
* [FlashGet](http://www.oldversion.com/windows/flashget-1-73)
* [Free Download Manager](https://www.freedownloadmanager.org/)
* [WellGet](https://www.softpedia.com/get/Internet/Download-Managers/WellGet.shtml)
* [VisualWget](https://sites.google.com/site/visualwget/a-download-manager-gui-based-on-wget-for-windows)
* [AM Downloader](https://mozib.io/amdownloader) / [2](https://github.com/antikmozib/am-downloader)

## Offline Browser
* [httrack](https://www.httrack.com/)
* [Teleport](http://www.tenmax.com)
* [MetaProducts.Offline Explorer](https://metaproducts.com/products/offline-explorer)
* [Visual Web Ripper](http://visualwebripper.com/)

## Analyzers
* [Charles](https://www.charlesproxy.com/) - Is an HTTP proxy / HTTP monitor / Reverse Proxy that enables a developer to view all of the HTTP and SSL / HTTPS traffic
* [Telerik.Fiddler](https://www.telerik.com/fiddler) - Web Debugging Proxy Tool
* [HTTP Debugger](https://www.httpdebugger.com/)

## Firewall
* [TinyWall](https://tinywall.pados.hu/)
* [Evorim.Firewall](https://www.evorim.com/en/free-firewall)
* [simplewall](https://www.henrypp.org/product/simplewall)
* [GlassWire](https://www.glasswire.com/)
* [Look 'n' Stop](http://www.looknstop.com) (till win7)

## Limiters
* [NetLimiter](http://www.netlimiter.com)
* [seriousbit.netbalancer](http://seriousbit.com/netbalancer/)

## Network
* [HostsMan](http://www.abelhadigital.com/hostsman/) - Manage your hosts file with ease
* [MyLanViewer](http://www.mylanviewer.com/network-ip-scanner.html) - IP address scanner 
* [RdpGuard](https://rdpguard.com/) - Protect Windows RDP, MySQL, MS-SQL etc.
* [NetSetMan](https://www.netsetman.com/) - Network profiles switch
* [FabulaTech.USB over Network](http://www.usb-over-network.com/usb-over-network.html)
* [UltraVNC](https://www.uvnc.com/) - Remote PC network access
* [AnyDesk](https://anydesk.com/en) - Remote Desktop anywhere, anytime
* [TeamViewer](https://www.teamviewer.com/) - Control, manage, monitor, and repair computers
* [Rustdesk](https://rustdesk.com/) - TeamViewer alternative
* [mRemoteNG](https://mremoteng.org/) - RDP connections manager (make always off, on each connection the `Cache Bitmap`)
* (discontinued) [Microsoft.Remote Desktop Connection Manager](https://filehippo.com/download_remote_desktop_connection_manager/) - RDP connections manager
* [GetScreen](https://getscreen.me/)  

## KVM  
* [Microsoft.Garage Mouse without Borders](https://www.microsoft.com/en-us/download/details.aspx?id=35460) - Control computers from a single mouse and keyboard  
* [ShareMouse](https://www.sharemouse.com/) - Control multiple computers from a single mouse and keyboard  
* [Barrier](https://github.com/debauchee/barrier) - forked from Synergy v1.9 codebase. Synergy was a commercialized reimplementation of the original CosmoSynergy written by Chris Schoeneman.
* [Synergy](https://symless.com/synergy) - Share your mouse and keyboard via network  

## Image Upload
* [MyImgur](http://myimgur.eden.fm/)
* [EasyImgur](https://bryankeiren.com/easyimgur/)

## Mail
* [Mozilla.Thunderbird](https://www.thunderbird.net/)
  * [Proton Mail Bridge Thunderbird setup guide](https://proton.me/support/protonmail-bridge-clients-windows-thunderbird)
* [Betterbird](https://www.betterbird.eu/) - is a fine-tuned version of Mozilla Thunderbird
* [Just Report It](https://justreport.it/) - Thunderbird & Outlook addon, report to spamcop & domain registrar
* [Claws Mail](https://www.claws-mail.org/) - is an email client (and news reader) based on GTK+
* [Desksoft.CheckMail](http://www.desksoft.com/CheckMail.htm)
* [POP Peeper: Email Notifier](https://www.esumsoft.com/products/pop-peeper/) - email notifier that runs in your Windows taskbar
* [MailStore Home](https://www.mailstore.com/en/products/mailstore-home/) - Central archive for all emails. Reads mbox / pst / thunderbird (unicode, in search use * for wildcard, because searching by words). 

## Mail mbox
* [BitRecover.mbox viewer](https://www.bitrecover.com/free/mbox-viewer/) - direct browse mbox (no so good on search, tip use F3 after the first search)
* [BitRecover.mbox Converter Wizard](https://www.bitrecover.com/mbox-converter/) - convert gmail mbox to pst, with attachments
* [Thunderbird addon - ImportExportTools NG](https://addons.thunderbird.net/en-US/thunderbird/addon/importexporttools-ng/) - convert gmail mbox to thunderbird. The original [addon](https://addons.thunderbird.net/en-US/thunderbird/addon/importexporttools/) supports 14.x - 16.x
* [PST Walker](https://www.pstwalker.com/pstwalker.html) - light & portable by company, use it in combination with the mbox2pst (super search + unicode + attachments)

## Mail spam 
* [spamcop](https://www.spamcop.net/) - forward the junk mails to fight spam. Once registered you will get a unique mail address to send the junk mails for investigation. If you like to use multiple mails, please see the **Mailhosts** option, you need to registered all mails there.
  * [How do I get my email program to reveal the full, unmodified email](https://www.spamcop.net/fom-serve/cache/19.html) ?  

## Mail proxy
* [duckduckgo email protection](https://duckduckgo.com/email/) - requires browser addon
* [Forward Email](https://forwardemail.net/en)
* [simplelogin](https://simplelogin.io/) - proxy by proton  

## RSS
* [QuiteRSS](https://quiterss.org/)
* [RSS Guard](https://github.com/martinrotter/rssguard)
* [Inoreader](https://www.inoreader.com/) - online
* [battware.Desktop Ticker](http://www.battware.co.uk/desktopticker.htm)  

## wifi
* [Nirsoft.WifiInfoView](https://www.nirsoft.net/utils/wifi_information_view.html) - Scans the wireless networks in your area and displays extensive information
* [Passmark.WirelessMon](https://www.passmark.com/products/wirelessmonitor/) - Monitor wireless adapters and WiFi access points
* [faproc.Wifi Analyzer](https://play.google.com/store/apps/details?id=com.farproc.wifi.analyzer) - Turns your android phone into a Wi-Fi analyzer
* [Nirsoft.WirelessKeyView](https://www.nirsoft.net/utils/wireless_key.html) - Recover wireless network key
* [ubiquity.WiFiman](https://play.google.com/store/apps/details?id=com.ubnt.usurvey) - Dynamic visualization of your WiFi signal and more. [homepage](http://wifiman.com/)  

## fax
* [Snappy Fax](https://www.snappysoftware.com/) - Sending and receiving fax, forward to email
* [VentaFax](http://www.ventafax.com/) - Sending and receiving fax and voice messages via a fax modem

## modem
* [AnalogX.CallerID](http://www.analogx.com/contents/download/System/callerid/Freeware.htm)
* [CallClerk.Caller ID](https://callclerk.com/index.html)
* [VZ Enhanced 56K](https://erickutcher.github.io/) - Caller ID notifier  

## share
* [Rejetto.HFS](http://www.rejetto.com/hfs/) - Use it to send and receive files
* [voidtools.Everything](https://www.voidtools.com/) - how to [enable HTTP server](https://www.voidtools.com/support/everything/http/)  

## misc
* [atkinsio.Bookmarks HTML Generator](https://github.com/atkinsio/bookmarks-html-generator)
* [Clean Flash Installer](https://github.com/CleanFlash/installer) - the mission of keeping the original Flash Player alive
  * [FlashPatch](https://github.com/darktohka/FlashPatch) - modifies the Flash Player installation, making it possible to play flash files &nbsp; ([adobe.setup Firefox/Chrome](https://www.flash.cn/flashplayer/3400192/install_flash_player_ppapi_cn.exe)) &nbsp; ([adobe.setup activeX](https://www.flash.cn/flashplayer/3400192/install_flash_player_ax_cn.exe))
* [ContaCam](https://www.contaware.com/contacam.html) - webcam recording and motion detection  
* [q](https://github.com/natesales/q) - DNS client with support for UDP, TCP, DoT, DoH, DoQ and ODoH  
* [Tired of Paywalls and Login Screens](www.thisischip.com/)  
