---
icon: material/home-outline 
---


# :material-home-outline: Accueil 


## Qu'est ce que le projet **Badger Pipeline** ?

Le but de ce projet est de créer un pipeline de production pour les films de 4eme année de l'ESMA Montpellier 2026. Ce pipeline sera basé sur le format USD (Universal Scene Description). Il utilisera principalement Houdini et Maya.


!!! note
    Pour l'instant, le pipeline est en phase de recherche et de développement. Il n'est pas encore opérationnel. Le but de ce document est de présenter les avancées du projet et les choix techniques qui ont été faits.

**Pourquoi Badger ? **Car ça sonne plutot bien et qu'il fallais un nom de code au projet.

------

## Qu'est ce que le format USD ?

Le format **USD** (Universal Scene Description) est un format de fichier développé par Pixar pour représenter des scènes 3D. Il a été pensé pour etre le plus flexible et performant possible. L'avantage d'un tel format "universel" est qu'il peut etre utilisé par plusieurs logiciels de 3D, notament Houdini et Maya, et qu'il ne se base pas sur un logiciel en particulier.
<br>
Le format permet de stocker des informations sur la géométrie, les matériaux, les lumières, les caméras ...
<br><br>
L'USD est en train de s'imposer comme un standard dans l'industrie de l'animation et des effets visuels. De plus en plus de studios adoptent ce format pour leurs pipelines de production, car il permet une meilleure collaboration entre les différents départements (modélisation, animation, rendu, etc.). C'est pourquoi je pense qu'il peut etre un gros attout pour la création de nos films, ainsi qu'une corde de plus ajouter a notre arc.

------

## Pourquoi le format USD ?

Le principal avantage de l'USD réside dans son systeme de composition arcs (références de références ...).. Ce système permet d’emboîter plusieurs fichiers USD, chacun jouant un rôle précis dans la description de l’asset ou de la scène. Cela apporte de la propreté, et une flexibilité énorme.
Par exemple, il devient possible de séparer proprement la géométrie, le lookdev (matériaux, shaders), la déclaration de l’asset dans une scène ...
<br>
<br>
Cela permet une modularité extrême : si, au moment du rendu, on souhaite modifier un seul asset, il n’est pas nécessaire de remonter toute la hiérarchie de scènes ou de republier un fichier lourd depuis Maya ou Houdini. On peut directement remplacer ou surcharger le fichier concerné, sans casser l’ensemble.
<br>
<br>
Un autre avantage majeur : la gestion des niveaux de détail grâce aux systèmes de proxy. Le pipeline que je conçois repose justement sur ce principe : permettre l’affichage de géométries légères (proxies) dans le viewport, tout en gardant les versions high-res disponibles pour les étapes comme le rendu. Cela permet d’optimiser les performances des artistes, notamment en animation, où les géométries high-poly ne sont pas nécessaires.

------

## Comment est structuré ce document ?

Ce document est structuré en plusieurs sections pour faciliter la compréhension du pipeline USD que je développe.

1. **[Démarage](./demarage)** : Cette section explique les étapes initiales pour commencer à utiliser le pipeline USD, y compris l'installation des logiciels nécessaires et la configuration de l'environnement de travail.

2. **[Départements](./departements)** : Chaque département du pipeline (Modélisation, Texturing, Rigging, Animation, Lighting, TLO) est détaillé dans une section dédiée. Pour chaque département, vous trouverez une description de son rôle, les entrées et sorties attendues, ainsi que des guides pratiques pour créer et publier des scènes dans Houdini ou Maya. 

3. **[Structure](./structure)** : Cette section décrit la structure des fichiers et des dossiers utilisés dans le pipeline USD, ainsi que les conventions de nommage à respecter.

4. **[Outils](./outils)** : Ici, vous trouverez des informations sur les outils et scripts développés pour faciliter le travail avec le pipeline USD.

5. **[Références](./references)** : La dernière section liste les ressources et documentations utilisées pour la création du pipeline, ainsi que des liens utiles pour approfondir vos connaissances sur l'USD.

## Contribution

Pour participer au projet, je vous conseille d'abord de me contacter afin de discuter des idées et des contributions possibles. Vous pouvez proposer des améliorations, signaler des bugs ou même contribuer directement au code si vous avez les compétences nécessaires.

Pour **contribuer au code**, voici la démarche à suivre :

1. Forkez le dépôt [GitHub du projet](https://github.com/ThomasEscalle/Pipeline_USD_2025-2026_src).
2. Clonez votre fork en local.
3. Créez une nouvelle branche pour votre fonctionnalité ou correction de bug.
4. Faites vos modifications et testez-les.
5. Commitez vos changements avec des messages clairs.
6. Poussez votre branche sur votre fork.
7. Ouvrez une Pull Request vers le dépôt principal en décrivant vos modifications.
8. Attendez la revue de code et les éventuels retours. Envoyez moi un message si j'oublie de regarder votre PR.



Pour contribuer à **l'écriture de la documentation**, je vous invite à faire éxactement la même démarche que pour le code, mais sur un dépôt différent : [GitHub de la documentation](https://github.com/ThomasEscalle/Pipeline_USD_2025).


Pour cela, il vous faudras installer MkDocs, ansi que le thème Material for MkDocs. Vous trouverez toutes les informations nécessaires dans la documentation officielle de MkDocs : [MkDocs Documentation](https://www.mkdocs.org/) et [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

<br>



Vous pouvez aussi m'envoyer un message pour que j'ajoute votre nom dans la section des contributeurs ci-dessous.

!!! info
    Voici un tutoriel pour vous aider au processus de contribution : [Comment contribuer sur GitHub](https://docs.github.com/fr/get-started/quickstart/contributing-to-projects).

------

## Contributeurs


**Thomas ESCALLE** :

Développeur principal du pipeline USD, responsable de l'architecture et de l'implémentation des outils. Contributeur principal de la documentation. Accessoirement, chef suprême super cool (CSSC) du film Uptight.

[:fontawesome-brands-linkedin:](https://www.linkedin.com/in/thomas-escalle/){ .md-button }
[:fontawesome-brands-github:](https://github.com/ThomasEscalle){ .md-button }
[:fontawesome-solid-envelope:](mailto:thomas.escalle32@gmail.com){ .md-button }
[:fontawesome-brands-artstation:](https://www.artstation.com/thomasesc){ .md-button }

------

**Mathieu CARREY** :

Développeur du plugin ZBrush, et Substance permettant ainsi les intégrations de ces logiciels dans prism, de la documentation associée, ainsi qu'une aide précieuse sur la réflexion globale du projet.

[:fontawesome-brands-linkedin:](https://www.linkedin.com/in/mathieu-carrey-91531b327/){ .md-button }
[:fontawesome-brands-github:](https://github.com/Calimer01){ .md-button }
[:fontawesome-solid-envelope:](#){ .md-button }


------

Merci aussi à :

**Nathan LUBRANO DI VAVARIA** : pour son aide sur la structure et les nomenclatures, ses retours, et pour avoir relu la documentation. 

[:fontawesome-brands-linkedin:](https://www.linkedin.com/in/nathan-lubrano-di-vavaria-b98758238/){ .md-button }
[:fontawesome-solid-envelope:](mailto:nathan.lubranodivavaria@gmail.com){ .md-button }
