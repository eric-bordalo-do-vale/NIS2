\# Analyse d'écart et feuille de route — HydroRégie



\## 1. Objectif et périmètre



Cette analyse d'écart évalue le niveau de préparation d'HydroRégie au regard

des mesures de gestion des risques prévues par l'article 21 de la directive

NIS2.



Elle couvre les systèmes d'information de gestion (IT), les systèmes

industriels (OT), les accès distants, les actifs critiques et les prestataires

participant à la fourniture d'eau potable.



\## 2. Analyse d'écart



| Domaine NIS2 | Situation constatée ou à vérifier | Écart / risque | Priorité | Action recommandée |

|---|---|---|---|---|

| Analyse des risques et politique de sécurité | À vérifier | Absence possible de cartographie des actifs et des risques IT/OT | Haute | Réaliser une analyse de risques et formaliser une politique de sécurité |

| Gestion des incidents | À vérifier | Détection, escalade et traçabilité des incidents potentiellement insuffisantes | Haute | Définir une procédure de gestion des incidents et une cellule de crise |

| Continuité d'activité et sauvegardes | À vérifier | Risque d'interruption prolongée du service ou de perte de données | Haute | Tester les sauvegardes et définir un plan de continuité et de reprise |

| Segmentation IT/OT | IT et OT non cloisonnés | Propagation possible d'un incident IT vers les systèmes industriels | Critique | Mettre en place des zones IT, DMZ industrielle et OT avec des pare-feu |

| Sécurité des fournisseurs | À vérifier | Accès ou dépendance aux prestataires insuffisamment maîtrisés | Moyenne | Recenser les prestataires et encadrer leurs accès par contrat et MFA |

| Gestion des accès et des actifs | À vérifier | Comptes trop privilégiés ou actifs non inventoriés | Haute | Appliquer le moindre privilège, inventorier les actifs et revoir les comptes |

| Cyberhygiène et formation | À vérifier | Risque de phishing, mots de passe faibles ou erreurs humaines | Moyenne | Former les salariés et organiser des campagnes de sensibilisation |

| MFA et communications sécurisées | À vérifier | Risque de compromission des accès distants ou administrateurs | Haute | Imposer le MFA pour VPN, administration et comptes à privilèges |



\## 3. Priorisation



La segmentation entre les environnements IT et OT constitue l'écart prioritaire,

car elle est explicitement identifiée dans le scénario et peut permettre la

propagation d'un incident vers les systèmes industriels.



Les actions relatives à la continuité d'activité, à la gestion des incidents,

aux accès privilégiés et aux sauvegardes sont également prioritaires. Elles

contribuent directement au maintien du service d'eau potable en cas de crise.



\## 4. Feuille de route



| Échéance | Actions principales | Responsable |

|---|---|---|

| 0 à 30 jours | Nommer un responsable du projet NIS2, inventorier les actifs critiques, lancer l'analyse de risques IT/OT et formaliser la procédure d'escalade des incidents | Direction générale, RSSI, DSI, responsable OT |

| 1 à 3 mois | Déployer le MFA pour les accès sensibles, revoir les comptes à privilèges, tester les sauvegardes, élaborer le plan de continuité et encadrer les accès prestataires | RSSI, DSI, responsable OT |

| 3 à 6 mois | Mettre en œuvre la segmentation IT/OT, créer une DMZ industrielle, appliquer des règles de filtrage, centraliser les journaux et réaliser un exercice de crise | DSI, responsable OT, intégrateur réseau |

| En continu | Former les salariés, suivre les vulnérabilités, réévaluer les risques et contrôler l'efficacité des mesures | RSSI, RH, direction |



\## 5. Conclusion



HydroRégie doit traiter en priorité le manque de cloisonnement entre IT et OT.

La feuille de route proposée permet de réduire progressivement les risques,

d'améliorer la résilience du service d'eau potable et de structurer la mise en

conformité avec les exigences de la directive NIS2.

