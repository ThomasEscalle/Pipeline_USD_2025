---
icon: material/table
---

# :material-table: Modules

![Houdini_icon](../assets/icons/houdini.png){width=40px}
<br>
==Travail à l'asset==

------

## :material-information-slab-box-outline: Description

Le département `Modules` est chargé de créer des assemblages d’éléments réutilisables. Un module correspond à un groupe d’items au format USD, principalement utilisés pour composer des décors ou des accessoires. Un module ne doit pas contenir d’assets animés (comme des personnages, créatures ou véhicules), mais peut inclure des assets statiques (décors, accessoires, etc.) ou même d’autres modules.

Un exemple de module pourrait être, par exemple, un bureau composé de plusieurs assets tels qu'une table, une chaise, un ordinateur, une lampe, etc. Chaque élément est un asset distinct, mais ensemble ils forment un module réutilisable.

On peut considérer un module comme une liste de références vers des fichiers `.usd`. Il est donc très léger.

Il est à différencier du `SetDress`, qui correspond à l'assemblage final d'une scène pour une séquence. Cependant, le fonctionnement est en grande partie similaire.

Les modules sont donc utilisées :

- Pour composer d'autres Modules
- Pour composer des SetDress

-----

## :material-import: Qu'est ce qui rentre ?

Un module peut recevoir en entrée plusieurs fichiers `.usd` représentant les éléments à assembler. Cependant, aucun asset n'est importé par défaut par l'algorithme de création de scène. Il est de la responsabilité de l'artiste de sélectionner et d'importer les assets nécessaires pour composer le module.

-----

## :material-export: Qu'est ce qui sort ?

Un module génère un fichier `.usd` qui référence tous les assets importés et organisés par l'artiste.



------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment créer une scène dans Houdini

1. Todo

-----


## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment la scène est t'elle crée ?

La scène créée ne contient pas d'assets importés par défaut. Il est de la responsabilité de l'artiste de sélectionner et d'importer les assets nécessaires pour composer le module.

Elle ne contient que le nécessaire pour créer un module, le nettoyer, et le publier / exporter.

Le nettoyage du module consiste uniquement à grouper les éléments ensemble sous un groupe parent. Il n'est donc pas nécessaire de trop se soucier de la hiérarchie au moment du placement des assets.


-----

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment publier une scène dans Houdini

1. Todo
