---
icon: material/camera-enhance-outline
---

# :material-camera-enhance-outline: RLO

![Maya_icon](../assets/icons/maya.png){width=40px}
<br>
==Travail à la séquence==

------

## :material-information-slab-box-outline: Description

Le RLO (pour Rough Layout) est la phase de **layout à la séquence**. C'est le moment ou l'on vas faire un premier jet de mise en place des **plans**, des **personnages** et des **caméras**.

On vas importer le `setdress`, `les personnages` (rig low), et `créer autant de caméras qu'il ya de shots` dans la séquence. Puis on vas positionner les personnages et les caméras pour chaque plan.
Il n'est pas nécessaire de faire une animation poussée, mais il faut que les personnages soient positionnés correctement dans le décor, et que les caméras soient placées pour capturer l'action. Les caméras non plus n'on pas besoin d'être animées de manière fluide, mais elles doivent être placées de manière à capturer l'action de chaque plan.

!!! warning "Attention a la nomenclature des caméras"
    Il est essentiel de **nommer précisément les caméras créées** dans le RLO. En effet, ces caméras seront exportées puis distribuées dans chaque shot grâce à leur nommage cohérent. Une mauvaise nomenclature peut entraîner des erreurs lors de la distribution des caméras dans les plans.

    La nomenclature est la suivante : **cam_seq####_shot####_version####**

    - `seq####` : le numéro de la séquence
    - `shot####` : le numéro du plan dans la séquence
    - `version####` : la version de la caméra. Par défaut, on commence avec version0001. La version est facultative, mais recommandée pour garder une trace des modifications. C'est a votre préférence.

    Exemple : cam_seq0010_shot0030_version0001
    
------

## :material-import: Qu'est ce qui rentre ?

Le `RLO` reçoit :

- Le `setdress` de la séquence
- Les `personnages` (rig low)
- Les `props` nécessaires

Evidement, il faut aussi avoir la `storyboard` et le `script` de la séquence pour pouvoir positionner les éléments correctement.

------

## :material-export: Qu'est ce qui sort ?

Il y'a plusieurs publishs a effectuer dans le RLO :

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
