\# Gestion de crise et notifications réglementaires — HydroRégie



\## 1. Scénario d'incident



Le scénario retenu est une attaque par ransomware détectée sur un poste de

travail administratif. Des tentatives de connexion inhabituelles vers des

ressources industrielles sont également observées.



Compte tenu de l'absence actuelle de cloisonnement entre IT et OT, cet incident

est considéré comme significatif : il présente un risque de propagation vers

les systèmes de supervision et pourrait affecter la continuité de la

production et de la distribution d'eau potable.



\## 2. Organisation de crise



| Rôle | Responsabilités |

|---|---|

| Direction générale | Décide des orientations majeures, valide la communication externe et mobilise les ressources nécessaires |

| RSSI | Coordonne la réponse cyber, qualifie l'incident et pilote l'investigation |

| DSI | Isole les systèmes IT affectés, restaure les services et coordonne les équipes techniques |

| Responsable OT | Vérifie l'intégrité des systèmes industriels et garantit la sécurité du processus de production |

| Communication | Prépare les messages destinés aux salariés, usagers et partenaires |

| Juridique / DPO | Évalue les obligations réglementaires complémentaires, notamment en cas de données personnelles concernées |



\## 3. Chronologie de gestion de crise



| Délai | Actions |

|---|---|

| H0 — Détection | Un poste administratif signale une activité anormale ; le SOC ou la DSI ouvre un ticket d'incident et conserve les journaux disponibles |

| H0 à H+4 | Le RSSI qualifie l'incident, mobilise la cellule de crise, isole le poste compromis et suspend les accès distants non indispensables |

| H+4 à H+24 | La DSI recherche les indicateurs de compromission, contrôle les comptes à privilèges et applique des règles temporaires de filtrage entre IT et OT ; le responsable OT vérifie l'absence d'impact sur la supervision et les automates |

| Avant H+24 | HydroRégie transmet une alerte précoce à l'autorité compétente |

| H+24 à H+72 | Les équipes poursuivent l'investigation, restaurent les systèmes à partir de sauvegardes vérifiées, renforcent les accès et évaluent l'impact opérationnel |

| Avant H+72 | HydroRégie transmet une notification d'incident détaillée à l'autorité compétente |

| Après H+72 | Retour progressif à la normale, surveillance renforcée, analyse de la cause racine et retour d'expérience |

| Au plus tard un mois après la notification | HydroRégie transmet un rapport final ou, si l'incident est toujours en cours, un rapport d'avancement |



\## 4. Alerte précoce — 24 heures



\*\*Destinataire :\*\* Autorité nationale compétente / CSIRT compétent

\*\*Objet :\*\* Alerte précoce NIS2 — Incident cyber significatif — HydroRégie



HydroRégie, entité essentielle du secteur de l'eau potable, informe avoir pris

connaissance le \[date et heure] d'un incident de cybersécurité affectant un

poste de travail de son environnement IT.



L'incident présente des caractéristiques compatibles avec une attaque par

ransomware. Des tentatives de connexion inhabituelles vers des ressources

industrielles ont été détectées. À ce stade, aucun impact sur la production ou

la distribution d'eau potable n'est confirmé.



Les premières mesures de confinement ont été engagées : isolement du poste

concerné, suspension préventive des accès distants non indispensables et

vérification de l'environnement OT. L'investigation est en cours. Aucun impact

transfrontière n'est identifié à ce stade.



\## 5. Notification d'incident — 72 heures



\*\*Destinataire :\*\* Autorité nationale compétente / CSIRT compétent

\*\*Objet :\*\* Notification NIS2 — Incident cyber significatif — HydroRégie



Le \[date et heure], HydroRégie a détecté un incident de cybersécurité sur son

environnement IT, présentant des caractéristiques compatibles avec une attaque

par ransomware. L'incident a été qualifié de significatif en raison du risque

de propagation vers l'environnement OT et de son impact potentiel sur un

service essentiel de fourniture d'eau potable.



Les investigations menées à ce stade indiquent que \[nombre] postes de travail

ont été affectés. Aucun système OT, automate ou système de supervision n'est

confirmé comme compromis à ce stade. Les indicateurs de compromission connus,

les comptes concernés et les journaux pertinents sont en cours d'analyse.



Les mesures prises comprennent l'isolement des systèmes affectés, la

réinitialisation des comptes sensibles, le renforcement du filtrage IT/OT, la

suspension des accès distants non indispensables et la restauration des

services à partir de sauvegardes vérifiées. La continuité de distribution d'eau

potable est maintenue.



\## 6. Rapport final — un mois



\*\*Destinataire :\*\* Autorité nationale compétente / CSIRT compétent

\*\*Objet :\*\* Rapport final NIS2 — Incident cyber significatif — HydroRégie



L'incident détecté le \[date] a affecté l'environnement IT d'HydroRégie. Son

origine probable est \[à compléter après investigation]. L'analyse n'a pas mis

en évidence de compromission des systèmes OT ni d'interruption de la

distribution d'eau potable.



Les actions de remédiation ont inclus l'isolement des équipements touchés, la

restauration depuis des sauvegardes vérifiées, la réinitialisation des comptes,

le renforcement des règles de filtrage et la mise en place d'une surveillance

renforcée.



Le retour d'expérience a confirmé la nécessité d'accélérer la segmentation

IT/OT, de généraliser le MFA pour les accès sensibles, de tester régulièrement

les sauvegardes et d'organiser des exercices de gestion de crise. Ces actions

sont intégrées à la feuille de route de mise en conformité NIS2.

