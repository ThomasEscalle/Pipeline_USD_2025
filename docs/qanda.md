# Questions et Réponses

## :material-diamond-stone: Qu'est-ce que Prism ?

**Prism** est un logiciel [open source](https://fr.wikipedia.org/wiki/Open_sourceww) de gestion d'assets conçu pour les projets d’animation 3D. Il automatise le flux de production, organise les fichiers et s’intègre facilement avec des outils comme Maya, Houdini ou Nuke. C’est l’outil que nous utilisons pour ce pipeline.

La plupart des fonctionnalités que nous exploitons proviennent en réalité d’un plugin Prism dédié à la gestion des ressources USD (non pris en charge nativement par Prism, sauf via un plugin payant).

**Site officiel**: [prism-pipeline.com](https://prism-pipeline.com/).


----

## :material-download-box-outline: Comment installer le pipeline sur mon ordinateur ?

----

## :material-download-circle-outline: Comment installer le pipeline sur un serveur ?

----

## :material-hexagon-multiple-outline: Qu'est ce qu'un variant en USD ?

----

## :material-account-cowboy-hat-outline: Qu’est-ce qu’un product dans Prism ?

Un product dans Prism est un élément exporté depuis un logiciel afin d’être utilisé ailleurs (dans un autre département ou un autre logiciel).
Il se distingue des scene files, qui correspondent aux scènes de travail dans lesquelles les artistes créent et modifient le contenu.

Les products peuvent être versionnés et possèdent toujours un Master.

----

## :material-account-tie-hat-outline: Qu’est-ce qu’un master product ?

Un master product dans Prism est la version principale et validée d’un product.
C’est la dernière version approuvée et publiée.

Ce concept est essentiel, car les fichiers .usd se réfèrent directement aux master products.
De cette manière, le lien reste toujours identique, tout en permettant un système de versioning efficace.

----

## :material-vector-difference: Quelle est la difference entre un **export** et un **publish** ?

Dans notre pipeline, nous faisons une distinction entre export et publish.
Ces deux actions se ressemblent, mais elles n’ont pas le même rôle.

- Un export correspond à une sauvegarde destinée à un usage interne au même département.
    - Exemple : si un asset est créé en procédural dans Houdini et que l’on veut l’ouvrir dans Maya, on effectue un export en .abc ou en .usd pour pouvoir le récupérer dans Maya.
- Un publish, en revanche, est la version validée et finale de l’objet, utilisée pour la communication entre départements.
C’est une étape essentielle, car les fichiers .usd référencent directement les publish.

----
## :material-table-chair: Quelle est la différence entre un char, un item, un module et un prop ?

- **Char** : Abréviation de "character", un char est un personnage 3D, qui va être riggé et animé.
- **Item** : Un item est un objet 3D générique dans la scène, non animable.
- **Module** : Un module est un ensemble d'items regroupés pour former une partie cohérente d'une scène. Par exemple, un module peut contenir tous les éléments d'un bureau.
- **Prop** : Un prop est un objet 3D riggé et animable, qui n'est pas un personnage. Par exemple, une voiture ou une arme.<br>
Toutes ces notions sont regroupées sous le terme générique d'assets.


**Résumé :**

| Notion           | Char (Character)                  | Item                        | Module                      | Prop                        |
|------------------|:---------------------------------:|:---------------------------:|:---------------------------:|:---------------------------:|
| Modélisé         | <font color="green">:material-check-bold:</font> | <font color="green">:material-check-bold:</font> |                             | <font color="green">:material-check-bold:</font> |
| Surfacing        | <font color="green">:material-check-bold:</font> | <font color="green">:material-check-bold:</font> |                             | <font color="green">:material-check-bold:</font> |
| Riggué           | <font color="green">:material-check-bold:</font> |                             |                             | <font color="green">:material-check-bold:</font> |
| Animable         | <font color="green">:material-check-bold:</font> |                             |                             | <font color="green">:material-check-bold:</font> |
| Groupe d'objets  |                                   |                             | <font color="green">:material-check-bold:</font> |                             |
| Exemple          | <font color="teal">Personnage</font> | <font color="teal">Chaise, livre</font> | <font color="teal">Bureau (ensemble)</font> | <font color="teal">Voiture, arme</font> |

----

## :material-bug-outline: Comment reporter un bug technique ?

Il vous suffit de créer un ticket sur github, dans la section [Issues](https://github.com/ThomasEscalle/Pipeline_USD_2025-2026_src/issues). De cette façon, nous pourrons suivre et résoudre le problème plus efficacement.<br>
Faites bien attention à préciser les étapes pour reproduire le bug, ainsi que l'environnement dans lequel il se produit. Cela m'aidera à comprendre et à résoudre le problème plus rapidement.
Voir [comment créer une issue Github](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/creating-an-issue) pour plus de détails.
