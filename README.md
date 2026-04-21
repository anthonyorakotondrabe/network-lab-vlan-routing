# 🖧 Network Lab - VLAN & Inter-VLAN Routing

##  Objectif

Ce projet simule une infrastructure réseau simple avec segmentation VLAN et routage inter-VLAN.
Il permet de comprendre comment isoler les réseaux et permettre la communication entre eux.

---

##  Technologies utilisées

* Cisco Packet Tracer
* VLAN (Virtual LAN)
* Router-on-a-stick
* IPv4 addressing

---

##  Topologie du réseau

Le lab contient :

* 1 Routeur
* 1 Switch
* 2 VLAN :

  * VLAN 10 → 192.168.10.0/24
  * VLAN 20 → 192.168.20.0/24
* 2 PCs
* 2 Laplops

---

##  Configuration

### 🔹 Switch

* Création des VLANs 10 et 20
* Attribution des ports aux VLANs
* Configuration du trunk vers le routeur

### 🔹 Routeur

* Configuration des sous-interfaces :

  * G0/0.10 → VLAN 10
  * G0/0.20 → VLAN 20
* Encapsulation dot1Q
* Attribution des adresses IP

---

##  Plan d’adressage

| Appareil       | IP           |
| -------------- | ------------ |
| PC1            | 192.168.10.2 |
| PC2            | 192.168.20.2 |
| Routeur VLAN10 | 192.168.10.1 |
| Routeur VLAN20 | 192.168.20.1 |

---

## Tests

* Ping entre PC1 et PC2 
* Communication inter-VLAN fonctionnelle 

---

##  Captures d’écran

Les captures sont disponibles dans le dossier `/screenshots` :

* Topologie réseau
* Résultat des tests (ping)

---

##  Structure du projet

* `/topology` → fichier Packet Tracer
* `/configs` → configurations switch et routeur
* `/screenshots` → images du projet

---


##  Auteur

RAKOTONDRABE Tokiniaina Anthonyo Sarobidy
Étudiant en Informatique
