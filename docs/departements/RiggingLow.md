---
icon: material/skull
---

# :material-skull: Rigging Low

![Maya_icon](../assets/icons/maya.png){width=40px}
<br>
==Travail à l'asset==

-----

## :material-information-slab-box-outline: Description

Le `Rig Low` consiste a créer des rigs simplifiés pour les modèles 3D basiques créés dans le département [`Modeling Low`](../ModelingLow). Ces rigs sont utilisés pour positionner et animer les modèles dans des le [`Rough Layout`](../RLO) et ne servirons que de référence pour l'animation.

Ces rigs n'apparaitrons pas au rendu, ils peuvent donc etre simplifiés et ne pas contenir toutes les fonctionnalités d'un rig final.

Il n'est pas possible d'avoir de systemes de variants pour un rig low ou high. Un asset ne peux contenir qu'un seul rig. Si vous avez besoin de plusieurs rigs, il faut créer plusieurs assets (exemple : une voiture, si vous avez plusieurs modeles de voitures, il faut créer un asset par modele. Il est cependant possible de créer des variations de texture.)

Pour le rig de personnages, je conseille vivement d'utiliser un **autorig** pour se simplifier la vie et etre plus efficace.

!!! note
    Les rigs ne se font que dans maya, car l'animation ne se fait que dans maya. Si vous voullez faire un rig dans houdini, il faudra le faire au niveau des FX.

-----

## :material-import: Qu'est ce qui rentre ?

Le `Rigging Low` reçoit en entrée le fichier `.usd` produit par le `Modeling Low`, qui normalement, ne contiens que de la géométrie. Il ne supporte qu'une géometrie a la fois.

-----

## :material-export: Qu'est ce qui sort ?

Le `Rigging Low` produit en sortie un fichier `.ma` pret à être utilisé dans le `Rough Layout`.

-----

## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment créer une scène dans Maya

1. Todo

-----

## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment la scène est t'elle crée ?

La scène crée contiens une hierarchie de Rig comme celle vue en cours. On peu choisir dans les options de création de la scène de la créer automatiquement, ou de créer cette hierarchie par soit meme.

De plus des assets sont importées automatiquement :

- Le `Modeling Low` de l'asset courant. L'algorythme recherche le dernier modeling low publié, dont le format est en .usd. Si il en trouve plusieurs (comme avec des variants), il ne prend que le premier. Je vous conseille donc de bien verifier au moment de la création de la scène que c'est bien le bon modeling low qui est importé. Il detecte les Modeling Low en cherchant les assets qui contiennent "ModL" et "Publish" dans leur nom.

Voici a quoi ressemble une scène de rigging low crée automatiquement :<br>
```
char_<assetName>_rigl_grp
├── char_<assetName>_rigl_geo
│    └── # Geometrie importée du Modeling Low #
├── GlobalMove_01
│    ├── Joints_01
│    ├── CTRLs_01
│    └── IKs_01
├── RelaySystem_01
└── ExtraNodes_01
     ├── ExtraNodes_To_Show_01
     └── ExtraNodes_To_Hide_01
```

-----


## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment publier une scène dans Maya

1. Todo

