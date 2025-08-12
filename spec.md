
---

## **spec.md**
```markdown
# 📑 Spécifications - VinylBeats

## 1. Objectif
Créer un lecteur musical en ligne utilisant l’API Deezer, affichant les morceaux populaires et permettant de rechercher et écouter des extraits.

---

## 2. Fonctionnalités principales
- **Lecture audio**
  - Utilisation de `Audio()` en JavaScript
  - Lecture/Pause
  - Navigation piste précédente/suivante
  - Animation du vinyle pendant la lecture

- **Affichage**
  - Grille de vinyles avec pochette, titre, artiste, album
  - Design responsive (desktop et mobile)
  - Barre de recherche

- **Données**
  - API : `https://api.deezer.com`
  - Proxy CORS : `https://corsproxy.io/`
  - Points d’accès utilisés :
    - `chart/0/tracks?limit=20` → hits du moment
    - `search?q=<query>&limit=20` → recherche personnalisée
  - Fallback en cas d’erreur : données de démonstration

---

## 3. Technologies utilisées
- **HTML5** → structure
- **CSS3** → design moderne, responsive et animations
- **JavaScript ES6** → logique applicative
- **API Deezer** → données musicales
- **Proxy CORS** → contournement des restrictions de navigateur

---

## 4. Structure des fichiers
/vinylbeats
│── index.html → Page principale
│── style.css → Styles (peut être intégré dans HTML)
│── script.js → Code JavaScript (peut être intégré dans HTML)
│── README.md → Guide d’installation et utilisation
│── spec.md → Spécifications techniques et fonctionnelles

---

## 5. Scénario utilisateur
1. L’utilisateur ouvre l’application → les hits Deezer sont chargés.
2. Il clique sur un vinyle → le morceau démarre et le disque tourne.
3. Il peut mettre en pause, passer au suivant ou revenir en arrière.
4. Il tape un artiste dans la recherche → la grille se met à jour.

---

## 6. Contraintes
- Les extraits sont limités à 30 secondes.
- L’application doit rester responsive.
- L’API Deezer est publique mais nécessite un proxy CORS côté client.

---

## 7. Améliorations futures
- Ajout de playlists
- Lecture complète via OAuth Deezer
- Système de favoris
- Mode hors-ligne avec cache..
