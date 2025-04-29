# Departements

## Travail a l'asset


<div class="grid cards" markdown>

-   [:material-cube:{ .lg .middle } **Modeling Low** ( ``modl`` )](#modeling-low-modl)
-   [:material-cube-outline:{ .lg .middle } **Modeling High** ( ``modh`` )](#modeling-high-modh)
-   [:material-skull:{ .lg .middle } **Rigging Low** ( ``rigl`` )](#rigging-low-rigl)
-   [:material-skull-outline:{ .lg .middle } **Rigging High** ( ``righ`` )](#rigging-high-righ)
-   [:material-table:{ .lg .middle } **Modules** ( ``modu`` )](#modules-modu)
-   [:material-brush:{ .lg .middle } **Lookdev / Texturing** ( ``lkdv`` )](#lookdev-texturing-lkdv)

</div>

## Travail a la séquence

<div class="grid cards" markdown>

-   [:material-animation:{ .lg .middle } **Set Dress** ( ``stdr`` )](#set-dress-stdr)
-   [:material-camera-enhance-outline:{ .lg .middle } **RLO** ( ``rlo`` )](#rlo-rlo)
-   [:material-lightbulb-on-30:{ .lg .middle } **Master Lighting** ( ``lght`` )](#master-lighting-lght)

</div>

## Travail au shot

<div class="grid cards" markdown>

-   [:material-camera-image:{ .lg .middle } **FLO** ( ``flo`` )](##flo-flo)
-   [:material-animation-outline:{ .lg .middle } **Animation** ( ``anim`` )](#)
-   [:material-group:{ .lg .middle } **Assembly** ( ``asmb`` )](#)
-   [:material-lightbulb-variant:{ .lg .middle } **Lighting** ( ``lght`` )](#)
-   [:material-cog-outline:{ .lg .middle } **TLO** ( ``tlo`` )](#)
-   [:material-image-edit-outline:{ .lg .middle } **Compositing** ( ``comp`` )](#)
-   [:material-image-filter-drama-outline:{ .lg .middle } **Matte Painting** ( ``matp`` )](#)

</div>


----



## :material-cube: Modeling Low ( ``modl`` )

Modeling Low est le département responsable de la création des assets 3D en basse définition. Les modèles doivent être réalisés avec le moins de polygones possible, sans chanfreins (bevels) ni arêtes de contention.
Le modèle ainsi créé sert de base à tous les autres départements. Il est utilisé comme proxy pour l'affichage dans le viewport, et constitue également la géométrie utilisée pour les items dans les scènes d'animation.

``` mermaid
graph TB
  B{ **Modeling Low**};
  B -->C[Modules];
  B -->D[Rig Low];
  B -->E[Modeling High];
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.

----

## :material-cube-outline: Modeling High ( ``modh`` )

Modeling High est le département responsable de la création des assets 3D en haute définition. Le modèle crée est celui qui sera utilisé pour le rendu final.
Il peut etre sculpté sur ZBrush et importé dans Maya, ou bien il peut être créé directement dans Maya.

Il travaille sur la base de la géometrie low (``modl``). Il peut soit recréer une nouvelle géometrie de zéro, mais en respectant les proportions de la géometrie low, soit utiliser la géometrie low comme base et ajouter des détails supplémentaires comme des chanfreins (bevels) et des arêtes de contention.

Il est très important que les modés qui sortent de ce département soient de la plus haute qualité possible. Ils doivent respecter les normes suivantes :

- Aient des UVs propres et non superposées.
- Une géometrie propre, sans nomanifolds, faces inversées, ou autres erreurs de géometrie.

``` mermaid
graph TB
  A[ **Modeling Low**];
  A -->B[Modeling High];
  B{ **Modeling High**};
  B -->D[Rig High];
  B -->E[Lookdev & Texturing];
  B -->F[CFX Setup];
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.

----

## :material-skull: Rigging Low ( ``rigl`` )

Le département Rigging Low est responsable de la création des rigs sur la géométrie low. Il doit produire un rig de base, très simple, servant uniquement à prévisualiser les proportions des personnages et des accessoires dans le RLO.
Il n’est pas nécessaire d’ajouter un rig facial ni de systèmes complexes comme des ribbons ou des vêtements. Le rig doit simplement être fonctionnel et utilisable pour les besoins de l’animation.

L’utilisation d’un autorig est recommandée afin de simplifier et accélérer le processus. [WombatAutoRig](https://github.com/ThomasEscalle/WombatAutoRig)

``` mermaid
graph TB
  A[ **Modeling Low**];
  A -->B[Rigging Low];
  B{ **Rigging Low**};
  B -->C[RLO];
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.

----

## :material-skull-outline: Rigging High ( ``righ`` )

Le département Rigging High est responsable de la création des rigs en haute définition. Il doit produire un rig complet, incluant un rig facial ainsi que des systèmes avancés comme des ribbons, des vêtements ou tout autre élément nécessitant des contrôles complexes.

Si le personnage nécessite des vêtements ou des cheveux simulés (CFX), il est préférable de les inclure dans la modélisation, de les rigger dans un premier temps, puis de les remplacer par une simulation au moment opportun dans la production.


``` mermaid
graph TB
  A[ **Modeling High**];
  A -->B[Rigging High];
  B{ **Rigging High**};
  B -->C[Animation];
  B -->D[FLO];
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.

----

## :material-table: Modules ( ``modu`` )

Le département Modules est responsable de la création des modules (assemblages de plusieurs items).

``` mermaid	
graph TB
  A[ **Modeling Low**];
  A -->B[Modules];
  B{ **Modules**};
  B -->C[Set Dress];
```


!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.


----

## :material-brush: Lookdev / Texturing ( ``lkdv`` )

Le département Lookdev / Texturing est responsable de la création des textures et des shaders pour les modèles 3D.

Pour cela, il peut utiliser Substance Painter, Mari, ou tout autre logiciel de texturing adapté.
Les shaders doivent ensuite être créés dans Houdini, afin d’être exportés au format USD pour le pipeline.

La partie Texturing consiste à peindre et générer les textures (par exemple dans Substance Painter), tandis que la partie Lookdev consiste à assembler ces textures et à développer les shaders finaux utilisés dans le rendu.


``` mermaid
graph TB
  A[ **Modeling High**];
  A -->B[Lookdev / Texturing];
  B{ **Lookdev / Texturing**};
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.



----

## :material-animation: Set Dress ( ``stdr`` )

Le département Set Dress est responsable de la création des décors pour chaque séquence.
Le setdress constitue la construction finale du décor : c’est un assemblage cohérent d’items et de modules, positionnés pour composer l’environnement tel qu’il apparaîtra à l’image.

``` mermaid

graph TB
  A[ **Modeling Low**];
  A -->B[Set Dress];
  B{ **Set Dress**};
  B -->C[RLO];
  B -->D[FLO];
  B -->E[Animation];
  B -->F[Master Lighting];
  B -->G[Assembly];
```


!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.

-----

## :material-camera-enhance-outline: RLO ( ``rlo`` )

Le département RLO (Rough Layout) est responsable de la création d’un layout très basique de la séquence. Il est chargé de placer les caméras ainsi que les personnages en low rig (rigl) dans la scène.

Il travaille en parallèle avec le département de montage afin de s’assurer que le layout est conforme au découpage et au rythme définis dans le montage de la séquence.

``` mermaid
graph TB
  A[ **Set Dress**];
  A -->B[RLO];
  B{ **RLO**};
  B -->D[FLO];
  B -->E[Master Lighting];

```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.


-----

## :material-lightbulb-on-30: Master Lighting ( ``lght`` )

Le département Master Lighting est responsable de la création de l’éclairage principal d’une séquence.
Il définit un éclairage global cohérent qui servira de base au travail du département Lighting, lequel se chargera par la suite d’affiner cet éclairage plan par plan pour l’intégrer parfaitement à l’image finale.

``` mermaid
graph TB
  A[ **Set Dress**];
  A -->B[Master Lighting];
  B{ **Master Lighting**};
  B -->C[FLO];
  B -->D[Lighting];
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.


-----

## :material-camera-image: FLO ( ``flo`` )

Le département FLO (Final Layout) est responsable de la création du layout final de la séquence. Il doit s’assurer que le layout est conforme au découpage et au rythme définis dans le montage de la séquence. Il affine le placement des caméras et des personnages. A la difference du RLO il travaille a la séquence, avec des rigs en haute définition (righ).

``` mermaid
graph TB
D[ **Rig High**];
D -->B[FLO];
  A[ **RLO**];
  A -->B[FLO];
  B{ **FLO**};
  B -->C[Animation];
```

!!! info ""
    **:material-arrow-down-bold-box-outline: Qu'est ce qui rentre ? :**
    Ce qui rentre.

!!! info ""
    **:material-arrow-up-bold-box-outline: Qu'est ce qui sort ? :**
    Ce qui sort.

----

