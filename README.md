# Tutorial-Pipe-Node-Installer
This is my documentation of my node project.

# Install Pipe Node (PoP Cache Node)

## **System Requirements**
- Linux (Ubuntu 20.04+)
- 24/7 Connectivity
- **Minimal** 4GB RAM & 100GB Storage
- **Pastikan Ports 80 dan 443 terbuka**

---

## **Tutorial Install**

### **Update Package**
```bash
sudo apt update && sudo apt upgrade -y
```

### **Download dan Install Pipe Node**
```bash
curl -L -o pop "https://dl.pipecdn.app/v0.2.8/pop"
chmod +x pop
```

### **Buat Folder untuk Cache**
```bash
mkdir download_cache
```

### **Gunakan Referal**
```bash
sudo ./pop --signup-by-referral-route 8e03431981c3fdb2
```

### **Start Node**
```bash
screen -S pipe
sudo ./pop --ram 4 --max-disk 100 --cache-dir ./download_cache --pubKey <Solana Wallet Address>
```
* Gantilah <Solana Wallet Address> dengan alamat wallet Solana Anda!
* Anda bisa menyesuaikan RAM dan disk dengan nilai yang lebih besar sesuai kapasitas server.
* Screen Optional

---

## **Basic Commands**
```bash
# Cek Node ID
nano ~/node_info.json
# Generate Referal
./pop --gen-referral-route
# Cek Poin
./pop --points
# Cek Status Node
./pop --status
# Masuk Screen Pipe
screen -r pipe
# Keluar Screen
CTRL+A+D
```
---
### 🔗 Dashboard Node: https://dashboard.pipenetwork.com/node-lookup
### 🔗 Official Website: https://pipe.network/
### 🔗 Tutorial Resmi: https://docs.pipe.network/devnet-2#monitor

### 🔥 Goodluck! 🚀

