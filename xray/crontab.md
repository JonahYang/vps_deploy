12 3 * * * (/usr/bin/wget -v -N  https://github.com/crab21/v2ray-rules-dat/releases/latest/download/geoip.dat -O /root/xray/geoip.dat)
13 3 * * * (/usr/bin/wget -v -N  https://github.com/crab21/v2ray-rules-dat/releases/latest/download/geoip.dat -O /root/xray/geoip.dat)
10 3 * * * (/usr/bin/wget -v -N  https://github.com/crab21/v2ray-rules-dat/releases/latest/download/geosite.dat -O /root/xray/geosite.dat)
11 3 * * * (/usr/bin/wget -v -N  https://github.com/crab21/v2ray-rules-dat/releases/latest/download/geosite.dat -O /root/xray/geosite.dat)
12 4 * * * (ls /etc/systemd/system | grep xray | xargs systemctl restart)
0 0,12 * * * (/bin/bash /root/xray/vnstat.sh)