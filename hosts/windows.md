# Windows

## VLAN

20

## Configuration réseau

Mode : DHCP

## Paramètres obtenus

- Adresse IP : DHCP
- Masque : 255.255.255.0
- Passerelle : 192.168.20.254
- DNS : 1.1.1.1 / 8.8.8.8
- Domaine : lab.net

## Vérification

```powershell
ipconfig /all
ping 192.168.20.254
tracert 192.168.30.1
```
