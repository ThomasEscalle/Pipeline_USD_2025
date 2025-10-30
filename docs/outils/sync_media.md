---
icon: material/draw
---

# Plugin Prism Sync Media

## Vue d'ensemble

Le plugin **Sync Media** pour Prism permet de copier coller automatiquement les médias (images et vidéos) associés aux shots d'un projet vers des emplacements définis par l'utilisateur, en fonction de règles configurables.

Il nous sert à envoyer la dernière version d'un playblast, d'un rendu 2D ou 3D vers des dossiers spécifiques pour qu'ils se mettent a jour automatiquement dans notre logiciels de montage ou de compositing.

## Fonctionnalités principales

### 🎯 Synchronisation automatique
- Détection automatique des shots dans le projet
- Identification de la dernière version des médias
- Copie intelligente vers les destinations configurées

### 🎨 Support multi-formats
- **Images**: `.jpg`, `.jpeg`, `.JPG`, `.png`, `.PNG`, `.tif`, `.tiff`, `.tga`, `.dpx`, `.exr`, `.hdr`
- **Vidéos**: `.mp4`, `.mov`, `.avi`, `.m4v`


## Installation et activation

### Menu d'accès
Le plugin ajoute un menu **"Sync Media"** dans la barre de menu du Project Browser avec :
- Action **"Synchronize"** 
- Raccourci clavier : `Ctrl+Shift+W`

## Configuration

### Fichier de configuration

Le plugin utilise un fichier de configuration JSON situé dans :
```
{pipeline_path}/sync_media_settings.json
```

### Structure du fichier de configuration

```json
{
    "rules": [
        {
            "source_media": ["keyword1", "keyword2"],
            "destination": {
                "images_destination": "/path/to/images/@seq@_@sht@_@frames@.@ext@",
                "videos_destination": "/path/to/videos/@seq@_@sht@.@ext@"
            }
        }
    ]
}
```

### Paramètres des règles

#### `source_media`
**Type**: `string` ou `array<string>`

Mots-clés pour filtrer les sources média. Le plugin cherche ces mots-clés dans le nom des dossiers de média.

**Exemples**:
```json
"source_media": "beauty"
// ou
"source_media": ["beauty", "final"]
```

#### `destination`
**Type**: `object`

Définit les templates de destination pour les images et vidéos.

**Propriétés requises**:
- `images_destination`: Template pour les images
- `videos_destination`: Template pour les vidéos

### Variables de template

Les templates de destination supportent les variables suivantes :

| Variable | Description | Exemple |
|----------|-------------|---------|
| `@seq@` | Nom de la séquence | `seq010` |
| `@sht@` | Nom du shot | `sht010` |
| `@shot_display_name@` | Nom d'affichage complet | `seq010_sht010` |
| `@frames@` | Numéro de frame (images uniquement) | `0001` |
| `@ext@` | Extension du fichier | `jpg` |
| `@pipeline@` | Chemin du pipeline (celui setproject dans prism) | `//minerva/3D5/Uptight..` |

### Exemple de configuration complète

```json
{
    "rules": [
        {
            "source_media": ["Anim", "Publish"],
            "destination": {
                "images_destination": "@pipeline@/04_Editing/images/@seq@/@sht@/@shot_display_name@_@frames@.@ext@",
                "videos_destination": "@pipeline@/04_Editing/videos/@seq@/@shot_display_name@.@ext@"
            }
        },
        {
            "source_media": "comp",
            "destination": {
                "images_destination": "@pipeline@/04_Editing/@seq@_@sht@_comp_@frames@.@ext@",
                "videos_destination": "@pipeline@/04_Editing/@seq@_@sht@_comp.@ext@"
            }
        }
    ]
}
```

## Fonctionnement

### Arborescence explorée

Pour chaque shot, le plugin explore :
```
{shot_path}/
├── Playblasts/
│   └── {media_source}/
│       └── v{XXX}/
│           └── {files}
├── Renders/
│   ├── 2dRender/
│   │   └── {media_source}/
│   │       └── v{XXX}/
│   │           └── {files}
│   └── 3dRender/
│       └── {media_source}/
│           └── v{XXX}/
│               └── {files}
```

---

!!! tip "Conseil d'utilisation"
    Testez d'abord vos règles sur un petit sous-ensemble de shots avant de les appliquer à l'ensemble du projet.

!!! warning "Attention"
    Ce plugin écrase les fichiers existants sans confirmation. Assurez-vous de bien configurer vos chemins de destination.