We can install Privoxy in Raspberry Pi to use it as proxy server to crawl data
```
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install privoxy
sudo nano /etc/privoxy/config
- edit listen-address :8118
sudo systemctl restart privoxy
sudo systemctl status privoxy
curl ipinfo.io -x proxyip:port
```


https://www.howtogeek.com/683971/how-to-use-a-raspberry-pi-as-a-proxy-server-with-privoxy/