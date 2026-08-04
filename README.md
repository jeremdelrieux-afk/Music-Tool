# HarmonyLab 🎛️

> Outil de théorie musicale et de production — 100% offline, aucune installation requise.

**[→ Ouvrir HarmonyLab](https://jeremdelrieux-afk.github.io/Music-Tool/)**

---

## Fonctionnalités

### 🎵 Harmonie

**Gamme & Accords**
- Sélection de tonique (12 notes) et de mode (Mineur naturel, Majeur, Dorien, Phrygien, Lydien, Mixolydien, Mineur harmonique, Mineur mélodique, Phrygien dominant, Locrien)
- Clavier interactif : notes de la gamme en bleu, accord sélectionné en violet, tonique en orange, hors gamme en sombre
- Notes affichées sur toutes les touches du clavier
- Guide mélodie : notes classées par tension harmonique (stable / couleur / tension) sur l'accord sélectionné
- Accords empruntés (mode parallèle, mineur harmonique, napolitain)
- Suites d'accords par genre (DnB, Hi-Tek Techno Minimal, Death Metal, Dorien)
- Lecture audio des accords et des notes au clic
- Export MIDI par accord individuel (bouton ⬇ sur chaque ligne)

**Arpégiateur**
- Vitesse synchronisée au BPM (1/4, 1/8, 1/16, 1/8T)
- Sens : montant, descendant, alterné, aléatoire
- 1 à 3 octaves
- Play / Stop
- Export MIDI du pattern arpégé

**Cercle des Quintes**
- Visualisation SVG interactive — clic pour naviguer vers une tonalité
- Surbrillance automatique de la relative mineure/majeure
- Panel modulations : notes communes et notes qui changent par destination
- Relations modales : relative, parallèle
- Détection d'accords pivot entre tonalités adjacentes
- Responsive mobile

**Compatibilité harmonique**
- Comparaison de deux tonalités avec score de compatibilité en %
- Notes communes, notes exclusives à chaque tonalité
- Accords pivot communs aux deux tonalités

---

### ⏱️ Tempo & Rythme
- Calculateur BPM avec slider et saisie manuelle
- Tap Tempo (bouton ou barre espace)
- Tableau de subdivisions (ronde → triple croche, pointées, triolets) en ms
- Référentiel de genres par BPM (DnB, Neurofunk, Hi-Tek Minimal, Techno, House, Trance, Death Metal) avec mise en surbrillance automatique selon le BPM courant

---

### 🎚️ FX Studio

**Delay**
- 8 subdivisions disponibles (1/4, 1/8, 1/16, 1/4., 1/8., 1/4T, 1/8T, 1/2)
- Temps de delay et ping-pong offset en ms synchronisés au BPM
- Feedback : calcul du nombre de répétitions audibles et durée de décroissance totale
- Tableau de référence par type de delay (Slapback, Echo, Ping-Pong, Tape, Chorus)

**Reverb**
- Pre-delay et RT60 par type (Room, Hall, Plate, Spring, Chamber, Ambience)
- Pre-delay BPM sync (1/32, 1/16, 1/8)
- Guide mix wet par instrument

**Compresseur**
- Timings attack/release synchronisés BPM pour chaque subdivision
- Presets par usage (sidechain, kick, bus basses, bus drums, voix)

**Saturation**
- 5 types : Tape, Tube, Hard Clip, Transformer, Bitcrusher
- Guide comportement par niveau de drive
- Guide positionnement dans la chaîne (avant EQ, après EQ, parallèle)

**Sidechain Pumping**
- Valeurs d'attack et release synchronisées au BPM par genre
- 6 genres : Drum & Bass, Neurofunk, Techno, Hi-Tek Minimal, House, Trance
- Ratio, threshold, knee et routing FL Studio par genre
- Alternative recommandée pour chaque genre

---

### 🔊 Sound Design

**Fréquences des notes**
- Tableau Hz et période (ms) pour chaque note, octave 0 à 8
- Diapason A4 réglable (440 Hz standard)
- Boutons copie rapide sur chaque fréquence
- Zones spectrales (Sub, Basse, Bas-médium, Médium, Présence, Air)

**Harmoniques & conflits**
- Calcul des harmoniques et sous-harmoniques de la basse fondamentale
- Détection des conflits fréquentiels avec le kick
- Identification de la note correspondante et des cents d'écart
- Solutions proposées : transposition ou notch EQ

**Transposition de sample**
- Note source → note cible : calcul en demi-tons, cents, ratio fréquentiel
- Champ désaccordage initial en cents (micro-tuning)
- Recommandation d'algorithme FL Studio par type de contenu (Drums, Basse, Mélodique mono, Polyphonique, Voix)
- Correction de formants : quand l'activer selon l'amplitude du shift
- Mapping des notes de la gamme après transposition

---

### 🛠️ Outils
- Export MIDI de tous les accords de la gamme courante
- Export MIDI de l'arpège courant
- Synchronisation globale : tous les outils suivent la tonalité et le BPM courants

---

## Tips interactifs
- Icône `?` à côté de chaque section — survolez pour afficher l'explication contextuelle
- Infobulles inline, sans positionnement flottant

---

## Stack
- HTML / CSS / JavaScript vanilla — zéro dépendance, zéro framework
- Polices embarquées en base64 (Syne, JetBrains Mono, DM Sans) — fonctionne 100% offline
- Web Audio API pour la lecture audio native
- Compatible PC, mobile et tablette

---

## Usage

Ouvrir directement dans le navigateur :
```
https://jeremdelrieux-afk.github.io/Music-Tool/
```

Ou télécharger `index.html` et double-cliquer — fonctionne sans connexion internet.

---

*Projet personnel — usage libre*
