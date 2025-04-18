# Accueil 

## Qu'est ce que le projet Pipeline USD 2025 ?

Le but de ce projet est de créer un pipeline de production pour les films de 4eme année de l'ESMA Montpellier 2026. Ce pipeline sera basé sur le format USD (Universal Scene Description). Il utilisera principalement Houdini et Maya.

!!! note
    Pour l'instant, le pipeline est en phase de recherche et de développement. Il n'est pas encore opérationnel. Le but de ce document est de présenter les avancées du projet et les choix techniques qui ont été faits.

## Qu'est ce que le format USD ?

Le format **USD** (Universal Scene Description) est un format de fichier développé par Pixar pour représenter des scènes 3D. Il a été pensé pour etre le plus flexible et performant possible. L'avantage d'un tel format "universel" est qu'il peut etre utilisé par plusieurs logiciels de 3D, notament Houdini et Maya, et qu'il ne se base pas sur un logiciel en particulier.
<br>
Le format permet de stocker des informations sur la géométrie, les matériaux, les lumières, les caméras ...
<br><br>
L'USD est en train de s'imposer comme un standard dans l'industrie de l'animation et des effets visuels. De plus en plus de studios adoptent ce format pour leurs pipelines de production, car il permet une meilleure collaboration entre les différents départements (modélisation, animation, rendu, etc.). C'est pourquoi je pense qu'il peut etre un gros attout pour la création de nos films, ainsi qu'une corde de plus ajouter a notre arc.

## Pourquoi le format USD ?

Le principal avantage de l'USD réside dans son systeme de composition arcs (références de références ...).. Ce système permet d’emboîter plusieurs fichiers USD, chacun jouant un rôle précis dans la description de l’asset ou de la scène. Cela apporte de la propreté, et une flexibilité énorme.
Par exemple, il devient possible de séparer proprement la géométrie, le lookdev (matériaux, shaders), la déclaration de l’asset dans une scène ...
<br>
<br>
Cela permet une modularité extrême : si, au moment du rendu, on souhaite modifier un seul asset, il n’est pas nécessaire de remonter toute la hiérarchie de scènes ou de republier un fichier lourd depuis Maya ou Houdini. On peut directement remplacer ou surcharger le fichier concerné, sans casser l’ensemble.
<br>
<br>
Un autre avantage majeur : la gestion des niveaux de détail grâce aux systèmes de proxy. Le pipeline que je conçois repose justement sur ce principe : permettre l’affichage de géométries légères (proxies) dans le viewport, tout en gardant les versions high-res disponibles pour les étapes comme le rendu. Cela permet d’optimiser les performances des artistes, notamment en animation, où les géométries high-poly ne sont pas nécessaires.

## Miro Board

Voici le miro board que j'ai crée pour le projet. Il sert a les differentes étapes du pipeline.

<iframe width="768" height="432" src="https://miro.com/app/live-embed/uXjVIGE7tZo=/?moveToViewport=-4399,-2989,25838,9710&embedId=330836658338" frameborder="0" scrolling="no" allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen></iframe>

[Lien Miro](https://miro.com/app/board/uXjVIGE7tZo=/)

## Enjeux et Objectifs

- Nous voulions intégrer le **RLO** ( rough layout ) et le **FLO** ( final layout ) comme part entière du pipeline.
- Créer un pipeline compatible avec Prism pour faciliter la création de scènes avec des Template, et l'importation d'assets en utilisant le drag & drop de Prism
- Gérer les FX avec des **setup a la séquence** et des **intégration au shot**.

## Todo List Thomas

- :material-close-box-outline: Integrer les **FXs** dans le pipeline.
- :material-close-box-outline: Integrer les **CFXs** dans le pipeline.
- :material-close-box-outline: Integrer le **matte painting rough** dans le pipeline.
- :material-close-box-outline: Regarder comment fonctionne le systeme de **materials** et comment les appliquer procéduralement.
- :material-close-box-outline: Faire des **edits d'USD dans le RLO, FLO et Anim** au cas ou il y'ai des changements sur le set dress a faire par shot
- :material-close-box-outline: Se renseigner sur le **scale des items entre maya et houdini**, notamment sur les cameras et leurs focales
- :material-close-box-outline: Demander aux autres groupes si ils veulent faire des resources **USD en commun pour la promo** (plus de chance de passer aupres des profs ? )
- :material-close-box-outline: Regarder comment **balancer l'anim sur des assets**, a priori avec une priorité plus forte ? A enquêter
- :material-close-box-outline: Demander avis a Noah et Louis
- :material-close-box-outline: Réfléchir si je dev pluggin custom pour publish ou si on se base complètement sur celui de prism