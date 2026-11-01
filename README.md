# Travaux Pratiques — Administration Unix (RHEL 9)

**École :** École Marocaine des Sciences de l'Ingénieur (EMSI)  
**Filière :** 4IIR (4e année Ingénierie Informatique et Réseaux)  
**Encadrante :** Mme. Berraho Sanae  
**Réalisé par :** Badr  
**Année universitaire :** 2026/2027  
**Environnement technique :** Red Hat Enterprise Linux 9 (RHEL 9)

## À propos de ce dépôt

Ce dépôt regroupe l'ensemble des comptes rendus détaillés, configurations, commandes et captures d'écran réalisés dans le cadre du cours d'**Administration Unix**. Chaque dossier correspond à un travail pratique (TP) complet avec ses explications techniques et ses preuves d'exécution sur machine virtuelle RHEL 9.

## Sommaire des Travaux Pratiques

| TP | Sujet du TP | Principaux concepts abordés | Dossier |
| :--- | :--- | :--- | :--- |
| **TP n°2** | **Configuration des paramètres du Boot Loader GRUB2** | Séquence de démarrage (BIOS/UEFI), `/boot` & BLS, `/etc/default/grub`, `/etc/grub.d/40_custom`, `grub2-mkconfig`, réinitialisation du mot de passe `root` (`rd.break` & SELinux `/.autorelabel`), sécurisation par mot de passe (`grub2-setpassword`) | [📂 TP2-GRUB2-RHEL9](https://www.google.com/search?q=./TP2-GRUB2-RHEL9/) |
| **TP n°3** | *Prochain TP* | *(À compléter au fil des séances)* | `./TP3-...` *(à venir)* |

## Organisation du dépôt

```text
.
├── README.md                  # Présentation générale du dépôt et sommaire des TP
└── TP2-GRUB2-RHEL9/           # Dossier du TP n°2 (GRUB2)
    ├── README.md              # Compte rendu complet du TP n°2
    └── screenshots/           # Captures d'écran des manipulations sous RHEL 9
```

## Prérequis et environnement

- **Hyperviseur :** VMware Workstation / VirtualBox
- **Système d'exploitation :** Red Hat Enterprise Linux 9.8 (`kernel 5.14.0-687.61.1.el9_8.x86_64`)
- **Privilèges :** Accès administrateur (`root` / `sudo`)
