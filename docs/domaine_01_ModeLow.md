# Modeling Low

## Description

| Nom         | Valeur                               |
| ----------- | ------------------------------------ |
| `GET`       | :material-check:     Fetch resource  |
| `PUT`       | :material-check-all: Update resource |
| `DELETE`    | :material-close:     Delete resource |


## Qu'est ce que le modeling low ?

Le modeling low est la première étape de la création d'un personnage ou d'un objet 3D. Il s'agit de créer une version simplifiée du modèle, qui sera ensuite utilisée comme proxy pour les étapes suivantes du pipeline. Le but est de créer une géométrie légère et optimisée, qui pourra être utilisée dans le viewport de Houdini ou Maya sans ralentir le système.

Il est utilise pour commencer a placer les elements sur le setdress, sans forcement avoir le modèle final. Il est aussi utilisé pour les animations, afin de ne pas surcharger le système avec des modèles trop lourds.

## Qu'est ce qui rentre ?

- Rien de particulier, le modeling low est crée de 0 sur une scène maya vide.

## Qu'est ce qui sort ?

- Un fichier USD contenant la géométrie low poly du personnage ou de l'objet.