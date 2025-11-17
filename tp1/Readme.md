# Playbook Ansible – Installation d'Apache2 sur Ubuntu

Ce projet contient un playbook Ansible permettant d’installer, activer et vérifier le service **Apache2** sur un serveur.

---

## 📦 Contenu du dépôt

- **apache.yml**  
  Playbook Ansible effectuant :
  - mise à jour du cache `apt`
  - installation d’Apache2

- **hosts.ini** (exemple d’inventaire)

---

## 🖥️ Prérequis

- Ansible installé sur la machine de contrôle  
- Accès SSH vers les hôtes distants  
- Ubuntu (20.04, 22.04, 24.04…) sur les machines cibles  
- L’utilisateur distant doit pouvoir devenir root (`become: yes`)

---

## 🗂️ Exemple d’inventaire (`hosts.ini`)

```ini
[web]
192.168.1.20 

