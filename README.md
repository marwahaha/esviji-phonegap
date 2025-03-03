# PhoneGap port of the esviji web game

<img src="https://upload.wikimedia.org/wikipedia/fr/7/74/Logo_phonegap.png" alt="PhoneGap" width="180" align="right" />

## Introduction

This is a project to port [the esviji Web puzzle game](http://esviji.com) to native apps for iOS and Android.

## ALL WHAT FOLLOWS IS OBSOLETE!

This part of the project (the PhoneGap port) has been [abandonned February 16th, 2016](https://twitter.com/esviji/status/699565462519042051) to focus on the more future proof Web only version.

The code as of this date is still available [in the `phonegap` branch of the esviji project](https://github.com/esviji/esviji/tree/phonegap).

## Creating/updating the source webapp

The `www/` folder is generated by [the `grunt phonegap` task available in the esviji project](https://github.com/esviji/esviji/blob/master/Gruntfile.js)

The PhoneGap `config.xml` file is generated from [the source config.xml file in the esviji project](https://github.com/esviji/esviji/blob/master/src/config.xml).

## Generating the native apps binaries

Adobe's free [PhoneGap Build](https://build.phonegap.com/apps/) service is used to generate iOS and Android apps binaries:
https://build.phonegap.com/apps/1864078/builds

## Uploading the binaries to the stores

### Android

The `.apk` file downloaded from PhoneGap Build is uploaded to [Google Play Developer Console](https://play.google.com/apps/publish/).

### iOS

The `.ipa` file downloaded from PhoneGap Build is uploaded to [iTunes Connect](https://itunesconnect.apple.com/) with the [Application Loader](https://itunesconnect.apple.com/docs/UsingApplicationLoader.pdf) Mac OS app.

Some of the [app properties are mandatory](https://developer.apple.com/library/ios/documentation/LanguagesUtilities/Conceptual/iTunesConnect_Guide/Appendices/Properties.html#//apple_ref/doc/uid/TP40011225-CH26-SW2) before any publication.
