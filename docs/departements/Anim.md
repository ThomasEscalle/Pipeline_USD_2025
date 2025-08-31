---
icon: material/animation-outline
---

# :material-animation-outline: Animation


![Maya_icon](../assets/icons/maya.png){width=40px}
<br>
==Travail au shot==

------

## :material-information-slab-box-outline: Description

L'**animation** consiste à l'animation finale des personnages, des props et des caméras.

On recupere le setdress sous forme d'une scène USD (avec proxy et highres), les rigs, les caméras du FLO, ainsi que les ghosts animés du FLO.

Les rigs sont importés en tant que références.

------

## :material-import: Qu'est ce qui rentre ?

Ce qui rentre avant de commencer l'animation :

- Le `setdress` de la séquence, sous forme d'une scène USD (avec proxy et highres)
- Les `chars` et `props` en Rig High, sous forme de références
- Les `caméras` exportées du FLO
- Les ghosts des `éléments animées` (personnages, props animés) exportées du FLO
- Des références filmées au préalable (a importer soit meme)

------

## :material-export: Qu'est ce qui sort ?

Ce qui sort de l'animation :

- Les `éléments animées` (personnages, props animés) bakées, sous forme de cache USD.
- Les `caméras` exportées en cache USD. Elles doivent etre bakées pour ne pas perdre les animations.
- Les `edits du setdress`, sous forme d'un format USD (si besoin est de modifier le setdress de la séquence).
- Un `playblast` de chaque plan, pour validation et integration dans le montage.

------

## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment créer une scène dans Maya

1. Todo

------

## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment publier une scène dans Maya

1. Todo

