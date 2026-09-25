# Analyse qualité : Suivi des défauts de production

## 🎯 Contexte & objectif
Dans un cadre industriel, un article est prélevé aléatoirement sur la chaîne de production toutes les 15 minutes durant 10 jours, pendant un poste de travail de 8h, soit 320 prélèvements. Il est ensuite inspecté pour détecter d'éventuels défauts. L'objectif est d'identifier des tendances ou des dérives dans le processus de fabrication.

## 📊 Conclusions clés
Les articles possèdent en moyenne 10,3 défauts par prélèvement, sans dérive détectée sur la période. La carte de contrôle c (Shewhart, norme ISO 7870) démontre qu'il n'y a pas lieu d'intervenir, la variabilité de la qualité reste dans la norme.

## 🗂️ Structure du projet
data/raw : contient les données brutes, jamais modifiées.
notebooks : contient le fichier d'analyse exploratoire.

## 🔧 Reproduire l'analyse
Cloner ce répertoire, créer un environnement virtuel, installer les bibliothèques nécessaire au projet listées dans le fichier requirements.txt, et lancer le notebook 01_eda_defects.ipynb situé dans notebooks/.

## 🛠️ Outils & méthodes
Pour réaliser ce projet j'ai utilisé les bibliothèques : pandas, matplotlib et seaborn pour visualiser mes données.

J'ai également réalisé une carte de contrôle c, l'outil standard de la maîtrise statistique des procédés (SPC) qui permet de savoir si un écart est considéré comme normal, ou s'il révèle une cause spécifique du processus, nécessitant une intervention et/ou analyse de cause plus poussée.