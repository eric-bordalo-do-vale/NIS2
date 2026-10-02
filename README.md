# Mise en conformité NIS2 — Cas HydroRégie



## Présentation du projet



Ce dépôt présente une proposition de mise en conformité à la directive

européenne NIS2 pour HydroRégie, une régie des eaux desservant environ

450 000 habitants.



HydroRégie est qualifiée d'entité essentielle. Le scénario identifie un risque

majeur : les environnements informatiques de gestion (IT) et industriels (OT)

ne sont pas suffisamment cloisonnés. Un incident cyber affectant le système

d'information administratif pourrait donc se propager vers les systèmes

industriels nécessaires à la production et à la distribution d'eau potable.



## Objectifs



\- Qualifier HydroRégie au regard de la directive NIS2.

\- Identifier les principaux écarts de cybersécurité.

\- Proposer une feuille de route de mise en conformité.

\- Concevoir une architecture réseau segmentée entre IT et OT.

\- Définir une organisation de gestion de crise et les notifications

&#x20; réglementaires associées.



\
## Livrables



| Fichier | Contenu |

| --- | --- |

| \[01-qualification-nis2.md](01-qualification-nis2.md) | Qualification réglementaire d'HydroRégie comme entité essentielle |

| \[02-analyse-ecart-feuille-route.md](02-analyse-ecart-feuille-route.md) | Analyse d'écart au regard de l'article 21 et feuille de route |

| \[03-architecture-it-ot.md](03-architecture-it-ot.md) | Architecture réseau segmentée IT/OT avec DMZ industrielle |

| \[04-gestion-crise-notifications.md](04-gestion-crise-notifications.md) | Gestion de crise cyber et modèles de notifications réglementaires |



## Principaux constats



\- HydroRégie relève du secteur de l'eau potable et est une entité essentielle.

\- L'absence de cloisonnement IT/OT représente le risque prioritaire identifié.

\- La segmentation réseau, la DMZ industrielle, les pare-feu et le MFA réduisent

&#x20; le risque de propagation vers les systèmes industriels.

\- La continuité de la production et de la distribution d'eau potable est la

&#x20; priorité opérationnelle en cas d'incident.

\- Les incidents significatifs doivent faire l'objet d'une alerte précoce sous

&#x20; 24 heures, d'une notification sous 72 heures et d'un rapport final dans un

&#x20; délai d'un mois.



## Limites de l'étude



Cette étude repose sur les informations fournies par le cas pratique. Les

caractéristiques détaillées de l'architecture existante, des sauvegardes, des

outils de sécurité, des accès distants et des prestataires ne sont pas connues.



Les recommandations formulées constituent donc une proposition de travail.

Elles devraient être confirmées par un audit technique, documentaire et

organisationnel avant toute mise en œuvre opérationnelle.



## Références



* [Directive (UE) 2022/2555 — NIS2](https://eur-lex.europa.eu/eli/dir/2022/2555/oj?locale=fr)
* [ANSSI — Directive NIS 2](https://cyber.sites.beta.gouv.fr/reglementation/cybersecurite-systemes-dinformation/directives-nis-nis2-et-dispositif-saiv/directive-nis-2/)
* [MonEspaceNIS2](https://monespacenis2.cyber.gouv.fr/)
* [ENISA — NIS2](https://www.enisa.europa.eu/topics/awareness-and-cyber-hygiene/raising-awareness-campaigns/network-and-information-systems-directive-2-nis2)
* [Énoncé du cas pratique HydroRégie](pdf/NIS2.pdf)
---

