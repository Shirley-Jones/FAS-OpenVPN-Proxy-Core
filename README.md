# FAS-OpenVPN-Proxy-Core
## 使用方法
### 先创建OpenVPN四个配置文件 协议为TCP 端口号分别为 1194、1195、1196、1197 并启动
### 启动openvpn.bin（这个程序会将TCP 1194、1195、1196、1197 转发到443、3389用于免流）
### openvpn.bin -l 443 -d
### openvpn.bin -l 3389 -d
### 启动proxy.bin
### proxy.bin -l （线路proxy端口 例如8080） -d
### proxy.bin -l 8080 -d

完成！
