# JellyWrap

JellyWrap opens https://jellyfin.monstr.tv as a fullscreen Android application. Designed for phones, tablets and compatible Android/Google TV and Amazon Fire TV devices with a functioning system WebView. No ads or analytics added by the app.

## Download

[Download JellyWrap.apk](https://github.com/hossdawg/JellyWrap-Releases/releases/latest/download/JellyWrap.apk)

[Version history and SHA256 checksums](https://github.com/hossdawg/JellyWrap-Releases/releases)

The stable APK address always points to the latest published release. No GitHub login is required. Device compatibility testing status is documented in each release.

## Install using Downloader

Install Downloader by AFTVnews. Enable “Install unknown apps” for Downloader in device settings. Enter the download URL above, download JellyWrap.apk and choose Install. Open JellyWrap from your apps, then sign into Jellyfin. You can revoke the installer permission afterward.

A numeric Downloader code has not yet been registered. Maintainers can register the stable APK URL at https://go.aftvnews.com/ after publication, complete the service requirements, test the resulting code in Downloader, then document it here. A numeric code must come from that service; it cannot be selected by JellyWrap.

## Other installation methods

Download the APK in a browser and allow installation from that browser, or use `adb install -r JellyWrap.apk`. For updates, download the latest APK and install over the existing version. Login is retained with matching signing identity; uninstalling or clearing app data removes it. No automatic updater is included.

Android 6 or later and a working system WebView are required. Playback depends on system codecs and Jellyfin transcoding. Update WebView/system software if playback or navigation fails. Source code is maintained separately in a private repository.
