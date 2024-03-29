---
title: Invisible way to manage OS X Applications
date: 2023/6/13
categories:
- OS X
---

I'm not fond of receiving various types of notifications and badges, especially those related to app updates. They tend to disrupt my focus when I'm working or attending to personal tasks.

Moreover, the process of installing apps from the app store can be quite bothersome due to the overwhelming number of bright recommendations that compete for attention.

From the moment I installed Homebrew, I was hooked. Recently, I discovered Homebrew Cask, which has brought a new level of sophistication, ease, and efficiency to installing and managing GUI-based macOS applications like Postman and Mozilla.

However, one issue that remained was with regards to the AppStore. Unfortunately, there are several applications that could only be acquired exclusively through it, and thus cannot be replaced.

Fortunately, I discovered the mas-cli package, which can be located and installed using brew. This is the ideal solution for interacting with the AppStore.

While I won't provide an exhaustive list of commands, there are a few worth mentioning.

``` zsh
$ mas list
1619602800  Sticky Notes  (1.0.5)
1508833245  Floating      (44)
```

Just look for way you could install app now

``` zsh
$ mas lucky twitter
==> Downloading Twitter
==> Installed Twitter
```

Or keep all applications up-to-date

``` zsh
$ mas upgrade
Upgrading 2 outdated applications:
Xcode (7.0), Screens VNC (3.6.7)
==> Downloading Xcode
==> Installed Xcode
==> Downloading iFlicks
==> Installed iFlicks
```

That's why I love Unix. Everything could be done with console commands. It's fast and simple.
