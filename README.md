Janus CVE-2017-13156 PoC

usage: janus.py dex apk out_apk

ART can run both APK and DEX, so here DEX ahead of base.apk is actually the one to execute.

* extract the original classes.dex
* use APKTOOL to do stuffs on it
* fuse the new dex into original APK
* update the installed app :)

This vulnerability was found by GuardSquare https://www.guardsquare.com/en/blog/new-android-vulnerability-allows-attackers-modify-apps-without-affecting-their-signatures
