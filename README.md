# ansible_proxmox_deploy

Playbook para crear contenedores via ansible en Proxmox-ve instalado en Virtualbox

roles:	
- dependencies 
- ct

---

dark_mode:
```bash
wget https://raw.githubusercontent.com/Weilbyte/PVEDiscordDark/master/PVEDiscordDark.py
python3 PVEDiscordDark.py
```
---

Chequear que la API esta funcionando 

```bash
curl -k -d "username=root@pam&password=yourpassword" https://10.0.0.1:8006/api2/json/access/ticket
```
---

Chequear dependencias:

en host: tener instalado ansible
```bash
pip3 install --upgrade ansible
```
---

en servidor: tener instalador los paquetes proxmoxer y requests
```bash
pip3 install proxmoxer requests
```
---

para instalar pip:
```bash
apt update && apt upgrade && apt install -y python3-pip 
```

