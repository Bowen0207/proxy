#remote-ssh
ssh-keygen -R 149.28.235.11

域名，西部数码
dns，https://dash.cloudflare.com/
vps，https://www.vultr.com

about.wintersnowsakura.top
about.xiaomage.shop
about.dakeai2023.xyz
about.jerryzhou.shop
about.stevenproxy.top

bash ssh-install.sh 2
bash xary-install.sh 3
bash warp-install.sh proxy

#ssh
https://github.com/wulabing/Xray_onekey 
wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/wulabing/Xray_onekey/main/install.sh" && chmod +x install.sh && bash install.sh 2

#xary
apt install docbook
apt install autoconf
https://github.com/2dust/v2rayN
bash <(curl -Ss https://www.idleleo.com/install.sh) 3

#gpt
https://missuo.me/posts/cloudflare-warp-chatgpt/
bash <(curl -fsSL git.io/warp.sh) proxy
vi /etc/idleleo/conf/xray/config.json
# custom_outbound.json
{
    "tag": "socks5-warp",
    "protocol": "socks",
    "settings": {
        "servers": [{
            "address": "127.0.0.1",
            "port": 40000
        }]
    }
}
# route.json
{
    "type": "field",
    "outboundTag": "socks5-warp",
    "ip": ["::/0"]
}

systemctl restart xray


#Block ads
curl -s -S -L https://raw.githubusercontent.com/AdguardTeam/AdGuardHome/master/scripts/install.sh | sh -s -- -v
sudo /opt/AdGuardHome/AdGuardHome -s restart
you can control the service status with the following commands:
sudo /opt/AdGuardHome/AdGuardHome -s start|stop|restart|status|install|uninstall
