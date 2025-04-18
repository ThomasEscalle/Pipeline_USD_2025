# Structure

!!! note ""
    La structure du projet est organisée de manière à faciliter la gestion des fichiers et des versions. Chaque dossier correspond à une étape spécifique du pipeline de production. Voici un aperçu de la structure du projet :

```tree
<nom du projet>
├── 📁 00_Pipeline/
├── 📁 01_Management/
├── 📁 02_PreProd/
├── 📁 03_Production/
├── 📁 04_Editing/
├── 📁 05_USD/
├── 📁 06_Archives/
├── 📁 07_Resources/
├── 📁 08_Linetest/
├── 📁 09_Dev/
└── 📁 10_Comunication/
```

### Détails des dossiers


| Nom du dossier      | Description                          |
| ----------- | ------------------------------------ |
| [00_Pipeline](/Pipeline_USD_2025/00_Pipeline)          | Contient les outils et scripts utilisés pour le pipeline.  |                                                                             
| [01_Management](/Pipeline_USD_2025/01_Management)      | Dossier de gestion du projet, incluant les documents de planification et de suivi.|
| [02_PreProd](/Pipeline_USD_2025/02_PreProd)            | Dossier de pré-production, contenant les concepts, storyboards et autres documents préparatoires.|
| [03_Production](/Pipeline_USD_2025/03_Production)      | Dossier de production, où se trouvent les fichiers de travail des artistes.|
| [04_Editing](/Pipeline_USD_2025/04_Editing)            | Dossier d'édition, contenant les fichiers de montage et de post-production.|
| [05_USD](/Pipeline_USD_2025/05_USD)                    | Dossier contenant les publishs des fichiers USD et les ressources associées.|
| [06_Archives](/Pipeline_USD_2025/06_Archives)          | Dossier d'archives, où sont stockés les fichiers et versions obsolètes des USD.|
| [07_Resources](/Pipeline_USD_2025/07_Resources)        | Dossier contenant les ressources externes, comme les références et les documents de recherche.|
| [08_Linetest](/Pipeline_USD_2025/08_Linetest)          | Dossier contenant les fichiers servant a la presentation du projet, comme les jury et les reviews.|
| [09_Dev](/Pipeline_USD_2025/09_Dev)                    | Dossier de développement, où se trouvent les scripts et outils en cours de développement.|
| [10_Comunication](/Pipeline_USD_2025/10_Comunication)  | Dossier de communication, contenant les fichiers de communication externe, comme les réseaux sociaux et les festivals.|


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
