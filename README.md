# Portfolio · Sarah Nouria

Site mono-page, bilingue français / anglais, publié avec GitHub Pages.
Aucun framework, aucune étape de build : le site tient dans un seul fichier.

Adresse une fois GitHub Pages activé : **https://nouria08.github.io/portfolio/**
Version anglaise directe : https://nouria08.github.io/portfolio/?lang=en

## Contenu du dépôt

| Fichier | Rôle |
| --- | --- |
| `index.html` | Le site complet : HTML, CSS et JavaScript intégrés. |
| `sarah.png` | Portrait détouré (fond transparent) affiché dans l’en-tête du site. |
| `og-image.png` | Image d’aperçu de partage (WhatsApp, LinkedIn…), 1200 × 630 px. |
| `.nojekyll` | Fichier vide qui demande à GitHub Pages de servir les fichiers tels quels, sans traitement Jekyll. |
| `README.md` | Ce mode d’emploi. |

## Placeholders à remplacer avant diffusion

Dans `index.html` (recherche avec Ctrl+F / Cmd+F) :

| Placeholder | Où | Par quoi le remplacer |
| --- | --- | --- |
| `[À COMPLÉTER]` | Études de cas, 12 fois : Contexte, Action et Résultat pour Honda Maroc et Orange Maroc, en FR et en EN | Le texte définitif. Supprimer aussi la courte indication qui suit chaque marqueur. |

Le commentaire HTML qui signale cette zone contient aussi le marqueur : il est invisible sur le site et peut rester.

## Portrait

La photo est le fichier `sarah.png` à la racine du dépôt : une version détourée sur fond transparent. Elle est posée directement sur le fond de la page, sans cadre ni ombre, recadrée en CSS sur le visage et les épaules ; ses bords bas et latéraux sont légèrement fondus pour éviter une coupe nette. Ces réglages se trouvent dans le bloc « Portrait » de la balise `<style>`.

Attention : le recadrage est calculé pour la position du buste dans le fichier `sarah.png` actuel. Si la photo est remplacée par une image cadrée autrement (même sous le même nom), le cadrage doit être recalculé ; la formule est indiquée en commentaire au-dessus de `.hero-portrait img`.

## Modifier les textes

Chaque texte existe en deux versions côte à côte, marquées `lang="fr"` et `lang="en"`. Modifier les deux. Le bouton FR / EN affiche l’une ou l’autre sans recharger la page ; le français est la langue par défaut.

## Fusionner la branche de travail dans `main`

Le site a été préparé sur la branche `claude/portfolio-sarah-nouria-dp2e26`. GitHub Pages publiera la branche `main`, il faut donc d’abord fusionner.

**Depuis le site GitHub (le plus simple)**

1. Ouvrir https://github.com/Nouria08/portfolio
2. Cliquer sur **Compare & pull request** dans le bandeau jaune. Si le bandeau n’apparaît pas : onglet **Pull requests** → **New pull request** → `base: main` et `compare: claude/portfolio-sarah-nouria-dp2e26`.
3. Cliquer sur **Create pull request**, puis **Merge pull request**, puis **Confirm merge**.

**Depuis un terminal**

```bash
git checkout main
git pull origin main
git merge claude/portfolio-sarah-nouria-dp2e26
git push origin main
```

## Activer GitHub Pages

1. Dans le dépôt, ouvrir **Settings** (onglet en haut à droite).
2. Dans le menu de gauche, section *Code and automation*, cliquer sur **Pages**.
3. Sous **Build and deployment** → **Source**, choisir **Deploy from a branch**.
4. Sous **Branch**, choisir `main`, puis le dossier `/ (root)`, et cliquer sur **Save**.
5. Patienter une à trois minutes. L’onglet **Actions** affiche le déploiement *pages build and deployment* ; quand il est vert, le site est en ligne à https://nouria08.github.io/portfolio/.

Le dépôt est public : GitHub Pages fonctionne avec un compte GitHub gratuit.
Chaque modification poussée ensuite sur `main` est republiée automatiquement.

## Vérifier l’aperçu de partage

- L’image d’aperçu n’est accessible qu’une fois le site en ligne (son adresse absolue est `https://nouria08.github.io/portfolio/og-image.png`).
- WhatsApp garde en cache l’aperçu d’un lien. Si le lien a été partagé avant la mise en ligne ou avant une modification, partager une variante comme `https://nouria08.github.io/portfolio/?v=2` pour obtenir un aperçu à jour.
- Le Débogueur de partage de Meta (https://developers.facebook.com/tools/debug/) permet de contrôler les balises lues par les réseaux sociaux.

## Aperçu en local

Ouvrir `index.html` dans un navigateur, sans installation.

