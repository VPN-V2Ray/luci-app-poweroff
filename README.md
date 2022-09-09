# luci-app-poweroff

#Before the OpenWRT router system is compiled, run the following command to integrate the shutdown function into the system menu, and then the shutdown function from the menu can be realized.

cd openwrt

curl -fsSL  https://raw.githubusercontent.com/VPN-V2Ray/luci-app-poweroff/main/luci-app-poweroff/poweroff.htm > ./feeds/luci/modules/luci-mod-admin-full/luasrc/view/admin_system/poweroff.htm 

curl -fsSL  https://raw.githubusercontent.com/VPN-V2Ray/luci-app-poweroff/main/luci-app-poweroff/system.lua > ./feeds/luci/modules/luci-mod-admin-full/luasrc/controller/admin/system.lua
   
#OpenWRT路由器系统编译前，运行如下命令将关机功能集成到系统菜单中，即可实现从菜单中关机功能。

luci-app-poweroff
