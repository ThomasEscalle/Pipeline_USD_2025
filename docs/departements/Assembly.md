---
icon: material/group
---

# :material-group: Assembly

![Houdini_icon](../assets/icons/houdini.png){width=40px}
<br>
==Travail au shot==

------

## :material-information-slab-box-outline: Description

L'assembly (assemblage) est la phase ou on vas préparer notre scène finale avant le lighting. On vas sortir un fichier usd qui vas référencer les differents elements. C'est une phase purement technique.

On vas rassembler les elements suivants :

- La **caméra** finale du shot  
- Le **set dress** de la séquence
- Les **edits du setdress** (si besoin, provenant du RLO, FLO et animation)
- Les **assets USD** texturées des personnages, et des props
- Les **animations** des personnages et des props sous forme de cache USD, qui vas override la géometrie des assets USD texturées
- Les **FXs**
- Les **CFXs**


La plupart de ces imports devrais se faire automatiquement au moment de la création de la scène, si toutes les nomenclatures on bien étées respectées en amon. Cependant, il est important de vérifier que tout est bien en place, et de faire les ajustements nécessaires avant de publier la scène.


------

## :material-import: Qu'est ce qui rentre ?

Les elements suivant sont importées au moment de la création de la scène d'assembly :

- Le `set dress` de la séquence
- Les `edits du set dress` , provenant du RLO, FLO et animation
- La `caméra` finale du shot provenant de l'animation
- Les `assets USD` texturées des personnages et des props
- Les `animations` des personnages et des props sous forme de cache USD
- Les `FXs` (si il y en a)
- Les `CFXs` (si il y en a)

------

## :material-export: Qu'est ce qui sort ?

L'assembly sors un fichier `.usd` qui référence tous les éléments importés et les organise dans une structure hiérarchique claire. Ce fichier est ensuite utilisé comme base pour le département `Lighting`, où l'éclairage et les effets visuels sont ajoutés pour finaliser l'apparence du shot.

------


## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment créer une scène dans Houdini

1. Todo

------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment publier une scène dans Houdini

1. Todo

