# 🍄 Super Mario — Édition DeepSeek

[English](README.md) | [Українська](README.UA.md) | [Русский](README.RU.md) | [Deutsch](README.DE.md) | **Français** | [Português](README.PT.md)

Un jeu de plateforme expérimental dans le style de Super Mario, tenu dans **un seul fichier HTML**, créé avec le chat IA **DeepSeek**. Pas de framework, pas de compilation — ouvrez simplement le fichier dans un navigateur et jouez.

> 🤖 **À propos de l'expérience :** le jeu entier (HTML + CSS + JavaScript, ~1 770 lignes) a été généré lors d'une conversation avec DeepSeek, puis affiné. Il est publié comme exemple de développement de jeux assisté par IA. Le journal complet de la conversation (`log.txt`) reste hors du dépôt.

## ▶️ Comment jouer

1. Téléchargez ou clonez ce dépôt.
2. Ouvrez l'un des deux fichiers du jeu dans n'importe quel navigateur moderne (Chrome, Firefox, Safari, Edge) :
   — `SuperMarioDeepSeek.html` — l'expérience originale ;
   — `SuperMarioOMP.html` — l'édition étendue OMP Edition (voir « Variantes du jeu »).
3. Entrez votre nom de joueur — et c'est parti !

Pas de serveur, pas d'installation, pas de dépendances.

## 🎮 Commandes

| Action | Clavier | Bouton à l'écran |
|---|---|---|
| Démarrer / Pause | `Espace` | ▶ Démarrer / Pause |
| Aller à gauche | `←` | ◀ Gauche |
| Aller à droite | `→` | Droite ▶ |
| Sauter | `↑` | ⤒ Saut |
| Se baisser (passer sous les obstacles) | `↓` | ⤓ Se baisser |
| Recommencer la manche | `Échap` | ⟲ Recommencer |

Le déplacement est à inertie : Mario accélère tant que vous maintenez la direction et freine d'abord au changement de sens — la sensation classique.

## 🕹️ Déroulement du jeu

- Le parcours avec obstacles, fosses et bonus est généré au début de chaque manche.
- Ramassez les bonus : 🍒 cerise — **1 point**, 🍎 pomme — **2 points**, 🍯 miel — **3 points**.
- Un bonus raté ? Vous pouvez faire demi-tour pour le prendre.
- Tomber dans une fosse coûte **1 vie sur 3** ❤❤❤ — la manche recommence. Perdez les trois et la partie repart de zéro.
- Atteignez l'arrivée et gagnez un bonus de **10 points × vies restantes**.

## 🏆 Tableau des scores et historique

- Le score courant s'affiche au-dessus du classement.
- Le **classement du top 10** reste trié, le meilleur score en tête (rang, nom, meilleur score).
- Quand votre score entre au classement, l'entrée au plus faible score sort.
- Les **10 dernières parties** sont affichées dans une liste séparée.
- Tout est sauvegardé dans le `localStorage` du navigateur : votre historique sera encore là la prochaine fois.

> Remarque : la langue de l'interface du jeu est le russe.

## 🛠️ Technique

- Un seul fichier autonome : HTML + CSS + JavaScript.
- Rendu sur un `<canvas>` HTML5 (900 × 400).
- Persistance via `localStorage`.
- Les sprites des bonus sont dessinés par code — aucune image.

## 📦 Variantes du jeu

| Fichier | Description |
|---|---|
| `SuperMarioDeepSeek.html` | L'expérience originale : une manche générée, des bonus, des vies, un classement top 10. |
| `SuperMarioOMP.html` | **OMP Edition** — 3 niveaux thématiques (collines vertes → désert au coucher du soleil → nuit enneigée), ennemis goombas à écraser, pièces, power-ups (⭐ étoile d'invincibilité, 🍄 champignon vie supplémentaire, 🧲 aimant à bonus), trampolines, plateformes mobiles, multiplicateur de combo ×2…×5, sons et musique chiptune (Web Audio), fonds en parallaxe, particules et tremblement d'écran. Classement séparé. |

D'autres variantes du jeu sont toujours prévues.

## ⚖️ Licence

Publié sous la [licence MIT](LICENSE) — utilisation, copie, modification et redistribution gratuites.

**Avertissement :** projet de fan non commercial, sans lien avec Nintendo ni validé par elle. Toutes les marques liées à Mario appartiennent à leurs propriétaires respectifs.
