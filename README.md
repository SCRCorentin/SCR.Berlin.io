# Berlin Clubs Map (Leaflet + OSRM)

Carte interactive : recherche d'adresse, itinéraires (marche/vélo/voiture), menu "Itinéraire vers", boutons effacer/annuler, centrage sur votre position.

## Utiliser GitHub Pages

### Option 1 — Repo spécial `USERNAME.github.io`
1. Créez un dépôt public nommé **USERNAME.github.io** (remplacez USERNAME par votre pseudo GitHub).
2. Ajoutez ce fichier `index.html` à la racine, puis poussez sur `main`.
3. Ouvrez `https://USERNAME.github.io` → la carte est en ligne.

### Option 2 — N'importe quel repo + GitHub Pages (branche `gh-pages`)
Ce projet inclut un workflow GitHub Actions qui déploie automatiquement le site sur **GitHub Pages**.

1. Créez un dépôt (public ou privé).
2. Poussez le contenu (y compris `.github/workflows/pages.yml`).
3. Sur GitHub → *Settings* → *Pages* → *Build and deployment* :
   - *Source*: **GitHub Actions**
4. Poussez sur `main` → le workflow publie le site. L'URL sera du type:
   `https://USERNAME.github.io/REPO`

### Commandes Git rapides

```bash
git init
git add .
git commit -m "Init Berlin map"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

## Notes
- La géolocalisation (📍) nécessite **HTTPS** → OK avec GitHub Pages.
- Les profils OSRM: `foot` (marche), `bike` (vélo), `driving` (voiture).
- Les temps de trajet proviennent du routeur public **OSRM** (router.project-osrm.org).
