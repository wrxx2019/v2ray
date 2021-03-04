# v2ray
最好用的 V2Ray 一键安装脚本 &amp; 管理脚本

## 脚本说明
[V2Ray 一键安装脚本](https://github.com/233boy/v2ray/wiki/V2Ray%E4%B8%80%E9%94%AE%E5%AE%89%E8%A3%85%E8%84%9A%E6%9C%AC)

## 搭建教程
[V2Ray搭建详细图文教程](https://github.com/233boy/v2ray/wiki/V2Ray%E6%90%AD%E5%BB%BA%E8%AF%A6%E7%BB%86%E5%9B%BE%E6%96%87%E6%95%99%E7%A8%8B)

## 资助 V2Ray
请考虑 [资助 V2Ray 发展](https://www.v2ray.com/chapter_00/02_donate.html)

## 更多 V2Ray 教程文章
https://github.com/233boy/v2ray/wiki

依次点击文件夹config--->server--->include找到 ban.json文件，点击该文件，再点击文件上方的小铅笔图标，对文件内容进行修改。

改成如下格式即可，一定要保留一个域名，否则最后生成的配置文件会少一段，导致搭建的v2ray无法翻墙。改完之后，点击下面的“Commit changes”按钮保存。 { "type": "field", "domain": [ "domain:360.com" ], "outboundTag": "blocked" }

git clone https://github.com/wrxx2019/v2ray -b master 
cd v2ray 
chmod +x install.sh 
./install.sh local

如果提示 curl: command not found ，那是因为你的 VPS 没装 Curl

ubuntu/debian 系统安装 Curl 方法: apt-get update -y && apt-get install curl -y

centos 系统安装 Curl 方法: yum update -y && yum install curl -y

安装好 curl 之后就能安装脚本了

V2Ray 配置文件路径：/etc/v2ray/config.json

Caddy 配置文件路径：/etc/caddy/Caddyfile

脚本配置文件路径: /etc/v2ray/233blog_v2ray_backup.conf

v2ray info 查看 V2Ray 配置信息

v2ray config 修改 V2Ray 配置

v2ray link 生成 V2Ray 配置文件链接

v2ray infolink 生成 V2Ray 配置信息链接

v2ray qr 生成 V2Ray 配置二维码链接

v2ray ss 修改 Shadowsocks 配置

v2ray ssinfo 查看 Shadowsocks 配置信息

v2ray ssqr 生成 Shadowsocks 配置二维码链接

v2ray status 查看 V2Ray 运行状态

v2ray start 启动 V2Ray

v2ray stop 停止 V2Ray

v2ray restart 重启 V2Ray

v2ray log 查看 V2Ray 运行日志

v2ray update 更新 V2Ray

v2ray update.sh 更新 V2Ray 管理脚本

v2ray uninstall 卸载 V2Ray

service caddy restart/stop/start/status
