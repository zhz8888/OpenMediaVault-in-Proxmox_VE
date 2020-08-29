>This is a OpenMediaVault install in Proxmox VE 5.x/6.x shell script.

## New systemd-nspawn ##

Add new systemd-nspawn version in [systemd-v1.0](https://github.com/ivanhao/OmvInPve/tree/systemd-v1.0).
Use `./install.sh` to install.

## Install Guide ##

1. Clone or download the code to your proxmox ve. `git clone https://github.com/zhz8888/OpenMediaVault-in-Proxmox_VE.git`.
2. Cd to the path.
3. Execute the `chmod +x ./*.sh` command to make it have right permission to execute the install or uninstall.
4. Execute the`./OpenMediaVault-in-Proxmox_VE-EN.sh` to install.

> Don't forget to make a snapshot for rpool before run it.You must run this script as `root`.

## Uninstall Guide ##
Execute the`apt-get autoremove openmediavault` or rollback your zfs rpool's snapshot and reboot.

##  Preview ##
![preview](./preview.png)
