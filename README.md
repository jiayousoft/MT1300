此项目专门为 GL-iNet MT1300 打造，感谢P3TERX的GitHub Actions项目。

感谢Lienol和Lean两位大神所提供的插件。

使用 GL-iNet 官方19.07.2源码，添加了Lienol和Lean两位大神的部分插件。

修改 .config 文件触发自动编译

目前GL源码的MT1300 profile不带WIFI驱动，如果需要，可以自己选择7615驱动，但是此驱动好像还有些问题：
1. 不能2.4G和5G两路WIFI，只能有1路。
2. 另外从WIFI连接不知道为什么DHCP拿不到地址。

建议使用GL官方的固件，然后搭配这里的ipk插件包。

此编译的固件 OpenWrt_firmware_gl-mt1300_yyyymmddhhmm 中已经包含插件包 mt1300-酸酸乳片.tar.gz。
ssh上传mt1300-酸酸乳片.tar.gz到GL官方固件下，然后执行install-酸酸乳片.sh即可。


2020-01-21 新增从Lean编译的固件，使用 .config.lean 触发编译
