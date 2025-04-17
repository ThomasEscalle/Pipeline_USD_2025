# Structure

## Structure du projet

La structure du projet est organisée de manière à faciliter la gestion des fichiers et des versions. Chaque dossier correspond à une étape spécifique du pipeline de production. Voici un aperçu de la structure du projet :

### Version simplifiée :

```tree

<nom du projet>
├── 00_Pipeline/
├── 01_Management/
├── 02_PreProd/
├── 03_Production/
├── 04_Editing/
├── 05_USD/
├── 06_Archives/
├── 07_Resources/
├── 08_Linetest/
├── 09_Dev/
└── 10_Comunication/

```

## Description des dossiers

### 00_Pipeline

Ce dossier est utilisé pour stocker les fichiers de **configuration du pipeline**. Il n'y a pas a toucher a quoi que ce soit dans ce dossier. Il est géré automatiquement par le gestionnaire de pipeline (Prism dans notre cas).

### 01_Management

Ce dossier sert a tout ce qui est **gestion de projet**. Il contient les racourcis vers les documents de gestion de production.

### 02_PreProd

Ce dossier est utilisé pour stocker les fichiers de **pré-production**. Il contient les concepts arts, les storyboards, les animatics, les références, les moodboards, etc. Il est divisé en plusieurs sous-dossiers ayant chacun une fonction précise.


## Version détaillée

```tree

<nom du projet>
├── 00_Pipeline/
├── 01_Management/
├── 02_PreProd/
│   ├── 01_Scenario/
│   |   ├── 📄 doc.lnk
│   |   ├── 📄 scenario_<version>.pdf
│   ├── 02_Concept/
|   |    ├── 01_Mood/
|   |    ├── 02_Char/
|   |    |    └── <nom du personnage>/
|   |    |         ├── edits/
|   |    |         ├── references/
|   |    |         ├── 📄 modelsheet_char_<nom du personnage>_<index>.png
|   |    |         └── 📄 concept_char_<nom du personnage>.pur
|   |    ├── 03_Enviro/
|   |    |    └── <nom de l'environnement>/
|   |    |         ├── edits/
|   |    |         ├── references/
|   |    |         ├── 📄 modelsheet_env_<nom de l'environnement>_<index>.png
|   |    |         └── 📄 concept_env_<nom de l'environnement>.pur
|   |    ├── 04_Props/
|   |    |    └── <nom du prop>/
|   |    |         ├── edits/
|   |    |         ├── references/
|   |    |         ├── 📄 modelsheet_prop_<nom du prop>_<index>.png
|   |    |         └── 📄 concept_prop_<nom du prop>.pur
|   |    └── 04_Keyshot/
│   |        └── <nom du keyshot>/
│   |             ├── edits/
│   |             ├── references/
│   |             └── 📄 keyshot_<nom du keyshot>.png
│   ├── 03_Storyboard/
│   ├── 04_Color Script/
│   └── 05_Cinematography/
├── 03_Production/
│   └── ❌ Todo/
├── 04_Editing/
│   └── ❌ Todo/
├── 05_USD/
│   └── ❌ Todo/
├── 06_Archives/
│   └── ❌ Todo/
├── 07_Resources/
│   ├── Artistes/
|   |   └── <nom de l'artiste>/
│   ├── Professeurs/
|   |   └── <nom du prof>/
│   └── Externals/
├── 08_Linetest/
│   ├── 01_Jury/
│   │   └── jury_<numero du jury>
│   ├── 02_ReviewProd/
│   │   └── prod_<date>
│   └── 03_ReviewDepartements/
│       └── <departement>
├── 09_Dev/
│   ├── Dev_pipeline_tools
│   ├── Dev_maya_tools
│   ├── Dev_nuke_tools
│   ├── Dev_houdini_tool
│   └── Pub
└── 10_Comunication/
    ├── 01_Prints/
    │   ├── Affiches/
    │   ├── Flyers/
    │   ├── Cartes de visite/
    │   └── Autres/
    ├── 02_Reseaux sociaux/
    │   ├── Instagram/
    │   ├── Youtube/
    │   ├── X/
    │   ├── TikTok/
    │   ├── Linkedin/
    │   ├── Rookies/
    │   └── Autres/
    └── 03_Festivals/

```
