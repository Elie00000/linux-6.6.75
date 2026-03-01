# linux-6.6.75.deb — Kernel Exploit (Vagrant Box)

Ce dépôt contient une box Vagrant personnalisée permettant de reproduire un environnement vulnérable basé sur le kernel `linux-6.6.75.deb`.  
L'objectif est de faciliter l’analyse, la démonstration, ou la mise en place d’un proof-of-concept exploit.

---

## 🚀 Contenu du projet

La box Vagrant est construite à partir des fichiers suivants :

- `metadata.json` — Métadonnées Vagrant
- `box.img` — Image disque
- `bzImage` — Image du kernel
- `ramdisk_v1.img` — Initramfs modifié
- `Vagrantfile` — Configuration Vagrant

L’ensemble est empaqueté dans une archive `.box`.

---

## 📦 Création de la box

Exécuter la commande suivante pour générer l’archive finale :

```bash
tar cvzf mitigation-v3-full.box \
  metadata.json \
  box.img \
  bzImage \
  ramdisk_v1.img \
  Vagrantfile
``

```bash
rm mitigation-v3-full.box
