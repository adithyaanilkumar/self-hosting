# self-hosting

MEC AP WPA 2: 

pass word : 8b140b20e7

```
ip a | grep 192
```


u will get something like  : 192.168.2.100/22

type 192.168.2.100:3001 in ur phone browser
## GHOST

```
docker run -d --name some-ghost -e NODE_ENV=development -e url=http://localhost:3001 -p 3001:2368 ghost
````
## Install JellyFin

```
curl https://repo.jellyfin.org/install-debuntu.sh | sudo bash
```
or
```
wget -O- https://repo.jellyfin.org/install-debuntu.sh | sudo bash
```

```
localhost:8096
```

## Install Open Media Vault

```
wget -O - https://raw.githubusercontent.com/OpenMediaVault-Plugin-Developers/installScript/master/install | sudo bash
```

## Install Tailscale

```
curl -fsSL https://tailscale.com/install.sh | sh
```

## Install - Docker

```
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
```

```
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```

```
echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```


```
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

```
sudo docker run hello-world
```

## Install Portainer

```
docker volume create portainer_data
```

```
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest
```

```
https://localhost:9443
```



# 

