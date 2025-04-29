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

## Détails des dossiers


| Nom du dossier      | Description                          |
| ----------- | ------------------------------------ |
| [00_Pipeline](#00_pipeline)          | Dossier racine du projet, contenant la structure de base et les fichiers de configuration.|                                                                             
| [01_Management](#01_management)      | Dossier de gestion du projet, incluant les documents de planification et de suivi.|
| [02_PreProd](#02_preprod)            | Dossier de pré-production, contenant les concepts, storyboards et autres documents préparatoires.|
| [03_Production](#03_production)      | Dossier de production, où se trouvent les fichiers de travail des artistes.|
| [04_Editing](#04_editing)            | Dossier d'édition, contenant les fichiers de montage et de post-production.|
| [05_USD](#05_usd)                    | Dossier contenant les publishs des fichiers USD et les ressources associées.|
| [06_Archives](#06_archives)          | Dossier d'archives, où sont stockés les fichiers et versions obsolètes des USD.|
| [07_Resources](#07_resources)        | Dossier contenant les ressources externes, comme les références et les documents de recherche.|
| [08_Linetest](#08_linetest)          | Dossier contenant les fichiers servant a la presentation du projet, comme les jury et les reviews.|
| [09_Dev](#09_dev)                    | Dossier de développement, où se trouvent les scripts et outils en cours de développement.|
| [10_Comunication](#10_comunication)  | Dossier de communication, contenant les fichiers de communication externe, comme les réseaux sociaux et les festivals.|




### 00_Pipeline

```tree
<nom du projet>
└── 📁 00_Pipeline/
```

**Description :** Dossier géré automatiquement pas le gestionnaire de pipe. Il contiens tous les fichiers de configuration et les scripts nécessaires au bon fonctionnement du pipeline. 
C'est aussi ici que se trouve les templates de fichiers et de dossiers utilisés dans le projet.

---

### 01_Management

```tree
<nom du projet>
└── 📁 01_Management/
```

**Description :** Dossier de gestion du projet, incluant les documents de planification et de suivi. Il contient des fichiers de gestion de projet, des documents de suivi et d'autres ressources nécessaires à la gestion du projet.

---

### 02_PreProd

```tree
<nom du projet>
└── 📁 02_PreProd/
```

**Description :** Dossier de pré-production, contenant les concepts, storyboards et autres documents préparatoires. Il est divisé en plusieurs sous-dossiers pour organiser les différents aspects de la pré-production.

---

### 03_Production

```tree
<nom du projet>
└── 📁 03_Production/
```

**Description :** Dossier de production, où se trouvent les fichiers de travail des artistes. Il est divisé en plusieurs sous-dossiers pour organiser les différents aspects de la production.

---

### 04_Editing

---

### 05_USD

---

### 06_Archives

---

### 07_Resources

---

### 08_Linetest

---

### 09_Dev

---

### 10_Comunication

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
