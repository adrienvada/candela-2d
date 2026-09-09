# candela-2d — le site

La page de **Candela**, servie par GitHub Pages sur https://adrienvada.fr/candela-2d/

## ⚠️ Ce dépôt est GÉNÉRÉ. Ne pas l'éditer à la main.

`index.html` et `images/` sont produits par l'assembleur qui vit dans le dépôt du
jeu, à `tools/site/` :

```bash
cd tools/site && python3 assembler.py --fichiers /chemin/vers/candela-2d-site
```

Une retouche faite ici serait écrasée à la génération suivante, sans prévenir.
**La source est `tools/site/candela.tpl.html`**, dans
[Candela-2D---Godot](https://github.com/adrienvada/Candela-2D---Godot).

## Pourquoi un dépôt séparé du jeu

Trois raisons, et la première est la seule qui compte vraiment.

1. **`update_manager.gd` porte l'URL du dépôt de jeu en dur.** Renommer
   `Candela-2D---Godot` en `candela-2d` pour obtenir la bonne adresse de page
   ferait dépendre la mise à jour automatique de **tous les builds déjà
   installés** d'une redirection GitHub, indéfiniment.
2. La racine du dépôt de jeu est plate par conception : un `index.html` y
   atterrirait entre `player.gd` et `game_state.gd`, et Godot le scannerait
   comme une ressource.
3. Le nom du dépôt EST l'adresse : `candela-2d` donne `adrienvada.fr/candela-2d/`.

## Les liens de téléchargement

Ils pointent vers `releases/latest/download/` du dépôt de jeu : **ils suivent
les sorties sans que cette page change**. Seul le tampon de version affiché est
écrit en dur, et il porte sa date — un numéro daté vieillit honnêtement.
