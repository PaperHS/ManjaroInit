# ManjaroInit
init terminal
```
sudo pacman-mirrors -c China
sudo pacman Syyu
sudo pacman -S yaourt git vim emacs
yaourt google-chrome
yaourt wechat
yaourt shadowsocksr
git clone https://github.com/breakwa11/gfw_whitelist.git
yaourt -S proxychains-ng
sudo vim /etc/systemd/system/shadowsocksr-libev-local@.service

[Unit]
Description=Shadowsocks-Libev Custom Client Service for %I
Documentation=man:ss-local(1)
After=network.target

[Service]
Type=simple
CapabilityBoundingSet=CAP_NET_BIND_SERVICE
ExecStart=/usr/bin/ss-local -c /etc/shadowsocksr-libev/config.json

[Install]
WantedBy=multi-user.target




sudo systemctl enable --now shadowsocksr-libev-local@config.service
```
