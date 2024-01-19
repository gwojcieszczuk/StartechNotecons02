## Startech NOTECONS02 USB Crash Cart Adapter software, version 118.1017

![startech256.png](misc/startech256.png)
* Repackaged as AppImage (x86_64)
* [Download Link](https://webserver.inode.ws/Startech/Startech-NOTECONS02-USB-Crash-Cart-Adapter-2401191147-x86_64.AppImage)
* To be used with the following hardware:
   * [https://www.startech.com/en-us/server-management/notecons02](https://www.startech.com/en-us/server-management/notecons02)
   * [https://www.startech.com/en-us/server-management/notecons02x](https://www.startech.com/en-us/server-management/notecons02x)
* List of supported and tested Linux distributions

  Anything older than Ubuntu 20.04 LTS should work.

<br>

* List of changes made to original software
  * removed `libz.so.1`
  * removed `libstdc++.so.6`
  * replaced `ffmpeg-lin` with static build of ffmpeg release 6.0

## Using AppImage package

AppImage file can be launched from GUI or CLI. You will need to initially use CLI to create persistent UDEV rule for your Startech adapter device.

Show supported list of Linux distributions.

```console
./Startech-NOTECONS02-USB-Crash-Cart-Adapter-XXXXXXXX-x86_64.AppImage supported
```

Show version of current AppImage build.

```console
./Startech-NOTECONS02-USB-Crash-Cart-Adapter-XXXXXXXX-x86_64.AppImage version
```

Create persistent UDEV rule on your system. Without this step, Startech software won't be able to access adapter device if you're running AppImage as a non-root user.

```console
sudo ./Startech-NOTECONS02-USB-Crash-Cart-Adapter-XXXXXXXX-x86_64.AppImage udev-install
```
