# Cisco Router-on-a-Stick Lab

## Description

Ce projet présente la mise en œuvre d'une architecture Cisco basée sur le principe du **Router-on-a-Stick**, permettant le routage inter-VLAN à l'aide d'un routeur connecté à un switch de distribution via un lien trunk IEEE 802.1Q.

L'infrastructure comprend plusieurs VLAN utilisateurs, un VLAN de management, un serveur DHCP intégré au routeur et des switches d'accès connectés à un switch de distribution.

---

## Topologie

> Ajouter ici votre schéma dans le dossier `topology/`.

```text
R1
 │
 │ Trunk 802.1Q
 │
SW-DISTRIB
├── SW-ACCESS-1 (VLAN 10)
├── SW-ACCESS-2 (VLAN 20)
└── SW-ACCESS-3 (VLAN 30)
```

---

## VLAN

| VLAN | Nom | Réseau | Passerelle |
|------|------|----------------|----------------|
|10|USERS|192.168.10.0/24|192.168.10.254|
|20|SERVERS|192.168.20.0/24|192.168.20.254|
|30|LINUX|192.168.30.0/24|192.168.30.254|
|99|MANAGEMENT|192.168.99.0/24|192.168.99.254|

---

## Fonctionnalités

- Router-on-a-Stick
- IEEE 802.1Q
- VLAN
- Trunk
- DHCP
- Routage Inter-VLAN
- VLAN de Management
- Cisco IOS
- Linux
- Windows

---

## Structure du projet

```
configs/
docs/
hosts/
images/
topology/
```

---

## Vérification

```
show vlan brief
show interfaces trunk
show ip interface brief
show ip route
show ip dhcp binding
```

---

## Auteur

Projet réalisé dans le cadre d'un laboratoire Cisco.
