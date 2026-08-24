# WallPaper-by-Sn

Collection de fonds d'écran pour Wallpaper Engine.

## Comment ajouter un wallpaper

1. Copie ton image (jpg/png) dans le dossier `wallpapers/`
2. Ajoute une entrée dans `wallpapers/manifest.json` :

```json
{
    "wallpapers": [
        {
            "id": "mon-wallpaper",
            "name": "Mon Wallpaper",
            "image": "wallpapers/mon-wallpaper.jpg"
        }
    ]
}
```

3. Push sur GitHub
4. Lance Wallpaper Engine - il téléchargera automatiquement le nouveau wallpaper

## Structure attendue

```
wallpapers/
├── manifest.json
├── ocean-01.jpg
├── city-night.png
└── ...
```

## Format du manifest.json

```json
{
    "wallpapers": [
        {
            "id": "identifiant-unique",
            "name": "Nom affiché",
            "image": "wallapers/fichier.jpg"
        }
    ]
}
```

- `id` : identifiant unique (utilisé pour le cache local)
- `name` : nom affiché dans l'app
- `image` : chemin relatif vers l'image dans le repo
