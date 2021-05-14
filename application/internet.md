## Browser

Unofficial windows, [IceCat](https://github.com/muslayev/icecat-win64) (Firefox based) for ultra privacy. The official Linux [here](https://www.gnu.org/software/gnuzilla/).

[Brave](https://brave.com/) (Chrome based) for ultra privacy.

	* Automatically open Chrome DevTools debug - `"c:\chrome.exe" -auto-open-devtools-for-tabs`

----------


both IceCat & Brave when restarted getting new fingerprint.

Tested with :

  * [FingerprintJS](https://fingerprintjs.com/demo)
    * [cross-browser tracking(https://fingerprintjs.com/blog/external-protocol-flooding/)
  * [Unique Machine](http://uniquemachine.org/)  

test browser [permissions](https://permission.site/).

----------

**Mozilla.Firefox** v86 Introduces [Total Cookie Protection](https://blog.mozilla.org/security/2021/02/23/total-cookie-protection/) (you have to enable **strict mode** on privacy setings)  
**Mozilla.Firefox** v87 Introduces [SmartBlock](https://blog.mozilla.org/security/2021/03/23/introducing-smartblock/) (NoScript and uBlock Origin teams helping this approach)
**Mozilla.Firefox** v88 isolates [window.name](https://www.mozilla.org/en-US/firefox/88.0/releasenotes/) data

get latest [here](https://www.mozilla.org/en-US/firefox/all/#product-desktop-release).

addons :

  * Chrome-like [translate](https://github.com/FilipePS/Traduzir-paginas-web/) functionality (aka on the fly) to Firefox - Filipe Ps.Translate Web Pages
  * Browsec [VPN](https://addons.mozilla.org/en-US/firefox/addon/browsec/) free & fast.

Chrome.[Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey-beta/gcalenpjmijncebpfijmoaglllgpjagf) / Firefox.[Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) -- [Youtube - dismiss sign-in script](https://greasyfork.org/de/scripts/412178-youtube-dismiss-sign-in)

[SponsorBlock](https://sponsor.ajay.app/) - Blocking Unwanted YouTube Video Segments.

[magnolia.Bypass Paywalls Clean]() - Add-on allows you to read articles from websites that implement a paywall. [chrome](https://gitlab.com/magnolia1234/bypass-paywalls-chrome-clean) / [firefox](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean)

## Minimal Browser
* [NetSurf](https://www.netsurf-browser.org/)
* [Nessie](https://www.radsix.com/)

## Password Manager

* KeePassXC

	I dont like the online systems, never use it.
	
	In case you still use the Roboform desktop edition export the existing logins by using the [following](https://www.pipiscrew.com/2015/08/app-roboform-to-keepass/) method.
	
	Use [Keepass v2.x](https://keepass.info/download.html) to import it. Then use the dbase with [KeePassXC](https://keepassxc.org/).
	
	**KeePassXC vs KeePass**
	
	Is a community-developed open-source fork of KeePass, one of the best password managers for Windows. KeePassXC differs from KeePass because it works on Linux, Mac, and Windows, but it also lacks some of the original software's features, such as plug-in support. [src](https://www.techradar.com/reviews/keepassxc)
	
	Then install the **KeePassXC-Browser addon** for [firefox](https://addons.mozilla.org/en-US/firefox/addon/keepassxc-browser/) or [chrome](https://chrome.google.com/webstore/detail/keepassxc-browser/oboonakemofpalcgghocfoadofidjkkk). 
	
	-
	
	The browser addons on [github](https://github.com/keepassxreboot/keepassxc-browser).
	
	WARNING the browser addon from github repository, has different signature by the one is on the marketplace… Possible when use the one by repository you have to download also the [KeePassXC](https://github.com/keepassxreboot/keepassxc) from the repository(?).. otherwise user getting something like “cant connect” error.
	
	-
	
	Connecting the application and extension, any adjustment made to tools > settings > browser integration, it saves the configuration under
	
	C:\Users\\%username%\AppData\Local\KeePassXC	
	
	official guide on [how to](https://keepassxc.org/docs/KeePassXC_GettingStarted.html#_setup_browser_integration)

* [bitwarden](https://bitwarden.com/) - the free online solution 
* [RoboForm](https://www.roboform.com/) - the well known

## FTP
* [FileZilla](https://filezilla-project.org/)
* [WinSCP](https://winscp.net/eng/index.php)

## Download Manager
* [HTTP Downloader](https://erickutcher.github.io/#HTTP_Downloader)
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
* [mRemoteNG](https://mremoteng.org/) - RDP connections manager
* (discontinued) [Microsoft.Remote Desktop Connection Manager](https://filehippo.com/download_remote_desktop_connection_manager/) - RDP connections manager

## KVM  
* [Microsoft.Garage Mouse without Borders](https://www.microsoft.com/en-us/download/details.aspx?id=35460) - Control computers from a single mouse and keyboard  
* [ShareMouse](https://www.sharemouse.com/) - Control multiple computers from a single mouse and keyboard  
* [Synergy](https://symless.com/synergy) - Share your mouse and keyboard via network  

## Image Upload
* [MyImgur](http://myimgur.eden.fm/)
* [EasyImgur](https://bryankeiren.com/easyimgur/)

## Mail
* [Mozilla.Thunderbird](https://www.thunderbird.net/)
* [Desksoft.CheckMail](http://www.desksoft.com/CheckMail.htm)
* [POP Peeper: Email Notifier](https://www.esumsoft.com/products/pop-peeper/) - email notifier that runs in your Windows taskbar
* [MailStore Home](https://www.mailstore.com/en/products/mailstore-home/) - Central archive for all emails. Reads mbox / pst / thunderbird (unicode, in search use * for wildcard, because searching by words). 

## Mail mbox
* [BitRecover.mbox viewer](https://www.bitrecover.com/free/mbox-viewer/) - direct browse mbox (no so good on search, tip use F3 after the first search)
* [BitRecover.mbox Converter Wizard](https://www.bitrecover.com/mbox-converter/) - convert gmail mbox to pst, with attachments
* [Thunderbird addon - ImportExportTools NG](https://addons.thunderbird.net/en-US/thunderbird/addon/importexporttools-ng/) - convert gmail mbox to thunderbird. The original [addon](https://addons.thunderbird.net/en-US/thunderbird/addon/importexporttools/) supports 14.x - 16.x
* [PST Walker](https://www.pstwalker.com/pstwalker.html) - light & portable by company, use it in combination with the mbox2pst (super search + unicode + attachments)

## RSS
* [QuiteRSS](https://quiterss.org/)
* [RSS Guard](https://github.com/martinrotter/rssguard)

## wifi
* [Nirsoft.WifiInfoView](https://www.nirsoft.net/utils/wifi_information_view.html) - Scans the wireless networks in your area and displays extensive information
* [Passmark.WirelessMon](https://www.passmark.com/products/wirelessmonitor/) - Monitor wireless adapters and WiFi access points
* [faproc.Wifi Analyzer](https://play.google.com/store/apps/details?id=com.farproc.wifi.analyzer) - Turns your android phone into a Wi-Fi analyzer
* [Nirsoft.WirelessKeyView](https://www.nirsoft.net/utils/wireless_key.html) - Recover wireless network key

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
