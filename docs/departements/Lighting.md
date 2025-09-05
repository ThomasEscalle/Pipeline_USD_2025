---
icon: material/lightbulb-variant
---

# :material-lightbulb-variant: Lighting

![Houdini_icon](../assets/icons/houdini.png){width=40px}
<br>
==Travail au shot==

------

## :material-information-slab-box-outline: Description

Le département `Lighting` est responsable de la création et de l'ajustement de l'éclairage dans une scène 3D par shot. Le lighteur travaille par dessus la scène assemblée par le département `Assembly`, qui inclut les personnages animé, les décors, les accessoires, et les effets visuels. Par dessus tout ça, on rajoute aussi le `MasterLighting`.

On peux soit ajuster les lumières existantes, les desactiver, ou en ajouter de nouvelles. 

Les lights peuvent etre animées, pour simuler des effets de lumières dynamiques, comme des éclairs, des feux de véhicules, ou des lumières de scène.

!!! tip
    Il est aussi possible, en cas de gros besoin, de modifier certains materiaux, ou certains elements de la scene. Mais cela doit rester exceptionnel.

------

## :material-import: Qu'est ce qui rentre ?

Au moment de la création de la scène, deux elements principaux sont importés :

- La scène d'`Assembly`, qui inclut tous les éléments nécessaires pour le shot, tels que les personnages, les décors, les accessoires, et les effets visuels.
- Le fichier de `Master Lighting`, qui contient les lumières et les réglages d'éclairage globaux pour la séquence.

------

## :material-export: Qu'est ce qui sort ?

On exporte un fichier `.usd` qui inclut la référence de la scène d'assembly, ainsi que les lumières et les réglages d'éclairage spécifiques au shot. Ce fichier est ensuite utilisé pour le rendu final de la scène dans le TLO.

------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment créer une scène dans Houdini

1. Todo

------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment publier une scène dans Houdini

1. Todo

