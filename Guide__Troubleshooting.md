# Troubleshooting Guide

᲼᲼

**Index**

- [Troubleshooting Guide](#troubleshooting-guide)
  - [Extension](#extension)
    - [Basic checks](#basic-checks)
    - [Check API status](#check-api-status)
    - [Check for Service Worker bug](#check-for-service-worker-bug)
    - [Install certificates](#install-certificates)
    - [Check for logs in console](#check-for-logs-in-console)
      - [In Chromium Based browsers](#in-chromium-based-browsers)
        - [Windows](#windows)
        - [MACs](#macs)
      - [In Firefox Based Browsers](#in-firefox-based-browsers)
        - [On Windows](#on-windows)
        - [On MACs](#on-macs)
  - [Userscript](#userscript)
  - [iOS app](#ios-app)
  - [YouTube Vanced  app](#youtube-vanced--app)
  - [Contact in Discord Server](#contact-in-discord-server)
  - [Useful Links](#useful-links)

᲼᲼

## Extension

(for Windows & MACs)

### Basic checks

1. Make sure you have latest version of extension installed (2.0.0.3)
2. Close all the tabs & restart your browser
3. Reinstall the extension.
4. [Check API status]
5. [Check service worker] (only for chromium based browsers)
6. [If you are on Windows 7 read this](#install-certificates)

<!-- metadata {
  "update_frequency": "every_release"
  "comment": "for now, if using bookdown.org, add a script to do it" 
} -->

<!-- TODO: automate the updating of version number -->

᲼᲼

### Check API status

If the basic checks didn't resolve anything

[See if you get any response from this link (click here)](https://returnyoutubedislikeapi.com/votes?videoId=QOFEgexls14)

If you **don't see something like** this, then the **API is down** and **everything is fine on your side**.

`{"id":"QOFEgexls14","dateCreated":"2021-12-28T02:53:20.995329Z","likes":2968,"dislikes":204,"rating":4.725047080979285,"viewCount":29157,"deleted":false}`

**If you see "Certificate error" and [if you are on Windows 7 (or earlier) read this](#install-certificates)**

᲼᲼

### Check for [Service Worker bug][5]

[in Chromium based browsers][1]

If nothing mentioned above this helped

1. Open any video on YouTube.
2. Open a new tab.
3. Type [chrome://extensions](chrome://extensions) in [address bar](https://en.wikipedia.org/wiki/Address_bar#Address_bar_implementations) (the [**topmost bar**](https://upload.wikimedia.org/wikipedia/commons/6/68/HTTPS_and_padlock_in_website_address_bar.jpg) below tabs)
4. Find the extension.
5. If its written <span style="color: red">`service worker (Inactive)`</span> in red, then the problem is with your browser.

**This is not a bug in the extesnion.** This is a bug in the browsers. **We cannot do anything about this.**

᲼᲼

### Install certificates

**Applies for Windows 7 (and earlier) only**

and only for  [Chromium Based Browsers][1]

- [Chromium based browsers][1] don't have their own certificate manager.
- They use Windows' certificates manager.

You can Follow this guide:

[Fix error NET::ERR CERT DATE INVALID - Your connection is not private - Windows 7 - 2021](https://youtu.be/JYZLxP2Z8G4)

If you don't want to install the certificate from Google drive

- Here is the official link to the certificate [**x1.i.lencr.org**](http://x1.i.lencr.org/).
- **You will have to close all the tabs** before downloading this certificate.

**The thumb print of real certificate is `cabd2a79a1076a31f21d253635cb039d4329a5e8`**

**To make sure that you have installed the correct certificate, you should consider checking if the thumbprints match.** To do this you can follow this guide: [How to check a certificate's thumbprint](https://knowledge.digicert.com/solution/SO9840.html)

᲼᲼

### Check for logs in console

#### [In Chromium Based browsers][1]

##### Windows

1. Press `Ctrl` + `Shift` + `J` all at one
2. Find `filter` box in the newly appeared window.
3. Type `Return`.
4. If you see any errors in red [please contact us][4] and report them in our [discord server][3]

##### MACs

1. Press `Cmd` + `Option` + `J` all at one
2. Find `Filter` box in the newly appeared window.
3. Type `Return`.
4. If you see any errors in red [please contact us][4] and report them in our [discord server][3]

᲼᲼

#### [In Firefox Based Browsers][2]

##### On Windows

1. Press `Ctrl` + `Shift` + `K` all at one
2. Find `Filter Output` box in the newly appeared window.
3. Type `Return`.
4. If you see any errors in red [please contact us][4] and report them in our [discord server][3]

##### On MACs

1. Press `Cmd` + `Option` + `K` all at one
2. Find `Filter Output` box in the newly appeared window.
3. Type `Return`.
4. If you see any errors in red [please contact us][4] and report them in our [discord server][3]

᲼᲼

᲼᲼

## Userscript

⚠ Under Construction

᲼᲼

᲼᲼

## iOS app

Coming soon. Please have patience.

᲼᲼

᲼᲼

## YouTube Vanced  app

Coming soon. Please have patience.

᲼᲼

᲼᲼

## Contact in Discord Server

**Only if nothing mentioned above helped and you still have problem.**

[Discord server link: https://discord.gg/mYnESY4Md5][3]

0. Join the discord server if haven't already
1. Go to #Bugs-and-problems channel
2. Thoroughly your problem there.

<!-- {
  "update_frequency" : "low"
} -->

᲼᲼

᲼᲼

## Useful Links

[List of Chromium Based Browsers][1]

[List of Firefox Based Browsers][2]

[Return-YouTube-Dislike Discord Server][3]

[Service Worker Bug in Chromium Based Browsers][5]

<!-- links -->

[1]: https://en.wikipedia.org/wiki/Chromium_(web_browser)#Browsers_based_on_Chromium

[2]: https://en.wikipedia.org/wiki/Category:Web_browsers_based_on_Firefox

[3]: https://discord.gg/mYnESY4Md5

[4]: #contact-in-discord-server

[5]: https://bugs.chromium.org/p/chromium/issues/detail?id=1271154
