# HarmonyLab 🎛️

> Outil de théorie musicale et de production — 100% offline, aucune installation requise.

**[→ Ouvrir HarmonyLab](https://jeremdelrieux-afk.github.io/Music-Tool/)**

---

## À propos

HarmonyLab est un outil de production musicale et de théorie harmonique développé en collaboration avec [Claude](https://claude.ai) (Anthropic). L'ensemble du code HTML, CSS et JavaScript a été écrit et itéré via des sessions de pair-programming avec Claude, à partir des besoins et du workflow d'un producteur de DnB, Neurofunk et Hi-Tek Minimal.

---

## Fonctionnalités

### 🎵 Harmonie

**Gamme & Accords**
- Sélection de tonique (12 notes) et de mode (Mineur naturel, Majeur, Dorien, Phrygien, Lydien, Mixolydien, Mineur harmonique, Mineur mélodique, Locrien)
- Clavier interactif avec notes affichées sur toutes les touches — couleurs par rôle (gamme, accord, tonique, hors gamme)
- Guide mélodie : notes classées par tension harmonique (stable / couleur / tension) sur l'accord sélectionné
- Accords empruntés (mode parallèle, mineur harmonique, napolitain)
- Suites d'accords par genre (DnB, Hi-Tek Techno Minimal, Death Metal, Dorien)
- Lecture audio des accords et des notes au clic
- Export MIDI par accord individuel

**Arpégiateur**
- Vitesse synchronisée au BPM (1/4, 1/8, 1/16, 1/8T)
- Sens : montant, descendant, alterné, aléatoire — 1 à 3 octaves
- Export MIDI du pattern arpégé

**Cercle des Quintes**
- Visualisation SVG interactive — clic pour naviguer vers une tonalité
- Surbrillance automatique de la relative mineure/majeure
- Modulations : notes communes et notes qui changent par destination
- Relations modales : relative, parallèle
- Accords pivot entre tonalités adjacentes

**Compatibilité harmonique**
- Score de compatibilité en % entre deux tonalités
- Notes communes, notes exclusives, accords pivot communs

---

### ⏱️ Tempo & Rythme
- BPM global éditable depuis le header (boutons +/- ou clic direct)
- Tap Tempo (bouton ou barre espace)
- Tableau de subdivisions (ronde → triple croche, pointées, triolets) en ms
- Référentiel de genres par BPM avec mise en surbrillance automatique

---

### 🎚️ FX Studio

**Delay** — temps synchronisé BPM, ping-pong offset, feedback, référence types de delay

**Reverb** — pre-delay et RT60 par type, pré-delay BPM sync (1/32, 1/16, 1/8), guide wet par instrument

**Compresseur** — timings attack/release BPM sync, presets par usage (sidechain, kick, bus basses, bus drums, voix)

**Saturation** — 5 types (Tape, Tube, Hard Clip, Transformer, Bitcrusher), guide drive et positionnement dans la chaîne

**Sidechain Pumping** — attack/release BPM sync par genre (DnB, Neurofunk, Techno, Hi-Tek Minimal, House, Trance), routing FL Studio et alternative recommandée

---

### 🔊 Sound Design

**Fréquences des notes** — tableau Hz et période par note et octave (0-8), diapason A4 réglable, zones spectrales

**Harmoniques & conflits** — calcul des harmoniques de la basse et du kick, détection des conflits fréquentiels, solutions proposées

**Transposition de sample** — note source → note cible, micro-tuning (désaccordage initial en cents), recommandation d'algorithme FL Studio par type de contenu, mapping gamme après transposition

---

### 🎹 Synthèse

**Mini Synthé jouable**
- OSC (Sine/Saw/Square/Triangle), octave ±2, détune
- Filter (LP/HP/BP/Notch), cutoff, resonance, drive
- Enveloppe ADSR avec sync au BPM
- LFO avec forme d'onde, rate, depth et destination (filtre/pitch/volume) — sync au BPM
- Clavier jouable synchronisé à la gamme et tonalité courantes
- Play continu avec mise à jour des paramètres en temps réel
- Visualiseur de signal (oscilloscope)

**Signal Flow** — modules OSC → FILTER → ENV → LFO → VCA cliquables avec explications et correspondances Serum 2

**LFO & Modulation** — visualiseur de formes d'onde, tableau Hz/BPM sync, sources et destinations dans Serum 2

---

### 🛠️ Outils
- Export MIDI de tous les accords de la gamme courante
- Export MIDI de l'arpège courant
- Synchronisation globale : tous les outils suivent la tonalité et le BPM courants

---

## Tips interactifs
- Icône `?` à côté de chaque section — survolez pour afficher l'explication contextuelle

---

## Stack
- HTML / CSS / JavaScript vanilla — zéro dépendance, zéro framework
- Polices embarquées en base64 (Syne, JetBrains Mono, DM Sans) — fonctionne 100% offline
- Web Audio API pour la lecture audio et le mini synthé
- Compatible PC, mobile et tablette

---

## Développement

Ce projet a été entièrement développé en pair-programming avec **Claude** (Anthropic) — de la conception de l'architecture à l'écriture du code, en passant par le débogage et les itérations UX. Les sessions de développement ont eu lieu sur [claude.ai](https://claude.ai).

---

## Usage

```
https://jeremdelrieux-afk.github.io/Music-Tool/
```

Ou téléchargez `index.html` et double-cliquez — fonctionne sans connexion internet.

---

*Projet personnel — usage libre*
