# ShadowFortress
📛 ShadowFortress - A Blocklist Aggregator

![Open Source](https://img.shields.io/badge/open%20source-100%25-success)
![Python](https://img.shields.io/badge/python-3.10%2B-blue)
![Threat Intel](https://img.shields.io/badge/threat%20intel-multi--source-critical)
![Blocklist](https://img.shields.io/badge/blocklist-IPv4-important)
![SIEM](https://img.shields.io/badge/SIEM-Wazuh-purple)
![Update](https://img.shields.io/badge/update-every%206h-informational)
![False Positives](https://img.shields.io/badge/false%20positives-reduced-success)

Licence : 

![License](https://img.shields.io/badge/license-GNU%20GPLv3-blue)

[Français]
📌 Description

Ce projet est un agrégateur de blocklists IP.
Il consolide plusieurs sources publiques de blocklists afin d’identifier les adresses IP les plus redondantes, c’est-à-dire celles apparaissant dans de nombreuses listes de blocage.

L’objectif est de fournir une blocklist optimisée, limitée à un maximum de 100 000 adresses IP, représentant les menaces les plus couramment observées.

⚙️ Fonctionnement

Agrégation de multiples blocklists publiques

Déduplication des adresses IP

Sélection des IP les plus fréquemment listées

Exclusion automatique d’une whitelist privée (non publique)

Génération de fichiers prêts à l’emploi

⏱ Actualisation automatique toutes les 6 heures

📂 Fichiers générés
Fichier	Description
blacklist_inbound.txt	Blocklist destinée au filtrage entrant
blacklist_outbound.txt	Blocklist destinée au filtrage sortant
STATS.md	Récapitulatif statistique (volumes, évolution, sources, etc.)
🛠️ Installation & intégration

Aucune installation n’est requise.

L’intégration dépend entièrement de l’environnement de l’utilisateur.
Les fichiers peuvent être exploités selon les procédures du constructeur ou de la solution utilisée, par exemple :

iptables / nftables

Firewalls Fortinet

Équipements Cisco

Firewalls ZyXEL

Toute autre solution réseau ou sécurité compatible avec des listes IP

🔐 Whitelist privée

Une whitelist privée est appliquée en amont du processus.
Les adresses IP qu’elle contient sont exclues systématiquement des blocklists générées.

La whitelist n’est pas publique et ne fait pas partie du dépôt.

📜 Licence

Ce projet est distribué sous licence GNU General Public License v3 (GPLv3).
Vous êtes libre de l’utiliser, le modifier et le redistribuer conformément aux termes de cette licence.

[English]
📌 Description

This project is an IP blocklist aggregator.
It consolidates multiple public blocklist sources to identify the most redundant IP addresses, meaning those appearing across many different blocklists.

The goal is to provide an optimized blocklist, capped at 100,000 IP addresses, focusing on the most commonly reported threats.

⚙️ How it works

Aggregation of multiple public blocklists

IP deduplication

Selection of the most frequently listed IPs

Automatic exclusion of a private whitelist

Generation of ready-to-use files

⏱ Automatic updates every 6 hours

📂 Generated files
File	Description
blacklist_inbound.txt	Blocklist intended for inbound filtering
blacklist_outbound.txt	Blocklist intended for outbound filtering
STATS.md	Statistical summary (volume, trends, sources, etc.)
🛠️ Installation & integration

No installation is required.

Integration depends entirely on the user’s environment.
The files can be consumed according to vendor or platform-specific procedures, such as:

iptables / nftables

Fortinet firewalls

Cisco devices

ZyXEL firewalls

Any other network or security solution supporting IP blocklists

🔐 Private whitelist

A private whitelist is applied upstream in the process.
Any IP address listed in it is systematically excluded from the generated blocklists.

The whitelist is not public and is not included in the repository.

📜 License

This project is licensed under the GNU General Public License v3 (GPLv3).
You are free to use, modify, and redistribute it in accordance with the terms of this license.


## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)

