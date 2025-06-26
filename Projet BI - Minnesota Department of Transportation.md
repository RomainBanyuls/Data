# 🎯 Projet BI - Minnesota Department of Transportation  
**Formation :** Google Business Intelligence  
**Cours :** Décisions, décisions : Tableaux de bord et rapports  
**Module 2 :** Activité – Créer des graphiques à partir de données de trafic  

## 🗂️ Contexte du projet

Le **Minnesota Department of Transportation** a sollicité la création d’un tableau de bord pour analyser et améliorer son infrastructure routière. En tant qu’analyste BI, l’objectif est de concevoir des **visualisations efficaces** à partir de données réelles de trafic (fichier : `Metro_Interstate_Traffic_Volume.csv`).

**Sources :**
- 📧 Courriel du superviseur (Jack Park)
- 📁 Scénario de jeu de rôle (Camila, partie prenante)
- 📊 Données de trafic issues de capteurs autoroutiers

## 🎯 Objectifs des visualisations

1. **Volume de trafic sur différentes échelles temporelles :** année, mois, semaine, jour, heure
2. **Volume de trafic selon les conditions météorologiques**
3. **Volume de trafic pendant les jours fériés**

## 📝 Planification des graphiques (Maquette)

Une **maquette papier** a été réalisée pour organiser visuellement les trois besoins principaux :

- 🧭 Axe principal : évolutif selon le temps
- 🖼️ Format choisi : combinaison de line charts, bar charts, scatter plots et heatmaps
- 🎨 Utilisation de codes couleur, étiquettes et titres explicites pour chaque graphique

## 🛠️ Démarche technique

### Étapes suivies :
1. **Importation du fichier CSV** dans Tableau Public
2. **Exploration des colonnes clés :**
   - `date_time` (Date et Heure)
   - `traffic_volume` (Volume de trafic)
   - `weather_main` (Météo)
   - `holiday` (Jour férié)
3. **Création de champs dérivés** :
   - `IS_HOLIDAY` : `if [holiday] = "None" then null else "X" end`
   - Extraction des composants temporels : année, mois, jour, heure
4. **Application de filtres dynamiques** :
   - Par période temporelle
   - Par météo
   - Par jours fériés

## 📈 Graphiques réalisés

### 📊 Graphique 1 : Trafic par heure
- **Type** : Carte thermique
- **Dimensions** : Date, Heure
- **Mesure** : Moyenne du volume de trafic
- **Utilité** : Identifier les pics de trafic journaliers/mensuels
![[graphique_volume_par_heure_heatmap.png]]

### 🌦️ Graphique 2 : Volume de trafic selon la météo
- **Type** : Bar chart + Filtre météo
- **Dimensions** : Météo principale, Heure
- **Mesure** : Moyenne du volume de trafic
- **Utilité** : Évaluer l’impact des conditions climatiques sur le trafic
![[graphique_2_trafic_par_meteo.png]]
### 🎉 Graphique 3 : Trafic pendant les jours fériés
- **Type** : Scatter plot + Highlight
- **Dimensions** : Jour, Heure
- **Mesure** : Volume de trafic
- **Utilité** : Comparer le trafic normal et celui des jours fériés
![[graphique_3_trafic_jours_feries.png]]
![[graphique_volume_par_jour_ferie.png]]
## ⚙️ Techniques et options utilisées

- Filtres interactifs (date relative, météo, jours fériés)
- Champs calculés (`IS_HOLIDAY`)
- Ajout de légendes automatiques (`Show Caption`)
- Respect des principes d’accessibilité (couleurs + étiquettes)

## 📌 Résultats

Les visualisations permettent de répondre clairement aux besoins exprimés par la partie prenante. Elles facilitent :
- Une prise de décision éclairée pour les constructions futures
- La détection des périodes de trafic critique
- Une meilleure planification en cas de conditions météorologiques défavorables ou de jours fériés

## 🧠 Compétences mobilisées

- Lecture de besoins métiers
- Création de maquettes visuelles
- Utilisation avancée de Tableau Public
- Création de champs calculés
- Application de filtres dynamiques
- Bonnes pratiques de design de dashboards

## 🗒️ Note personnelle

Ce projet m’a permis d’appliquer une méthodologie complète de création de visualisations en BI. J’ai particulièrement apprécié la liberté créative dans le choix des graphiques, tout en répondant à des objectifs concrets. Le travail avec des données réelles renforce la dimension professionnelle de l’activité.

---
