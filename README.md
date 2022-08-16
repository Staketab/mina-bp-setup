# MINA NODE SETUP
Setup Mina node with Uptime system (Snark and Sidecar).

## 1. Clone repository:

```
git clone https://github.com/Staketab/mina-bp-setup.git
```
## 2. Copy your data (Important)

Copy your keys (my-wallet and my-wallet.pub) in your `/home/user/keys/` or `/root/keys/` folder.  

### Then set permittions:
```
chmod 700 $HOME/keys
chmod 600 $HOME/keys/my-wallet
```

## 3. Start pre-install script:
```
cd mina-bp-setup \
&& chmod +x install.sh \
&& ./install.sh
```
## 4. Start the Node
Run this command to start the node:  
```
docker-compose up -d
```

Other commands:
1. Check status
```
docker exec -it mina mina client status
```
2. Stop docker-compose
```
docker-compose down
```
3. Docker-compose logs
```
docker-compose logs -f mina
```
```
docker-compose logs -f sidecar
```

# DONE
