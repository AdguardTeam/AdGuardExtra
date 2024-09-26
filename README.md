# AdGuard Extra

AdGuard Extra is a userscript (or a browser extension) that is supposed to fight ad blocking circumvention attempts which become more and more and popular. Regular ad blocking rules do not allow us being as flexible as it's necessary, that's why AdGuard Extra was developed.

AdGuard Extra comes pre-installed with all premium AdGuard apps, which support userscripts, i.e for AdGuard for Windows, AdGuard for Mac, and AdGuard for Android you won't need to do anything to use it.
However, if you want to use it alongside AdGuard browser extension or any other ad blocker, you'll need to use an additional extension.

## How to install AdGuard Extra

### Chrome or Chromium-based browser

* **Stable version**: https://agrd.io/adguard_extra_chrome_release
* Beta: https://agrd.io/adguard_extra_chrome_beta

### Firefox

* **Stable version**: https://agrd.io/adguard_extra_firefox_release
* Beta: https://agrd.io/adguard_extra_firefox_beta

### Userscript

1. Install Tampermonkey
2. Click the following link to install AdGuard Extra: https://userscripts.adtidy.org/release/adguard-extra/1.0/adguard-extra.user.js

If you are using Tampermonkey version 5.1 or lower you need also change Inject Mode:

1. Open Settings and switch the mode to Advanced.
2. Scroll down the settings page and locate the Inject Mode option.
3. Change Inject Mode to Instant.

Alternatively, you can install the beta version of AdGuard Extra userscript: https://userscripts.adtidy.org/beta/adguard-extra/1.0/adguard-extra.user.js

## How to exclude websites

### Userscript

You can restrict userscript from working on certain websites by adding `@exclude` rule to the userscript header. For example, to exclude `example.com`, you should add the following line to the userscript header:
```
// @exclude  *://example.com/*
// @exclude *://*.example.com/*
```

When using Tampermonkey, you can also use the built-in editor to add the rule. To do so, open the userscript settings, and add the pattern to the `Blacklisted Pages` field of `Security` section.

### Extension

AdGuard Extra extension can be restricted to specific websites in Chrome with `Allow site access` option of the extension settings.

## Important

AdGuard Extra is a companion extension, it is supposed to be used with a full-scale ad blocker like AdGuard or any other.

It provides no user interface save for the extension icon in the toolbar. Your browser should allow you to hide the icon if it annoys you.

Please note that it is only useful on a limited set of websites, and it does nothing on the websites not from this list.

For problematic sites that change their code frequently, the solution is only included in the AdGuard Extra Userscript version. This version can be installed via Tampermonkey or via the AdGuard app for Mac, Windows or Android.

* If you are using Tampermonkey, installation instructions can be found in [AdGuard Extra Userscript](https://github.com/AdguardTeam/AdGuardExtra?tab=readme-ov-file#userscript).

* If you use the AdGuard apps for Mac and Windows, simply enable AdGuard Extra in the `Extensions` section. In AdGuard for Android, you can enable AdGuard Extra in the `Userscript` section `Settings --> Filtering --> Userscripts`.

The repository provides a list of problematic sites labelled `problematic`.
