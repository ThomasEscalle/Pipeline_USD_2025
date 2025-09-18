---
icon: material/power-plug-outline
---

# :material-power-plug-outline: Prism Plugin Principal

Le pluggin Prism est le coeur du système du pipeline. J'ai assayé de garder l'esprit de prism, mais en integrant de manière fluide et discrète les outils USD.

Voici les fonctionnalités principales du pluggin Prism:

1. **Création de scènes procédurales**: Le pluggin permet de générer des scènes dans differents logiciels (Houdini,Maya et bientot Nuke) et pour chaque départements. Les scènes crées sont générées via script python, ce qui permet d'avoir une hierarchie propre, des nomenclatures respectées, des exports pré configurées, ainsi qu'un import semi automatique des départements précédents. Les scènes générées sont au maximum optimisées et permettent de netoyer et de ranger facilement les scènes.

2. **Gestion des assets USD** : Le pluggin crées automatiquement, en background, les differents fichiers USD nécessaire pour fabriquer vos scènes. Cependant, il est possible de modifier manuelement ces fichiers pour plus de flexibilité. Il integre une fenetre qui liste ces differents assets, et permet de les drag & drop directement dans houdini.

3. **Gestion des variants** : Le pluggin permet de modifier les variants des assets directement depuis l'interface du pluggin. Vous pouvez ainsi choisir pour chaque variant de chaque asset, quelle modelisation et quel materiau utiliser.

4. **Integration de l'API USD et de USDview** : Le pluggin intègre l'API USD et permet de visualiser les assets USD directement dans USDview. Il est possible de lancer USDview depuis le pluggin, et de charger la scène courante ou un asset spécifique. C'est un outil très pratique pour vérifier rapidement les assets et les scenes et trouver d'eventueles erreurs.