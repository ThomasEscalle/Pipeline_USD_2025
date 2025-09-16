# :material-checkbox-outline: Todo list



## Départements :

### <font color="green">:material-checkbox-outline:</font> Modeling Low
- <font color="green">:material-checkbox-outline:</font> - Maya
- <font color="green">:material-checkbox-outline:</font> - Houdini
- <font color="green">:material-checkbox-outline:</font> - Documentation


### <font color="green">:material-checkbox-outline:</font> Modeling High
- <font color="green">:material-checkbox-outline:</font> - Maya
- <font color="green">:material-checkbox-outline:</font> - Houdini
- <font color="red">:material-checkbox-blank-outline:</font> ZBrush
- <font color="green">:material-checkbox-outline:</font> - Documentation

### <font color="green">:material-checkbox-outline:</font> Rigging Low
- <font color="green">:material-checkbox-outline:</font> - Maya
- <font color="green">:material-checkbox-outline:</font> - Documentation

### <font color="green">:material-checkbox-outline:</font> Rigging High
- <font color="green">:material-checkbox-outline:</font> - Maya
- <font color="green">:material-checkbox-outline:</font> - Documentation

### <font color="orange">:material-checkbox-blank-outline:</font> Surfacing
- <font color="green">:material-checkbox-outline:</font> - Houdini
- <font color="red">:material-checkbox-blank-outline:</font> - Substance Painter
- <font color="green">:material-checkbox-outline:</font> - Documentation

### <font color="orange">:material-checkbox-blank-outline:</font> Modules
- <font color="green">:material-checkbox-outline:</font> - Houdini
- <font color="green">:material-checkbox-outline:</font> - Documentation
- <font color="red">:material-checkbox-blank-outline:</font> - Asset USD (faire un script pour automatiser la création des assets USD a partir des modules ?)

### <font color="green">:material-checkbox-outline:</font> Set Dressing
- <font color="green">:material-checkbox-outline:</font> - Houdini
- <font color="green">:material-checkbox-outline:</font> - Documentation

### <font color="green">:material-checkbox-outline:</font> Master Lighting
- <font color="green">:material-checkbox-outline:</font> - Houdini
- <font color="green">:material-checkbox-outline:</font> - Documentation

### <font color="red">:material-checkbox-blank-outline:</font> Lighting
- <font color="red">:material-checkbox-blank-outline:</font> - Houdini
- <font color="red">:material-checkbox-blank-outline:</font> - Documentation

### <font color="red">:material-checkbox-blank-outline:</font> RLO
- <font color="red">:material-checkbox-blank-outline:</font> - Maya
- <font color="red">:material-checkbox-blank-outline:</font> - Documentation

### <font color="red">:material-checkbox-blank-outline:</font> FLO
- <font color="red">:material-checkbox-blank-outline:</font> - Maya
- <font color="red">:material-checkbox-blank-outline:</font> - Documentation

### <font color="red">:material-checkbox-blank-outline:</font> Animation
- <font color="red">:material-checkbox-blank-outline:</font> - Maya
- <font color="red">:material-checkbox-blank-outline:</font> - Documentation

### <font color="red">:material-checkbox-blank-outline:</font> Assembly
- <font color="red">:material-checkbox-blank-outline:</font> - Houdini
- <font color="red">:material-checkbox-blank-outline:</font> - Documentation

### <font color="red">:material-checkbox-blank-outline:</font> TLO
- <font color="red">:material-checkbox-blank-outline:</font> - Houdini
- <font color="red">:material-checkbox-blank-outline:</font> - Documentation



## Outils :

- <font color="red">:material-checkbox-blank-outline:</font> - Faire le systeme de bookmarks dans le `Bp Asset Browser` Houdini


## Documentation générale :


- <font color="green">:material-checkbox-outline:</font> - Faire la page `Démarrage`
- <font color="green">:material-checkbox-outline:</font> - Finir la doc de l'`Autorig Maya`

<br>
<br>


## Notes Nathan :

1. Sur la cam, il faudrais un show / hide animatic 
    Quand on crées la camera dans les scenes (RLO), il faudrais avoir un image plane a l'interieur (qui suis) , avoir un controlle de l'opacité, et un bouton show / hide. Idéalement, avoir un bouton pour le caller en haut a gauche de la vue.
(modifier le rig de camera)

2. Prevoir un system d'offset / group pour plusieurs assets en meme temps. (compliqué)

3. Curve path pour les caméras et les véhicules.
    Prévoir un script pour faciliter la création de curve path (avec des controlleurs pour les points de la courbe) :
    - ouvrir une fenetre qui demande le nombre de controlleurs, ainsi que la taille de la courbe
    - créer une courbe avec le nombre de controlleurs demandé
    - Ajouter un node Rebuild curve, dont la résolution est drivé par un attribu
    - Ajouter un controlleur par dessus qui slide sur la courbe a partir d'un parametre U (de 0 a 1)

4. en RIG, voir comment implementer les deformers dans les rigs
