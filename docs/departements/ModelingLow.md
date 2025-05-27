
# :material-cube: Modeling Low

![Maya_icon](../assets/icons/maya.png){width=40px}
![Houdini_icon](../assets/icons/houdini.png){width=40px}
<br>
==Travail à l'asset==

## :material-information-slab-box-outline: Description

Le `Modeling Low` est le premier niveau de modélisation 3D et constitue également la première étape du pipeline de production. Il consiste à créer des modèles 3D basiques, souvent à partir de formes géométriques simples. Ces modèles serviront de proxys pour les différentes étapes de la production.

Ces modèles seront utilisés pour :

- La visualisation proxy dans le viewport.
- Servir de base pour la modélisation High.
- Servir de base pour le rigging Low, qui sera ensuite utilisé pour le Rough Layout.

<br>
---
## :material-import: Qu'est ce qui rentre ?

Il n'y a aucun département qui rentre dans le `Modeling Low`. Il s'agit du premier niveau du pipeline de production.

## :material-export: Qu'est ce qui sort ?

Le `Modeling Low` sort un fichier de type `.abc`. Il ne doit pas y avoir d'animation, ou de shading dans ce fichier.

<br>


## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment créer une scène dans Maya

1. Assurez-vous d'avoir un département de `Modeling Low` dans votre asset. Si ce n'est pas le cas, créez-en un.<br>
![image](../assets/screen_modeling_low/00.png){width=500px}

2. Créez vous une tache (exemple : `modl_01`). A noter que la nomenclature des taches n'est pas importante pour l'instant, vous pouvez mettre ce que vous voulez (UV, Procedural, Modeling, etc.).<br>
![image](../assets/screen_modeling_low/01.png){width=500px}

3. Click droit sur la partie 'files' (à droite), puis : <br>
`Create Template` -> `Modeling` -> `Maya - Low`<br>
![image](../assets/screen_modeling_low/02.png){width=500px}

Cela devrait vous créer un fichier en `.ma`. Double cliquez dessus pour l'ouvrir dans Maya.<br>
Dans maya, il devrait y avoir une hierarchie déja présente.


## ![Maya_icon](../assets/icons/maya.png){width=30px} Comment publier une scène dans Maya

1. Une fois votre modélisation terminée, assurez-vous tout est propre, sans problèmes dans la géometrie (faire un `Mesh Cleanup` si besoin).<br>
2. Assurez-vous que tous les objets soit bien hièrarchisés, et bien groupés dans le groupe `[département]_[nom]_modl_low`.<br>
![image](../assets/screen_modeling_low/03.png){width=500px}
3. Selectionnez le groupe `[département]_[nom]_modl_low` dans l'outliner.
4. Ouvrez la fenêtre du pipeline de production et cliquez sur le bouton `Publish`.<br>
![image](../assets/screen_modeling_low/04.png){width=500px}
5. Une fenêtre s'ouvre, verifiez bien que le champ `Output Type` est bien sur `abc`, et que le champ `object` est bien sur le groupe a publier.<br>
6. Cliquez sur le bouton `Add Selected` <br>
7. Cliquez sur le bouton `Publish` pour publier votre fichier.<br>
![image](../assets/screen_modeling_low/05.png){width=500px}
8. Vous devriez voir un message de succès qui s'affiche. Le modeling est maintenant publié et automatiquement appliqué a l'asset USD.



## ![Houdini_icon](../assets/icons/houdini.png){width=30px} Comment créer une scène dans Houdini

Cette fonctionnalité n'est pas encore implémentée dans Houdini.




## 