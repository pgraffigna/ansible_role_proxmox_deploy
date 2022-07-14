# ansible_proxmox_deploy

Playbook para crear contenedores via ansible en Proxmox-ve instalado en Virtualbox

roles:
- dependencias
- creacion_ct
- destruir_ct
- creacion_vms
- destruir_vm

---

proxmox script helper: [helper-scripts](https://tteck.github.io/Proxmox/)

---

Chequear que la API esta funcionando 

```bash
curl -k -d "username=root@pam&password=yourpassword" https://10.0.0.1:8006/api2/json/access/ticket
```
---

## instalacion ansible
```bash
apt update && apt install -y python3-pip
pip3 install --upgrade ansible
```
---

## en servidor proxmox: tener instalado proxmoxer
```bash
pip3 install proxmoxer 
```
---

## dependencias modulo proxmox
```bash
ansible-galaxy collection install community.general
```

