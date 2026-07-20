# Router-on-a-Stick

## Principe

Le Router-on-a-Stick permet à un routeur de réaliser le routage entre plusieurs VLAN grâce à une unique interface physique configurée en sous-interfaces.

Chaque sous-interface est associée à un VLAN via l'encapsulation IEEE 802.1Q.

## Sous-interfaces

| Interface | VLAN |
|-----------|------|
|e0/0.10|10|
|e0/0.20|20|
|e0/0.30|30|
|e0/0.99|99|

## VLAN natif

Le VLAN 99 est utilisé comme VLAN natif et VLAN de management.

## Avantages

- Économie d'interfaces physiques.
- Routage inter-VLAN centralisé.
- Configuration simple pour les environnements de laboratoire.
