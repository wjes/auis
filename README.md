# Arch Unattended Installation Script (AUIS)

Just a personal down-to-script of the official Arch Linux installation guide (https://wiki.archlinux.org/index.php/Installation_Guide)

After booting from the Arch Linux UEFI Live USB:

* Connect to the internet with wifi-menu
* Change the pacman mirror 
* Install git
* Download the repo:

```shell
git clone --single-branch --depth 1 https://github.com/wjes/auis.git
```
* Run the script:

```shell
chmod +x main.sh
# -upass : User password
# -rpass : Root password
# -r     : Reboot after finish
./main.sh [-upass <password>] [-rpass <password>] [-r] [-h]
```
* Profit!
