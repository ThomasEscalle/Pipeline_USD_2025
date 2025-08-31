---
icon: material/lightbulb-on-30
---

# :material-lightbulb-on-30: Master Lighting (mlght)

![Houdini_icon](../assets/icons/houdini.png){width=40px}
<br>
==Travail à la séquence==

------

## :material-information-slab-box-outline: Description

Le département `Master Lighting` est responsable de la création de l'éclairage principal et de l'ambiance visuelle d'une séquence. Contrairement au département `Lighting` qui se concentre sur l'éclairage spécifique des personnages et des éléments animés, le Master Lighting établit le cadre global de l'éclairage pour toute la scène. L'artiste doit se concentrer sur la création d'une atmosphère cohérente et immersive qui soutient la narration visuelle de la séquence.

Les lumières créées doivent donc etre réutilisables dans tous les shots.

!!! tip
    Il seras possible de modififier les paramètres des lumières, de désactiver ou d'ajouter des lumières en plus dans le département `Lighting`.


------

## :material-import: Qu'est ce qui rentre ?

Le Master Light se fais directement sur le SetDress de la séquence. Il n'y a pas besoin de personnages, ni de caméras spécifiques.

------

## :material-export: Qu'est ce qui sort ?

Le département Master Lighting génère un fichier `.usd` qui contient les lumières et les réglages d'éclairage pour la séquence. Il ne dois pas référencer le SetDress car celui-ci seras réimporté dans le département `Assembly`.
Ce fichier est ensuite utilisé comme base pour le département `Lighting`, où des ajustements spécifiques peuvent être apportés pour chaque shot individuel.

------

## :material-lightbulb-on-30: Quels sont les nodes que je peux créer ?


------


## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment créer une scène dans Houdini

1. Todo

------

## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment publier une scène dans Houdini

1. Todo

