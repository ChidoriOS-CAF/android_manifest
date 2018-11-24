ChidoriOS
===========
ChidoriOS is an AOSP based rom, meant to be as lightweight as possible. 
Our mission is to provide a stock-like experience even on low-end devices, allowing them to enjoy the latest version of Android.

How to Build?
-------------

To initialize your local repository:

```bash
  repo init -u git://github.com/ChidoriOS/manifest.git -b pie
```
  
Then to sync up:

```bash
  repo sync -c -jx --force-sync --no-clone-bundle --no-tags
```
Finally to build:

```bash
  . build/envsetup.sh
  lunch chidori_$device-userdebug
  mka bacon -jx
```
