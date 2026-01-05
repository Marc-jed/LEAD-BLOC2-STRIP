# Projet Stripe – Architecture de données (OLTP / OLAP / NoSQL)

## Présentation générale

Ce dépôt GitHub présente un projet d’architecture de données réalisé dans le cadre du **Bloc 2 – Concevoir et déployer des architectures de données (IA)**.

Le projet s’appuie sur une **étude de cas Stripe** et a pour objectif de concevoir une architecture de données complète intégrant :

* un système transactionnel (OLTP),
* un système analytique (OLAP),
* une base NoSQL,
* des pipelines de données,
* des mécanismes de sécurité et de conformité,
* une intégration simple de modèles de machine learning.

Le projet se concentre sur la **conception et la compréhension des architectures**, et non sur un déploiement industriel réel.

---

## Objectifs du projet

Les objectifs principaux sont :

* concevoir une architecture de données cohérente et évolutive,
* séparer les usages transactionnels, analytiques et machine learning,
* modéliser des schémas OLTP, OLAP et NoSQL adaptés aux besoins métier,
* illustrer l’utilisation des données via des requêtes SQL et NoSQL,
* intégrer les notions de sécurité, conformité et gouvernance des données.

---

## Contenu du dépôt

Le dépôt est organisé autour des livrables demandés dans le cadre du projet.

### 1. Architecture globale

* Diagramme d’architecture du pipeline de données
* Document décrivant les flux entre OLTP, OLAP, NoSQL et machine learning

---

### 2. Modèle OLTP

* Diagramme entité-relation (ERD) du système transactionnel
* Annexe décrivant les relations métier autour de l’entité TRANSACTION

---

### 3. Modèle OLAP

* Schéma analytique (schéma en flocon)
* Document d’accompagnement expliquant :

  * le grain de la table de faits,
  * les jointures,
  * les pré-agrégations,
  * l’optimisation des performances

---

### 4. Modèle NoSQL

* Schéma des collections NoSQL
* Document décrivant :

  * les types de données stockées,
  * la gestion des relations logiques,
  * la stratégie d’indexation,
  * l’intégration avec OLTP et OLAP

---

### 5. Sécurité et conformité

* Plan de sécurité et de conformité
* Mesures liées au chiffrement, aux accès, à la conformité réglementaire (RGPD, PCI-DSS, CCPA)
* Notions de surveillance et de gestion des incidents

---

### 6. Intégration du machine learning

* Document décrivant l’intégration d’un modèle de détection de fraude
* Extraction des données, entraînement, déploiement et surveillance du modèle
* Intégration du scoring dans le système NoSQL

---

### 7. Requêtes SQL et NoSQL

* Notebook contenant des exemples de requêtes SQL (OLAP)
* Exemples de requêtes NoSQL (MongoDB)
* Requêtes illustrant des cas d’usage métier :

  * analyse des revenus,
  * détection de fraude,
  * segmentation client

---

## Technologies utilisées

Les technologies mentionnées dans ce projet sont utilisées à titre illustratif :

* PostgreSQL (OLTP)
* Apache Kafka et Debezium (streaming et CDC)
* Apache Airflow (orchestration)
* Apache Spark (traitement des données)
* Snowflake (OLAP)
* MongoDB (NoSQL)
* MLflow (cycle de vie des modèles ML)
* Tableau / Power BI (visualisation)

---

## Conclusion

Ce dépôt présente une architecture de données complète et cohérente répondant aux besoins d’un système de paiement de type Stripe.
Il illustre les interactions entre les systèmes OLTP, OLAP et NoSQL, ainsi que l’intégration du machine learning et des aspects de sécurité et de conformité.


