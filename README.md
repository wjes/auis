# Arch Unattended Installation Script (AUIS)

Just a personal down-to-script of the official Arch Linux installation guide (https://wiki.archlinux.org/index.php/Installation_Guide)

After booting from the Arch Linux UEFI Live USB:

* Connect to the internet with `wifi-menu`
* Change pacman's mirror list `vim /etc/pacman.d/mirrorlist`
* Install git `pacman -S git`
* Download the repo:

__Vanilla__

```shell
git clone --single-branch --depth 1 https://github.com/wjes/auis.git
```

__Laptop__

```shell
git clone --single-branch --depth 1 --branch laptop https://github.com/wjes/auis.git
```

__Desktop__

```shell
git clone --single-branch --depth 1 --branch desktop https://github.com/wjes/auis.git
```

__Chromebook__

```shell
git clone --single-branch --depth 1 --branch chromebook https://github.com/wjes/auis.git
```

* Run the script:

```shell
# -upass : User password
# -rpass : Root password
# -r     : Reboot after finish
./main.sh [-upass <password>] [-rpass <password>] [-r] [-h]
```
* Profit!
