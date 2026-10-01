\# Architecture réseau segmentée IT/OT — HydroRégie



\## 1. Objectif



L'objectif est de séparer l'environnement informatique de gestion (IT) de

l'environnement industriel (OT), afin d'empêcher qu'un incident affectant le

réseau administratif puisse se propager directement vers les systèmes de

production et de distribution d'eau potable.



L'architecture proposée repose sur des zones distinctes, une DMZ industrielle,

des pare-feu et un contrôle renforcé des accès distants.



\## 2. Schéma d'architecture cible



```mermaid

flowchart LR

&#x20;   Internet\[Internet]

&#x20;   VPN\[VPN avec MFA]

&#x20;   IT\[Zone IT<br/>Postes administratifs<br/>Messagerie et applications de gestion]

&#x20;   FW1\[Pare-feu IT / DMZ]

&#x20;   DMZ\[DMZ industrielle<br/>Bastion / Jump server<br/>Serveur de transfert sécurisé<br/>Journalisation]

&#x20;   FW2\[Pare-feu DMZ / OT]

&#x20;   OT\[Zone OT<br/>Supervision SCADA<br/>Serveurs industriels]

&#x20;   FIELD\[Zone terrain<br/>Automates, capteurs, pompes et vannes]



&#x20;   Internet --> VPN

&#x20;   VPN --> IT

&#x20;   IT --> FW1

&#x20;   FW1 --> DMZ

&#x20;   DMZ --> FW2

&#x20;   FW2 --> OT

&#x20;   OT --> FIELD

```



\## 3. Description des zones



| Zone | Rôle | Niveau de criticité |

|---|---|---|

| Internet et accès distant | Accès des utilisateurs et des prestataires autorisés | Élevé |

| Zone IT | Postes administratifs, messagerie, applications de gestion et serveurs bureautiques | Élevé |

| DMZ industrielle | Zone tampon contrôlée pour les échanges entre IT et OT ; héberge le bastion, les services de transfert et la journalisation | Très élevé |

| Zone OT | Systèmes de supervision et serveurs nécessaires au pilotage industriel | Critique |

| Zone terrain | Automates, capteurs, pompes, vannes et équipements physiques | Critique |



\## 4. Principes de sécurité



\- Aucun accès direct entre la zone IT et la zone OT n'est autorisé.

\- Les échanges IT/OT transitent obligatoirement par la DMZ industrielle.

\- Les pare-feu appliquent le principe « tout interdire par défaut, n'autoriser

&#x20; que les flux nécessaires ».

\- Les accès d'administration et de maintenance passent par un VPN avec MFA,

&#x20; puis par un bastion situé dans la DMZ.

\- Les droits d'accès sont attribués selon le principe du moindre privilège et

&#x20; les actions d'administration sont journalisées.

\- Les équipements OT critiques sont isolés dans des VLAN dédiés afin de limiter

&#x20; les mouvements latéraux.

\- Les journaux des pare-feu, du VPN et du bastion sont centralisés pour faciliter

&#x20; la détection et l'investigation d'incidents.



\## 5. Continuité du service d'eau potable



La segmentation ne doit pas empêcher le fonctionnement local des installations

industrielles. En cas d'incident sur le réseau IT ou de coupure des échanges

avec la DMZ, les systèmes OT doivent pouvoir maintenir un fonctionnement

dégradé et sûr, selon des consignes locales validées par les équipes

d'exploitation.



Les sauvegardes des configurations critiques, des données de supervision et des

procédures de reprise doivent être testées régulièrement. Toute intervention

sur l'environnement OT doit être planifiée, validée et réversible afin de ne

pas affecter la disponibilité de la production et de la distribution d'eau.



\## 6. Justification



Cette architecture réduit le risque de propagation d'un ransomware ou d'un

accès non autorisé depuis le système d'information administratif vers les

systèmes industriels. La DMZ, les pare-feu, le MFA, le bastion et la

journalisation permettent de contrôler les flux, les identités et les actions

sensibles, tout en préservant les besoins légitimes d'exploitation et de

maintenance.

