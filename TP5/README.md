# TP n° 5 : Intégration dans les réseaux sous Linux (RHEL 9)

**École :** École Marocaine des Sciences de l'Ingénieur (EMSI)  
**Filière :** 4IIR — Administration Unix  
**Encadrante :** Mr. Noreddine Abghour  
**Étudiant :** Badr  
**Système :** Red Hat Enterprise Linux 9.8 (`x86_64`) — Interface réseau `ens192`  

---

## Objectifs du TP n° 5

- Explorer les commandes permettant de configurer et gérer les interfaces réseau sous Linux.
- Manipuler et analyser la commande classique **`ip`** (`iproute2` : `ip a`, `ip link`, `ip route`).
- Mettre en pratique les outils modernes de **NetworkManager** (**`nmcli`** et **`nmtui`**), y compris la gestion multi-profils sur une même carte réseau.
- Explorer les fichiers système de configuration réseau et de résolution de noms (`/etc/resolv.conf`, `/etc/NetworkManager/system-connections/`, `/etc/hostname`, `/etc/hosts`).

---

## Structure du dossier `T5`

Ce répertoire regroupe l'ensemble des comptes rendus (PDF et Markdown GitHub) et captures d'écran du **TP n° 5** répartis en trois ateliers :

| Atelier | Thème | Compte rendu GitHub | Compte rendu PDF | Captures |
| :--- | :--- | :--- | :--- | :--- |
| 📁 **Atelier 1** | Exploration de la commande classique `ip a` | [`Atelier1/README.md`](./Atelier1/README.md) | [`Compte_Rendu_TP5_Atelier1_ip.pdf`](./Atelier1/Compte_Rendu_TP5_Atelier1_ip.pdf) | 7 captures (`Atelier1/screenshots/`) |
| 📁 **Atelier 2** | Exploration de `nmcli` (multi-profils) et `nmtui` | [`Atelier2/README.md`](./Atelier2/README.md) | [`Compte_Rendu_TP5_Atelier2_nmcli_nmtui.pdf`](./Atelier2/Compte_Rendu_TP5_Atelier2_nmcli_nmtui.pdf) | 13 captures (`Atelier2/screenshots/`) |
| 📁 **Atelier 3** | Fichiers de configuration réseau, `hostname` et `/etc/hosts` | [`Atelier3/README.md`](./Atelier3/README.md) | [`Compte_Rendu_TP5_Atelier3_Config_Reseau.pdf`](./Atelier3/Compte_Rendu_TP5_Atelier3_Config_Reseau.pdf) | 6 captures (`Atelier3/screenshots/`) |

---

## Synthèse des compétences validées

1. **Configuration temporaire (`iproute2`) :** identification de `ens192`, bascule `UP`/`DOWN`, ajout/suppression d'une IPv4 temporaire (`192.168.1.200/24`) et manipulation de la table de routage.
2. **Administration persistante (`NetworkManager`) :** gestion des périphériques (`device`) et des connexions (`connection`), bascule statique/DHCP, suppression des adresses IP en doublon, création et activation de deux profils distincts (`ens192-static` et `ens192-dhcp`), exploration de `nmtui`.
3. **Fichiers système et résolution de noms :** inspection des serveurs DNS (`/etc/resolv.conf`) et des keyfiles `.nmconnection`, changement temporaire (`rhel9-temp`) puis permanent (`rhel9-badr`) du nom d'hôte avec `hostnamectl`, et résolution statique locale dans `/etc/hosts` (`serveur-test.local`).
