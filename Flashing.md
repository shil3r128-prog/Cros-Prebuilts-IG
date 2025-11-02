# Flashing

### On Windows, MacOS, ChromeOS (Not linux)

Go to the chrome webstore and install the extension called "Chromebook Recovery Utility"

Download the thing you want to flash (unzip it if you need to) to the USB and then open the extension. 
Click on the cog in the top right and select "Use local image" then select what you want to flash then flash it.

### Linux
You will probably need basic linux command line knowledge to do this 
Install p7zip to unzip if the file needs to be unzipped and the unzipped file is over 4GB with the commands below 

on Ubuntu or Debian based distros (For most beginner distros)
``` sudo apt update ```

``` sudo apt install p7zip ```

``` 7z x filename.bin.zip ```

then you will need to flash the USB

```lsblk```

(find your usb from that command)
**Try not to flash the wrong drive since this command is dangerous**

```sudo dd if=filename.bin.zip of=/dev/sdX```
