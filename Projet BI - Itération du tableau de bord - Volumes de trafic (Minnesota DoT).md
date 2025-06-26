# 🎯 Projet BI - Itération du tableau de bord : Volumes de trafic (Minnesota DoT)

## 📌 Contexte

Suite à la première version du tableau de bord livrée au **Minnesota Department of Transportation**, plusieurs retours ont été formulés par la partie prenante, Camila, relayés par le superviseur de projet Jack Park. Cette activité vise à **prendre en compte ces retours pour améliorer l’expérience utilisateur**, notamment pour les personnes non familières avec Tableau.

---

## 🧾 Objectifs de la modification

- Rendre le tableau de bord plus **accessible** à des utilisateurs non techniques.
- Permettre une **navigation dynamique** entre différentes échelles temporelles.
- Se **concentrer uniquement sur les données à partir de 2017**.
- Ajouter un **bouton de téléchargement** direct du tableau de bord.

---

## 🛠️ Modifications apportées

### ✅ Ajout d’un menu déroulant (filtre temporel interactif)

- **Filtre ajouté** sur la dimension `year` (année de la date/heure).
- Ce filtre permet à l’utilisateur de sélectionner les années d’intérêt.
- Application du filtre à **toutes les feuilles de calcul** liées dans le tableau de bord.
- Position : placé dans une **tuile flottante** en haut à droite pour une accessibilité immédiate.

### ✅ Ajout d’un bouton de téléchargement

- Ajout d’un **objet personnalisé** : bouton `Télécharger`.
- Ce bouton utilise une URL intégrée vers le lien public Tableau du projet.
- Il permet à l’utilisateur de **télécharger le tableau de bord ou les données** selon le paramétrage Tableau Public.
- Position : dans un bandeau supérieur, à gauche du filtre.

### ✅ Filtrage par plage temporelle (à partir de 2017)

- Le **filtre de date a été restreint** pour afficher uniquement les données de 2017 à 2018.
- Cela a été appliqué **au niveau du filtre global**, sans altérer les données sources.
- Les utilisateurs peuvent toujours changer d'échelle (jour, mois, année) grâce aux filtres dynamiques.

---

## 🧩 Éléments du tableau de bord mis à jour

| Graphique                                | Description                                                        |
|------------------------------------------|--------------------------------------------------------------------|
| **Graphique ligne - Volumes mensuels/an** | Affiche les volumes par mois pour les années 2017–2018            |
| **Carte thermique - Volumes par heure**   | Analyse de la densité horaire par jour du mois                    |
| **Graphique à barres - Conditions météo**| Regroupe le trafic selon la météo (clair, pluie, neige, etc.)     |
| **Graphique circulaire - Jours fériés**  | Compare l’affluence des différents jours fériés                   |
| **Menu filtre année**                    | Permet à l’utilisateur de choisir 2017 ou 2018                    |
| **Bouton de téléchargement**             | Téléchargement du dashboard depuis Tableau Public                 |


---
![[Minnesota Interstate Traffic Volume.pdf]]

---

## 💡 Améliorations supplémentaires

- Les **infobulles** ont été ajoutées pour afficher plus de détails lors du survol des graphiques.
- La mise en page a été optimisée avec des **tuiles flottantes** pour permettre un agencement plus flexible.
- Les **légendes ont été regroupées** logiquement avec leurs graphiques respectifs pour plus de lisibilité.

---

## 📤 Résultat

Le nouveau tableau de bord est plus **ergonomique**, **filtrable**, **personnalisable** et adapté à un public non technique. Il respecte les principes clés de design BI : accessibilité, interactivité et pertinence métier.

---

## 🧠 Compétences mobilisées

- Conception de tableaux de bord interactifs
- Filtrage multi-feuilles dans Tableau
- Ajout d’objets personnalisés (boutons, images)
- Application des retours utilisateurs en cycle itératif
- Visualisation orientée métier (affluence, météo, fériés)

---

## 📝 Note personnelle

Cette activité m’a permis de pratiquer un **cycle complet de conception BI** : de la création initiale à l’**amélioration basée sur les feedbacks**. Cela m’a sensibilisé à l’importance de l’**expérience utilisateur** dans un dashboard, surtout quand les parties prenantes ne sont pas techniques. Intégrer des filtres conviviaux et un bouton de téléchargement a rendu le tableau de bord bien plus utilisable.

---
