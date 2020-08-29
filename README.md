>这是一个在 Proxmox VE 5.x/6.x 中安装 OpenMediaVault 的脚本。

## 新的systemd-nspawn版本 ##

增加一个新的systemd-nspawn版本： [systemd-v1.0](https://github.com/ivanhao/OmvInPve/tree/systemd-v1.0)
好处是不污染主系统，随用随抛,与主系统隔离。
用`./install.sh`来安装。

## 安装说明 ##
#### 本人更改了脚本内容，支持 Proxmox VE 5.x和6.x安装。国内用户请执行`./OpenMediaVault-in-Proxmox_VE-CN.sh`来安装，国外用户请执行`./OpenMediaVault-in-Proxmox_VE-EN.sh`来安装。
#### 感谢“proxmox研究”群的  灬心海ζ丶 提供的安装方式，我只是在他的基础上整理了一键安装的脚本。我是群里的龙天，如果这个脚本帮到你了，麻烦点一下右上角的star小星星^_^

1.  clone 或下载安装包到 Proxmox VE 里，例如在 /root 目录运行：`git clone https://github.com/zhz8888/OpenMediaVault-in-Proxmox_VE.git`。
2. 命令行 cd 到安装包的路径里。
3. 执行`chmod +x ./*.sh`来让程序有执行的权限。
4. 执行`./OpenMediaVault-in-Proxmox_VE-CN.sh`来安装，根据提示很快就完成了。然后刷新界面。

> 不要忘记执行前给 rpool 做个快照，以便恢复快照。
> 需要用 root 账号来运行。

## 卸载 ##

执行`apt-get autoremove openmediavault` 来卸载。
或者回滚你的 rpool 快照，重启。

##  Preview 预览 ##
![preview](./preview.png)

> 如果用 OpenMediaVault 共享 Proxmox VE 的 rpool ，需要设置 acl 权限：
```
zfs set aclinherit=passthrough rpool
zfs set acltype=posixacl rpool
```
#### 如果这个脚本帮到你了，麻烦点一下右上角的 star 小星星^_^

## QQ交流群: 878510703

![QQ](http://upload-images.jianshu.io/upload_images/4171480-e0204ead0fb41d5e.jpg)

## 如果觉得好的请捐赠一下^_^
![alipay](https://upload-images.jianshu.io/upload_images/4171480-04c3ebb5c11cfdf9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


感谢捐赠人员！

捐赠列表：

*韬祺（来源支付宝）
