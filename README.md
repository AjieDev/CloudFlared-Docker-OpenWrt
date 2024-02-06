# CloudFlared-Docker-OpenWrt
Run CloudFlare Tunnel a.k.a Argo Tunnel in docker container on OpenWrt

Features;
- Remote LuCI securely with SSL
- Port Forwarding
- Self-Hosted Web Server
  
<a style="color:red">You need at least 2GB storage.</a>

### Setup docker on Openwrt

<b> Install docker and docker compose (default repo by openwrt)</b>

```
opkg update && opkg install docker dockerd docker-compose
```

### Building docker container

<b> Clone this repo to your root/user folder</b>

```
git clone https://github.com/AjieDev/CloudFlared-Docker-OpenWrt.git .
```

<b>Edit docker-compose.yaml and enter your token</b> </br>

```
nano docker-compose.yaml
```
<b> Input you token after TUNNEL_TOKEN=</b></br>
![image](https://github.com/AjieDev/CloudFlared-Docker-OpenWrt/assets/86506499/83590b5c-7940-4fec-9b14-f3ae1f2b42e3)</br>
<b> Then Save it by CTRL+O and Enter , Exit it by CTRL+X</b>

<b>Build the container</b>

```
docker-compose up -d
```

<b> Then, You are Done!</b>
You can check it by
```
docker ps
```
