#用的是大佬 https://github.com/VIKINGYFY/OpenWRT-CI 的源码, 增加了几个软件; 

#软件列表:

luci-app-samba4 | luci-app-cpufreq | luci-app-wolplus | luci-app-tailscale | luci-app-autoreboot | luci-app-advancedplus | luci-theme-kucat | luci-app-openclash | luci-app-passwall | luci-app-frpc | luci-app-syncthing | luci-app-zerotier | luci-app-vsftpd | luci-app-acl

有bug, 软件无法安装更新; 不知道在编释时如何替换源, 解决方法: 安装后在opkg配置--/etc/opkg/distfeeds.conf 删除原有的用以下替换:

src/gz openwrt_base https://archive.openwrt.org/releases/packages-23.05/aarch64_cortex-a53/base

src/gz openwrt_luci https://archive.openwrt.org/releases/packages-23.05/aarch64_cortex-a53/luci

src/gz openwrt_packages https://archive.openwrt.org/releases/packages-23.05/aarch64_cortex-a53/packages

src/gz openwrt_routing https://archive.openwrt.org/releases/packages-23.05/aarch64_cortex-a53/routing

src/gz openwrt_telephony https://archive.openwrt.org/releases/packages-23.05/aarch64_cortex-a53/telephony




# 固件简要说明：

固件每天早上4点自动编译。

固件信息里的时间为编译开始的时间，方便核对上游源码提交时间。

MEDIATEK系列、QUALCOMMAX系列、ROCKCHIP系列、X86系列。

# 目录简要说明：

workflows——自定义CI配置

Scripts——自定义脚本

Config——自定义配置
