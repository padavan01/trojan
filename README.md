# 系统要求及脚本介绍
1、系统>=centos7，用centos8最好，内核可直接开启bbr不需升级。

2、域名解析到VPS并生效。

3、脚本自动续签https证书

4、自动配置伪装网站，位于/usr/share/nginx/html/目录下，可自行替换其中内容

# 一、使用一键脚本安装
curl -O https://raw.githubusercontent.com/padavan01/trojan/master/trojan_centos7.sh && chmod +x trojan_centos7.sh && ./trojan_centos7.sh

# 另外建议安装bbr，来源于网络分享，以下脚本安装，建议用原版bbr加速，不赘述了
cd /usr/src && wget -N --no-check-certificate "https://raw.githubusercontent.com/padavan01/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
