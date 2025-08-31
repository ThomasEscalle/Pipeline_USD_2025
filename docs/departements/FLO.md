---
icon: material/camera-image
---

# :material-camera-image: FLO

![Maya_icon](../assets/icons/maya.png){width=40px}
<br>
==Travail au shot==

------

## :material-information-slab-box-outline: Description

FLO (pour Final Layout) est la phase de **layout au shot**. On vas y placer les personnages, les caméras, et les éléments dynamiques (props animés, véhicules, etc...) pour chaque plan d'une séquence.

On recupère les assets animés du RLO, ainsi que les caméras et les assets statiques du SetDress. On place tout ça dans la scène, on ajuste les positions, les échelles, les orientations, et on crée les animations de caméra si nécessaire.

Les assets animées importées du RLO ne sont pas riggées, ils sont présents sous forme de ghost.

------

## :material-import: Qu'est ce qui rentre ?

Ce qui rentre dans le FLO : 

- Les `caméras` exportées du RLO
- Le `setdress` de la séquence
- Les `edits du setdress` effectuées dans le RLO
- Les `chars` et `props` en Rig High
- Les ghosts des `éléments animées` (personnages, props animés) exportées du RLO

------

## :material-export: Qu'est ce qui sort ?

Ce qui sort du FLO :

- Les `éléments animées` (personnages, props animés) bakées, sous forme de cache USD.
- Les `caméras` exportées en .ma (pour conserver les curves et ne pas perdre les animations)
- Les `edits du setdress`, sous forme d'un format USD (si besoin est de modifier le setdress de la séquence).
- Un `playblast` de chaque plan, pour validation et integration dans le montage.

------


## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment créer une scène dans Maya

1. Todo

------

## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment publier une scène dans Maya

1. Todo

