# Documentation Pipeline USD 2025 - Uptight

## Qu'est ce que le projet Pipeline USD 2025 ?

Le but de ce projet est de créer un pipeline de production pour les films de 4eme année de l'ESMA Montpellier. Ce pipeline sera basé sur le format USD (Universal Scene Description). Il utilisera principalement Houdini et Maya.

## Qu'est ce que le format USD ?

Le format **USD** (Universal Scene Description) est un format de fichier développé par Pixar pour représenter des scènes 3D. Il a été pensé pour etre le plus flexible et performant possible. L'avantage d'un tel format "universel" est qu'il peut etre utilisé par plusieurs logiciels de 3D, notament Houdini et Maya, et qu'il ne se base pas sur un logiciel en particulier.
<br>
Le format permet de stocker des informations sur la géométrie, les matériaux, les lumières, les caméras ...
<br><br>
L'USD est en train de s'imposer comme un standard dans l'industrie de l'animation et des effets visuels. De plus en plus de studios adoptent ce format pour leurs pipelines de production, car il permet une meilleure collaboration entre les différents départements (modélisation, animation, rendu, etc.). C'est pourquoi je pense qu'il peut etre un gros attout pour la création de nos films, ainsi qu'une corde de plus ajouter a notre arc.

## Pourquoi le format USD ?

Le principal avantage d’un pipeline USD réside dans son systeme de composition arcs (références de références ...).. Ce système permet d’emboîter plusieurs fichiers USD, chacun jouant un rôle précis dans la description de l’asset ou de la scène. Cela apporte de la propreté, et une flexibilité énorme.
Par exemple, il devient possible de séparer proprement la géométrie, le lookdev (matériaux, shaders), la déclaration de l’asset dans une scène ...
<br>
<br>
Cela permet une modularité extrême : si, au moment du rendu, on souhaite modifier un seul asset, il n’est pas nécessaire de remonter toute la hiérarchie de scènes ou de republier un fichier lourd depuis Maya ou Houdini. On peut directement remplacer ou surcharger le fichier concerné, sans casser l’ensemble.
<br>
<br>
Un autre avantage majeur : la gestion des niveaux de détail grâce aux systèmes de proxy. Le pipeline que je conçois repose justement sur ce principe : permettre l’affichage de géométries légères (proxies) dans le viewport, tout en gardant les versions high-res disponibles pour les étapes comme le rendu. Cela permet d’optimiser les performances des artistes, notamment en animation, où les géométries high-poly ne sont pas nécessaires.


