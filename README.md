# HarmonyLab 🎛️

> Outil de théorie musicale et de production — 100% offline, aucune installation requise.

**[→ Ouvrir HarmonyLab](https://jeremdelrieux-afk.github.io/Music-Tool/)**

---

## Fonctionnalités

### 🎵 Gamme et Accords
- Sélection de tonique (12 notes) et de mode (Mineur naturel, Majeur, Dorien, Phrygien, Lydien, Mixolydien, Mineur harmonique, Mineur mélodique, Phrygien dominant, Locrien)
- Affichage des 7 accords diatoniques avec fonction harmonique et notes composantes
- Clavier interactif : notes de la gamme en bleu, accord sélectionné en jaune
- Guide mélodie : notes classées par couleur harmonique (stable / couleur / tension)
- Accords empruntés (mode parallèle, mineur harmonique, napolitain)
- Explication tonique vs fondamentale (concept harmonique vs acoustique)
- Lecture audio des accords au clic

### 🔄 Cercle des Quintes
- Visualisation SVG interactive — clic pour naviguer vers une tonalité
- Anneau extérieur : majeur / Anneau intérieur : mineur relatif
- Panel modulations : notes communes, notes qui changent, distance en quintes
- Relations modales : relative majeure, parallèle, échange modal dorien
- Accords pivot communs entre tonalités adjacentes

### ⏱️ BPM et Studio
- Calculateur de delay synchronisé BPM (10 subdivisions : 1/1 à 1/32, pointées, triolets)
- Feedback delay : calcul du nombre de répétitions audibles et durée de décroissance
- Tableau reverb : pre-delay et RT60 par type (Room, Hall, Plate, Spring, Chamber, Ambience)
- Timings compresseur synchronisés BPM (attack/release en ms par subdivision)
- Guide saturation : Tape, Tube, Hard Clip, Transformer, Bitcrusher — comportement par niveau de drive

### 🎚️ Transposition
- Calculateur de pitch shift : note source → note cible
- Résultats : demi-tons, cents, ratio de fréquence, changement de vitesse
- Recommandation d'algorithme FL Studio par type de contenu (Drums, Basse, Mélodique mono, Polyphonique, Voix)
- Correction de formants : quand l'activer selon l'amplitude du shift
- Mapping des notes de la gamme après transposition

---

## Stack

- HTML / CSS / JavaScript vanilla — zéro dépendance, zéro framework
- Fonctionne entièrement dans le navigateur (offline après premier chargement)
- Compatible PC et mobile

---

## Usage

Ouvrir directement dans le navigateur :
```
https://jeremdelrieux-afk.github.io/Music-Tool/
```

Ou télécharger `index.html` et double-cliquer — fonctionne sans connexion internet.

---

## Auteur

**Jérémy Delrieux** — Producteur DnB / Neurofunk / Hi-Tech Minimal  
Projet personnel — usage libre
