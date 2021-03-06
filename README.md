#  Windows udp2raw+kcptun 加速tcp流量 简易工具  by 蘭雅sRGB
蘭雅sRGB 龙芯小本服务器 | [sRGB.vicp.net](http://sRGB.vicp.net)

![](https://raw.githubusercontent.com/hongwenjun/WinKcp_Launcher/master/gui.png)

## Shadowsocks + Kcp+Udp2Raw加速 和 Udp2Raw服务TCP伪装 WireGuard Windows Kcp+Udp2Raw 启动器 

使用视频链接   https://youtu.be/A4edsGXQdIc

### 使用说明:
1. 需要先安装 WinPcap_4_1_3.exe (已经包含和其他windows客户端)
2. 修改 Windows_KCP.cmd 里的服务器IP参数，让双击启动
3. 双击 WinKcp_Launcher 管理 Windows_KCP.cmd 启动关闭 
4. 电脑$$客户端设置  127.0.0.1:3322     密码:xxx  加密 aes-256-gcm
5. 手机$$填PC电脑IP  192.168.1.188:3322 密码:xxx  加密 aes-256-gcm

![](https://raw.githubusercontent.com/hongwenjun/WinKcp_Launcher/master/windows_kcp.gif)

### 参数参考  udp2raw+kcptun 加速tcp流量 Step by Step 教程
https://github.com/wangyu-/udp2raw-tunnel/blob/master/doc/kcptun_step_by_step.md


### 详细见
[Windows_KCP加速使用说明.txt](https://raw.githubusercontent.com/hongwenjun/WinKcp_Launcher/master/Windows_KCP加速使用说明.txt)

### 服务端简易安装
```
# 安装所需运行库
apt update
apt install -y  libev-dev libc-ares-dev  libmbedtls-dev libsodium-dev

# 安装脚本 sku
mkdir -p sku && cd sku && wget -O sku.tgz https://git.io/fxy7s && tar -xvf sku.tgz && ./sku.sh
```
### 服务端简易配置
-  vim sku_config.sh 然后 *./sku_congfi.sh* 启用配置
