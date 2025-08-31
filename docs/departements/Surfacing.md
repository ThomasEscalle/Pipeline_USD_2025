---
icon: material/format-paint
---

# :material-format-paint: Surfacing

![Houdini_icon](../assets/icons/houdini.png){width=40px}
<br>
==Travail à l'asset==

------

## :material-information-slab-box-outline: Description

Le département `Surfacing` est responsable de la création et de l'application des shaders sur les modèles 3D.

Ce qui sors du département Surfacing est un fichier `.usd` contenant les **matériaux** et les **assignations des matériaux aux géométries**. Les textures et autres resources doivent etre référencées dans le shader.

L'artiste peut créer des matériaux procéduraux, ou utiliser des textures 2D. Si il souhaite créer ses textures, il peut créer une `task` pour le `texturing` dans le département `Surfacing`.

Il est possible de créer des variants de materiaux pour un meme asset.

------

## :material-import: Qu'est ce qui rentre ?

Le département Surfacing reçoit en entrée des fichiers `.usd` contenant les modèles 3D high (`Modeling High`) (items, personnages, véhicules, etc.) sur lesquels les matériaux seront appliqués.

-----

## :material-export: Qu'est ce qui sort ?

Le département Surfacing génère un fichier `.usd` qui contiens les materiaux et les assignations des matériaux aux géométries.

------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment créer une scène dans Houdini

1. Todo

------


## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment la scène est t'elle crée ?

La scène créée contient le nécessaire pour créer des matériaux, les assigner aux géométries, nétoyer l'ensemble, et publier / exporter.

Le nétoyage automatique du Surfacing consiste à **#todo**

De plus des éléments sont importées automatiquement :

- Le `Modeling High` de l'asset courant. L'algorythme recherche les modeling High publié, dont le format est en .usd. Si il en trouve plusieurs, la scène contiendra plusieurs groupes, permettant de créer autant de matériaux qu'il ya de géométries. Il detecte les Modeling High en cherchant les assets qui contiennent "ModH" et "Publish" dans leur nom.

------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment publier une scène dans Houdini

1. Todo

