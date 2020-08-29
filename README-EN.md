>This is a omv4 install in proxmox ve 5.3/5.4/6.0 shell script.

## new systemd-nspawn ##

add new systemd-nspawn version in [systemd-v1.0](https://github.com/ivanhao/OmvInPve/tree/systemd-v1.0)
use `./install.sh` to install.

## install guide ##

1. clone or download the code to your proxmox ve. `git clone https://github.com/ivanhao/OmvInPve.git`
2. cd to the path
3. execute the `chmod +x ./*.sh` command to make it have right permission to execute the install or uninstall.
4. `./OmvInPve.sh` to install.
> Don't forget to make a snapshot for rpool before run it.

> you must run this script as `root`.

## uninstall guide ##
`apt-get autoremove openmediavault`
or
rollback your zfs rpool's snapshot and reboot.
