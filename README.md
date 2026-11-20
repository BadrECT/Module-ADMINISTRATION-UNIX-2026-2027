# Travaux Pratiques — Administration Unix (RHEL 9)

**École :** École Marocaine des Sciences de l'Ingénieur (EMSI)  
**Filière :** 4IIR (4e année Ingénierie Informatique et Réseaux)  
**Encadrant :** Mr. Noreddine Abghour  
**Réalisé par :** Badr Kaanoune  
**Année universitaire :** 2026/2027  
**Environnement technique :** Red Hat Enterprise Linux 9 (RHEL 9)

## À propos de ce dépôt

Ce dépôt regroupe l'ensemble des comptes rendus détaillés, configurations, commandes et captures d'écran réalisés dans le cadre du cours d'**Administration Unix**. Chaque dossier correspond à un travail pratique (TP) complet avec ses explications techniques et ses preuves d'exécution sur machine virtuelle RHEL 9.

## Sommaire des Travaux Pratiques

| TP | Sujet du TP | Principaux concepts abordés | Dossier |
| :--- | :--- | :--- | :--- |
| **TP n°2** | **Configuration des paramètres du Boot Loader GRUB2** | Séquence de démarrage (BIOS/UEFI), `/boot` & BLS, `/etc/default/grub`, `/etc/grub.d/40_custom`, `grub2-mkconfig`, réinitialisation du mot de passe `root` (`rd.break` & SELinux `/.autorelabel`), sécurisation par mot de passe (`grub2-setpassword`) | [📂 TP2-GRUB2-RHEL9](./TP2-GRUB2-RHEL9/) |
| **TP n°3** | **Configuration des cibles et gestion des services par Systemd** | Architecture Systemd & PID 1, analyse des temps d'amorçage (`systemd-analyze blame / critical-chain`), administration des cibles (`graphical.target` vs `multi-user.target`, `isolate`), gestion des services (`systemctl` start, stop, restart, reload, enable, disable, mask, kill) et journalisation binaire avancée (`journalctl`) | [📂 TP3-Systemd-RHEL9](./TP3/) |
| **TP n°4** | **Gestion des paquetages sous Linux et création d'un dépôt local** | Gestionnaire bas niveau `rpm` (`-qa`, `-qi`, `-ql`, `-qf`, `-V`, `-K`, `--nodeps`), gestionnaire haut niveau `yum`/`dnf` (`install`, `upgrade`, `history undo`, `provides`, `group`, `config-manager`), création et configuration d'un dépôt local (`httpd`, `createrepo_c`, `/etc/yum.repos.d/mon_depot.repo`) | [📂 TP4-Paquetages-RHEL9](./TP4/) |

## Organisation du dépôt

```text
.
├── README.md                              # Présentation générale du dépôt et sommaire des TP
├── TP2-GRUB2-RHEL9/                       # Dossier du TP n°2 (GRUB2)
│   ├── README.md                          # Compte rendu complet du TP n°2
│   └── screenshots/                       # Captures d'écran des manipulations sous RHEL 9
├── TP3/                                   # Dossier du TP n°3 (Systemd & Journalctl)
│   ├── README.md                          # Compte rendu complet illustré du TP n°3
│   ├── Compte_Rendu_TP3_Systemd.pdf       # Version finale imprimable du rapport PDF
│   ├── Compte_Rendu_TP3_Systemd.docx      # Version éditable Word du compte rendu
│   ├── Enonce_TP3_Systemd.pdf             # Sujet officiel du TP
│   └── screenshots/                       # 26 captures d'écran classées par atelier
└── TP4/                                   # Dossier du TP n°4 (Gestion des paquetages RPM, DNF & Dépôt local)
    ├── README.md                          # Présentation générale du TP n°4 et sommaire des ateliers
    ├── atelier1/                          # Atelier 1 : Gestion de paquetages avec rpm
    │   ├── README.md                      # Compte rendu complet illustré (13 questions)
    │   ├── Compte_Rendu_TP4_Atelier1_RPM.pdf
    │   ├── Compte_Rendu_TP4_Atelier1_RPM.docx
    │   └── screenshots/                   # 18 captures d'écran
    ├── atelier2/                          # Atelier 2 : Gestion de paquetages avec yum / dnf
    │   ├── README.md                      # Compte rendu complet illustré (17 questions)
    │   ├── Compte_Rendu_TP4_Atelier2_DNF.pdf
    │   ├── Compte_Rendu_TP4_Atelier2_DNF.docx
    │   └── screenshots/                   # 27 captures d'écran
    └── atelier3/                          # Atelier 3 : Création d'un dépôt de logiciels local
        ├── README.md                      # Compte rendu complet illustré (7 étapes)
        ├── Compte_Rendu_TP4_Atelier3_Depot_Local.pdf
        ├── Compte_Rendu_TP4_Atelier3_Depot_Local.docx
        └── screenshots/                   # 14 captures d'écran
