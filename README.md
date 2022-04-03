# mtproto
Personal Telegram proxy

## Debian/Ubuntu:
```
apt-get install nodejs npm git
npm install pm2 -g
git clone https://github.com/FreedomPrevails/JSMTProxy.git
cd ./JSMTProxy/
# vim ./config.json # change secret: use only [a-f][0-9], length 32 is working
pm2 start mtproxy.js -i max
pm2 startup
firewall-cmd --add-port 6969/tcp
```
