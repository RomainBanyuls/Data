# 📊 Projet BI – Cyclistic : Tableaux de bord et Rapports

## 🎯 Objectif du projet

L'objectif est de concevoir un tableau de bord interactif pour **Cyclistic**, une entreprise de location de vélos basée à Chicago. Le tableau de bord doit permettre aux parties prenantes de comprendre les habitudes d'utilisation des vélos selon différents profils utilisateurs, et ainsi, de soutenir des décisions stratégiques (notamment la conversion des utilisateurs occasionnels en abonnés).

## 🧩 Questions métier

Le tableau de bord doit répondre à ces questions clés :
- Quels sont les **volumes d'utilisation** par type d'utilisateur (abonné vs occasionnel) ?
- Quels sont les **jours et heures de plus forte affluence** ?
- Quels types de **véhicules** sont les plus utilisés ?
- Existe-t-il des tendances saisonnières ou temporelles dans les locations ?

## 🧰 Données utilisées

Les données proviennent de l'open data de Cyclistic, incluant :
- Type d’utilisateur
- Type de vélo
- Date et heure de départ/arrivée
- Durée de la course
- Nom de station de départ et d’arrivée

Les données ont été nettoyées et modélisées avant importation dans Tableau Public.

## 📊 Visualisations créées

### 1. Volume d’utilisation par type d’utilisateur et type de vélo
- **Type** : Graphique à barres groupées
- **But** : Comparer l’utilisation des vélos par abonnés et utilisateurs occasionnels.
- **Insight** : Les abonnés utilisent majoritairement les vélos classiques, tandis que les occasionnels ont une utilisation plus variée.
![[graphique_1_utilisation_velos.png]]
### 2. Répartition horaire des trajets
- **Type** : Carte thermique (heatmap)
- **But** : Identifier les pics d’utilisation selon l’heure et le jour de la semaine.
- **Insight** : Les pics apparaissent en semaine à 8h et 17h pour les abonnés, et en journée le week-end pour les occasionnels.
![[graphique_2_heatmap_abonnes.png]]
### 3. Utilisation mensuelle (saisonnalité)
- **Type** : Graphique linéaire par mois et année
- **But** : Visualiser les variations de volume sur plusieurs mois.
- **Insight** : Forte saisonnalité, avec un pic d’activité durant l’été.
![[graphique_3_utilisation_mensuelle.png]]
### 4. Durée moyenne des trajets
- **Type** : Boxplot ou graphique à barres
- **But** : Comparer les durées selon le type d’utilisateur.
- **Insight** : Les utilisateurs occasionnels ont des trajets significativement plus longs.
![[graphique_4_duree_moyenne.png]]
## 🧠 Principaux enseignements

- Les abonnés ont des trajets courts et fréquents, souvent en semaine aux heures de pointe.
- Les utilisateurs occasionnels préfèrent les week-ends et les trajets plus longs, souvent à des fins de loisir.
- Les vélos classiques dominent, mais les vélos électriques attirent plus d'occasionnels.

## 🧩 Recommandations stratégiques

- Cibler les **utilisateurs occasionnels** avec des campagnes estivales incitant à l’abonnement.
- Proposer des **offres découvertes** pendant les week-ends.
- Ajuster la disponibilité des vélos électriques selon les pics identifiés.

## 💻 Outils utilisés

- **Tableau Public** : Visualisation et construction du tableau de bord
- **Google Sheets / Excel** : Nettoyage et pré-traitement des données
- **Markdown** : Rédaction de la documentation

## 🗒️ Note personnelle

Ce projet m’a permis d’appliquer concrètement les principes de la visualisation BI. J’ai appris à transformer des insights métier en visualisations pertinentes et à concevoir un tableau de bord logique, interactif et accessible aux décideurs non techniques.
