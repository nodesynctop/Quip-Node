# Quip-Node
One-Click Installer for Quip Node (Ubuntu)

Dashboard: `https://quipstats.test-hub.xyz`

X: `https://x.com/quipnetwork`

# Quests

👉 https://quest.quip.network/airdrop?referral_code=9T3DNNOA

You should run the node using the wallet that participated in the quest, because your node will earn points for the quest.

## ⚠️ Requirements
- VPS (Ubuntu 22.04 / 24.04)
- Minimum: 2 - 4 CPU / 8GB RAM
- Open port: 20049 (TCP + UDP)
- Installation of required packages
 ```
sudo apt update && sudo apt upgrade -y
sudo apt install curl git wget htop tmux build-essential jq make lz4 gcc unzip -y
 ```
## One-line Install
```
wget -O install.sh https://raw.githubusercontent.com/nodesynctop/Quip-Node/refs/heads/main/install.sh
chmod +x install.sh
sudo bash install.sh
```
### 👉 Node Name
Example:
`nodename`

### 👉 Wallet Address
You must enter a valid EVM wallet address:
```
0x2264465ddf34sf...
```
## 📦 What this script does

When you run the installer:

🔄 Update Ubuntu system

🐳 Auto install Docker (if missing)

📥 Pull Quip Node image

🚀 Deploy node in Docker container

🔁 Enable auto-restart on reboot

📊 Start node logging automatically

## 📊 Check node status
```
docker logs -f quip-node
```
## 🔁 Restart node
```
docker restart quip-node
```
## 🧹 Remove node
```
docker stop quip-node
docker rm -f quip-node
rm -rf ~/quip-data
```
