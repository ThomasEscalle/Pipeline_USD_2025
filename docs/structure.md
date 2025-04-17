# Structure

## Structure du projet

La structure du projet est organisée de manière à faciliter la gestion des fichiers et des versions. Chaque dossier correspond à une étape spécifique du pipeline de production. Voici un aperçu de la structure du projet :

### Version simplifiée :

```tree

<nom du projet>
├── 00_Pipeline
├── 01_Management
├── 02_PreProd
├── 03_Production
├── 04_PostProd
├── 05_Editing
├── 06_USD
├── 07_Archive
├── 08_Linetest
├── 09_Dev
└── 10_Prints

```

### Version détaillée

```tree

<nom du projet>
├── 00_Pipeline/
├── 01_Management/
├── 02_PreProd/
│   ├── 01_Scenario/
│   ├── 02_Storyboard/
│   ├── 03_Concept/
|   |    ├── 01_Mood/
|   |    ├── 02_Chara/
|   |    |    └── <nom du personnage>/
|   |    |         ├── attitude_expression/
|   |    |         └── turn/
|   |    ├── 03_Enviro/
|   |    └── 04_Props/
|   ├── 04_Keyshot/
│   ├── 05_Color Script/
│   └── 06_Cinematography/
├── 03_Production/
├── 04_PostProd/
├── 05_Editing/
├── 06_USD/
├── 07_Archive/
├── 08_Linetest/
├── 09_Dev/
└── 10_Prints/



```


## Description des dossiers

### 00_Pipeline

Ce dossier est utilisé pour stocker les fichiers de **configuration du pipeline**. Il n'y a pas a toucher a quoi que ce soit dans ce dossier. Il est géré automatiquement par le gestionnaire de pipeline (Prism dans notre cas).

### 01_Management

Ce dossier sert a tout ce qui est **gestion de projet**. Il contient les racourcis vers les documents de gestion de production.

### 02_PreProd

Ce dossier est utilisé pour stocker les fichiers de **pré-production**. Il contient les concepts arts, les storyboards, les animatics, les références, les moodboards, etc. Il est divisé en plusieurs sous-dossiers ayant chacun une fonction précise.