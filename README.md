#用的是大佬 https://github.com/VIKINGYFY/OpenWRT-CI 的源码, 增加了几个软件; 

#软件列表:

luci-app-samba4 | luci-app-cpufreq | luci-app-wolplus | luci-app-tailscale | luci-app-autoreboot | luci-app-advancedplus | luci-theme-kucat | luci-app-openclash | luci-app-passwall | luci-app-frpc | luci-app-syncthing | luci-app-zerotier | luci-app-vsftpd | luci-app-acl





# 固件简要说明：

固件每天早上4点自动编译。

固件信息里的时间为编译开始的时间，方便核对上游源码提交时间。

MEDIATEK系列、QUALCOMMAX系列、ROCKCHIP系列、X86系列。

# 目录简要说明：

workflows——自定义CI配置

Scripts——自定义脚本

Config——自定义配置
