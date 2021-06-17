---
author: "*LMD - UVSQ/Paris-Saclay*"
subtitle: Félix Langot
title: Prédire l'humidité troposphérique en fonction de l'organisation
  de la convection et de la circulation de grande échelle
---

- Tic de language: 'donc' 
- Opacité image
- Dr.
- Slide 1: préciser que je vais détailler après les simulations: 'juste illustration'
- Transition slide 1-2: Ce modèle s'appuie sur les simulations, le but est de reproduire les effets de l'organisation simulé dans CRM (Modèle analytique, etc..)
- Différents types ... Citer Houze, ne pas dire à l'oral
- Aggrégation + forte encouragée par SST + forte (citation)
- +aggrégation -> assèchement (Tobin)
- differentes organisation -> cyclone + ldg = exemple de convection regroupée = aggrégée
- Slide 2: Montrer les éléments 
- Remonter les flèches rouges et bleues
- Rajouter l'évaporation
- Texte: Ascendance, flux solaire, décrire
- Réaliste -> Les simulations permettent de reproduire l'assèchement en cohérence avec les obs
- Slide 4: Montrer avec la souris 
- Slide 5: unités
- Slide 6: écrire 'Cumulonimbus'
- Slide 7: Enlever le tableau
- Écrire à '5km' label
- Slide 8: Approche dynamique: Écrire négliger le mouvement horizontal+Vitesse uniforme (horizontale + temporelle)
- Racourcir le carré violet
- N-i -> N-30min
- Slide 9: Dire qu'on met 10 jours pour descendre du sommet de la trop à 5km
- Slide 10: Enlever
- Slide 11: écrire cumulonimbus sans ascendance
- Plus de ciel clair
- Slide 12: Supprimer le tableau
- à partir ... -> Sans considération microphysique
- Ajouter 'à 5km sur les labels
- Slie 13: Clarifier -> Changer légende en équation en indiquant les couleurs
- Ajouter 'à 5km'
- Slide 14: Schéma -> ajouter texte 'zone sèche', 'système mort', 'zone humide'
- Slide 15: Ajouter stage de perspective
- Souligner importance de la durée de vie des systèmes vs l'agrégation spatiale
- La corrélation agrégation spatiale - humidité à réinterpréter -> systèmes plus gros, plus long.
- Reste a confirmer avec les observations
- Les autres données que la moyenne -> considérer la microphysique

## Introduction

### Slide 1

- Organisation = comment les nuages se répartissent sur le domaine

- Figure: vapeur d'eau intégrée verticalement $\rightarrow$ issue d'un modèle numérique simulant la convection profonde

- **Transition** Utilisation de simulations $\rightarrow$ alimenter le modèle simple + vérifier les hypothèses du modèle et évaluer son réalisme.

### Slide 2

- **CRM:** Permet de simuler des nuages convectifs avec une résolution allant de la dizaine de mètre à plusieurs kilomètres sur un espace limité en 4D (temps+espace).
  
- Simulations de 50 jours, pas de temps journalier, analyse des 10 derniers jours.

- **Simulation en RCE:**

  - Simulation avec une boîte doublement périodique, typiquement utilisé pour étudier le climat tropical
  
  - Le chauffage par convection contrebalance le refroidissement radiatif

  - Fixation de la température de surface de l'océan.

  - Inclusion de l'énergie solaire fixée à sa valeur tropicale
  
  - Évaporation de l'eau qui génère cycle hydrologique

  - **Pourquoi et comment représenter la circulation de grande-échelle:**

  - Réalisme + gammes d'humidités étudiées

  - Représenter l'ascendance de grande échelle $\rightarrow$ ajout d'un terme d'advection verticale d'humidité et de température.

  - Les simulations en RCE avec CRM sont considérées comme réalistes



### Slide 3

- **Obtention de différents types d'organisation:** On ajoute au RCE un forçage différent en fonction du type d'organisation que l'on veut favoriser

  - Cumulonimbus isolés: RCE

  - Cyclones: RCE + Coriolis

  - Ligne de grain: RCE + cisaillement de vent

- On peut calculer la RH simulée d'une parcelle troposphérique avec SAM

- $q_{v}$ l'humidité spécifique et $q_{sat}$ l'humidité spécifique de saturation, en g/kg.

- Reproduction de l'assèchement de la troposphère par le CRM

## Comment prédire les distributions de *RH*?

### Slide 4

- 2 hypothèses sur comment l'organisation influence la $RH$

- Choix de la première hypothèse: Modèle d'advection-condensation

- L'humidité spécifique d'une parcelle $q_{v}$ reste
constante en l'absence de saturation (et donc de condensation)

- On dispose de l'humidité spécifique de saturation
$q_{sat}$ en fonction de l'altitude grâce au modèle SAM

- On peut donc prédire la RH de la troposphère à partir de
l'altitude de dernière saturation de la parcelle

Le modèle met en évidence les relations entre la RH et l'organisation de la convection

- Vitesse de subsidence de l'environnment $\rightarrow$ Si temps
de descente augmente, la probabilité de rencontrer un nuage augmente.

- Organisation $\rightarrow$ distribution des nuages
$\rightarrow$ probabilité de rencontre. Nuages sont très regroupés =
baisse de la probabilité

## Altitude de dernière saturation - Approche statique

### Slide 5

Comment trouver l'altitude de dernière saturation d'une parcelle se
situant dans la troposphère?

- **Approche statique:** L'altitude de dernière saturation d'une parcelle troposphérique correspond à l'altitude du nuage le plus proche au-dessus de la parcelle.

- SAM: rapports de mélange d'eau et de glace (*water mixing ratio, ice mixing ratio*) $q_{c},q_{i} \rightarrow$ Détection des nuages

  - Si $q_{c} + q_{i} > 10^{- 6}$ alors le point de grille est dans un nuage

**Transition** On peut donc mesurer l'altitude du nuage le plus proche de chaque point de grille à chaque pas de temps des simulations

### Slide 6

Bleu foncé = $z_{max}$...

## Altitude de dernière saturation - Approche dynamique

### Slide 7

### Slide 8

Simulations avec ascendance: vitesse verticale totale dans
l'environnement $w_{tot} = w_{env} + w_{LS}$, où $w_{LS}$ est
l'ascendance imposée.

- Exemple =  simulation de cumulonimbus sans ascendance

- On choisit 10 parcelles étant à l'altitude $z_{parcel}$ aux 10 derniers pas de temps.

- On remonte le temps et on trace la trajectoire de la parcelle gouvernée par $w_{tot}$.

**Transition** En utilisant les mêmes conditions pour détecter les nuages, on obtient les altitudes de dernières saturations suivantes:

Bibliographie
