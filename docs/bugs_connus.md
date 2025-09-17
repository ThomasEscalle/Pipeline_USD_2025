---
title: Bugs Connus
icon: material/bug
---

# :material-bug: Bugs Connus

Cette page recense les bugs connus du pipeline et des outils associés.

## Liste des bugs

---

### Utilisation simultanée de l'USD_View et du système de fabrication des variants

Il y'a un problème avec l'**utilisation simultanée de l'USD_View, et du systeme de fabrication des variants**.

Lorsqu’un fichier USD est ouvert dans l’interface via usdView, sa hiérarchie reste en mémoire dans le cache global d’USD. Même après suppression du fichier sur disque, USD peut continuer à considérer que ce fichier existe. Cela provoque une erreur lors d’une tentative de recréation d’un fichier portant le même nom ou le même identifiant dans le système de variants. La solution actuelle est de redémarrer prism, puis de réouvrir l'outil de "variants connection" pour valider.

Je n'ai pas encore trouvé de solution à ce problème.

---

*Merci de me signaler tout nouveau bug via le [repository github](../qanda/#comment-reporter-un-bug-technique).*
