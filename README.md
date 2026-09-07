# SLOW-DNS By inc🦜 

* SLOWDNS SCRIPT



THIS IS A SCRIPT FOR AUTO INSTALLATION OF SLOWDNS (DNSTT SERVER) WITH:

-SSH
-SSL
-DROPBEAR


**DNSTT Script**

## :heavy_exclamation_mark: Requirements

* A Linux-based operating system (Ubuntu) 
* Ubuntu 22.04 Server x86_64 / 22.04 Server x86_64
* Version 8.5 Preffered Ubuntu 22.04 Server x86_64
* It is recommended to use a new or formatted distro

# Installation for slow dns via ssh🖲️
```
rm -rf install; apt update; wget https://github.com/mamba07k/slow-dns/raw/main/install; chmod 777 install; ./install --start
```

# Installation for slow dns via socks😊
```
rm -rf install; apt update; wget https://github.com/mamba07k/slow-dns/raw/main/slowdns-socks; chmod 777 slowdns-socks; ./slowdns-socks --start
```

# Installation for slow dns via dropbear🐼
```
rm -rf install; apt update; wget https://github.com/mamba07k/slow-dns/raw/main/slowdns-drop; chmod 777 slowdns-drop; ./slowdns-drop --start
```

# Installation slow dns via ssl💡
```
rm -rf install; apt update; wget https://github.com/mamba07k/slow-dns/raw/main/slowdns-ssl; chmod 777 slowdns-ssl; ./slowdns-ssl --start
```
# After installing those install its manager now to manage scripts now install its manager
```
rm -rf install; apt update; wget https://github.com/mamba07k/slow-dns/raw/main/slowdns; chmod 777 slowdns; ./slowdns --start
```

# After Installation Command

```
iptables -I INPUT -p udp --dport 5300 -j ACCEPT

iptables -t nat -I PREROUTING -p udp --dport 53 -j REDIRECT --to-ports 5300

lsof -i :5300
```
# TO ACCESS THE MANAGER USE COMMAND🔥
```
slowdns
```


