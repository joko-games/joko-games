# Joko Games 🎮

Petit studio, gros moteur : des jeux en Rust et des addons World of Warcraft, tous écrits par une IA
(Claude, via Claude Code) sous la direction d'un humain qui fixe le cap, relit et valide.

Cinq projets à ce jour : deux jeux, trois addons.

---

## 🕹️ Les jeux

### 🏎️ [Star Racer](https://github.com/joko-games/star-racer)

Un jeu de course multijoueur en ligne, en Rust avec [Bevy](https://bevy.org), aux graphismes
volontairement géométriques. On y joue directement dans le navigateur, ou avec le client natif pour
Windows, Linux et macOS.

- **Statut :** v1.0.0 en release candidate, le plus avancé de la bande
- **Sous le capot :** client Bevy (natif et WebAssembly), serveur WebSocket, simulation partagée,
  éditeur de circuits des joueurs

### 🌌 [Project MMO](https://github.com/joko-games/project-mmo)

Un MMO spatial en gestation. Chaque serveur est une galaxie générée de façon procédurale ; chaque
joueur y pilote une sonde qui démarre dans son propre système stellaire, et le serveur se souvient
de sa position d'une session à l'autre.

- **Statut :** v0.1.0, les premières briques
- **Sous le capot :** Rust et Bevy, un workspace `protocol` / `server` / `client`, du JSON ligne par
  ligne sur TCP le temps que le protocole se stabilise

---

## ⚔️ Les addons World of Warcraft

La gamme *Essentials* : pour WoW Retail (12.1.5), en Lua, chacun avec sa logique testée hors du jeu
et un `install.ps1` qui le pose proprement dans `Interface\AddOns`. Seulement l'essentiel, comme leur
nom l'indique.

### 🗝️ [Mythic Essentials](https://github.com/joko-games/mythic-essentials)

Une petite fenêtre pour les clés Mythique+ : le DPS du groupe aux couleurs des classes, le chrono et
la progression de la clé, et qui n'a ni flacon ni nourriture. `/mye` pour l'ouvrir.

- **Statut :** v1.0.0

### 💰 [Trading Essentials](https://github.com/joko-games/trading-essentials)

Le carnet de comptes du marchand : l'historique des ventes à l'hôtel des ventes, le stock du compte,
des statistiques, la vente rapide, une liste de courses tirée des recettes suivies, et les prix dans
les infobulles. Compatible Auctionator.

- **Statut :** premier jet, pas encore lancé dans le client

### 🗺️ [World Quest Essentials](https://github.com/joko-games/world-quest-essentials)

Toutes les expéditions de Midnight dans une liste sobre à côté de la carte du monde : recherche,
filtres par récompense, tri par colonne, et un clic pour poser le point de passage. `/wqe`.

- **Statut :** v1.0.0, vu en marche en jeu

---

## 🤖 Comment c'est fait

Tout le code et toute la documentation sont écrits par Claude. L'humain derrière Joko Games donne la
direction, teste et tranche. Chaque dépôt garde sa doc dans `docs/` et son contexte de travail dans
un `CLAUDE.md`, pour qu'une nouvelle session reprenne là où la précédente s'est arrêtée.
