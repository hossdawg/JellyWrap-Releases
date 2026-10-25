# JellyWrap

JellyWrap opens https://jellyfin.monstr.tv as a fullscreen Android application. Designed for phones, tablets and compatible Android/Google TV and Amazon Fire TV devices with a functioning system WebView. No ads or analytics added by the app.

## Download

[Download JellyWrap.apk](https://github.com/hossdawg/JellyWrap-Releases/releases/latest/download/JellyWrap.apk)

[Version history and SHA256 checksums](https://github.com/hossdawg/JellyWrap-Releases/releases)

See [version metadata](version.json) for the current version. The direct public APK above is available without GitHub login. [Checksums](SHA256SUMS) · [Version metadata](version.json).

[JellyWrap 1.1.2 release](https://github.com/hossdawg/JellyWrap-Releases/releases/tag/v1.1.2) is published with the signed APK and SHA256SUMS. An alternative direct URL is https://raw.githubusercontent.com/hossdawg/JellyWrap-Releases/main/JellyWrap.apk. Build, lint, update-policy unit tests, signature verification and host-browser focus/zoom/fullscreen checks passed; real device installation, login persistence, playback/fullscreen and TV remote acceptance remain untested.

## Install using Downloader

Install Downloader by AFTVnews. Enable “Install unknown apps” for Downloader in device settings. Enter the download URL above, download JellyWrap.apk and choose Install. Open JellyWrap from your apps, then sign into Jellyfin. You can revoke the installer permission afterward.

A numeric Downloader code has not yet been registered. Maintainers can register the stable APK URL at https://go.aftvnews.com/ after publication, complete the service requirements, test the resulting code in Downloader, then document it here. A numeric code must come from that service; it cannot be selected by JellyWrap.

## Other installation methods

Download the APK in a browser and allow installation from that browser, or use `adb install -r JellyWrap.apk`. For updates, download the latest APK and install over the existing version. Login is retained with matching signing identity; uninstalling or clearing app data removes it. Version 1.1.0 adds 10% page zoom and automatic update checks when the app opens or resumes, at most every six hours. Install 1.1.0 manually once if you have 1.0.0. Future versions can be downloaded inside JellyWrap; choose Download update, then Install update. Android/Fire TV still requires installation confirmation and may ask you to allow JellyWrap to install unknown apps. Fullscreen video uses normal scale. APK updates are checked against the published checksum, package ID, newer version code and the existing signing identity. There is no silent installation or background update service. If your firmware cannot open the installer, continue using Downloader.

Android 6 or later and a working system WebView are required. Playback depends on system codecs and Jellyfin transcoding. Update WebView/system software if playback or navigation fails. Source code is maintained separately in a private repository.

Version 1.1.1 reduces TV remote navigation work and disables decorative TV card transitions and background backdrops. It keeps the 10% zoom and playback controls. Synthetic browser checks measure reduced DOM/layout work; actual performance on older Fire TV hardware still needs device testing.

Version 1.1.2 adds a yellow selection ring independent of Jellyfin theme outlines: circular around compact icons and rounded around larger controls/cards. The Moonfin header icon activates once on remote OK release. Inside Moonfin, native remote keys and its own focus indicator are used because its Flutter canvas is not an HTML control grid. Host tests pass; authenticated Moonfin and actual Fire TV remote operation still need device testing.
