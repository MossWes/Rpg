# Notre JDR avec MJ IA — cahier de décisions

> Pour : Wesley et Greg · version du 2026-11-21 · rien n'est décidé.
> Coche ta réponse (remplace `[ ]` par `[x]`), ajoute un mot si tu veux, puis renvoie le fichier à Wesley.
> Les options marquées ⭐ sont le conseil de Claude, pas une décision.

## L'idée en bref

Un jeu de rôle où **le maître du jeu est une IA**. Elle raconte l'histoire, joue les personnages et surtout **met en scène** : elle choisit quand montrer la carte du monde, l'image du lieu ou le plan de combat.

Ce qui rend la partie visuelle, comme les MJ en stream (voir les captures dans `references/`) :

1. **La carte du monde** : où est le groupe. On voyage de lieu en lieu par des routes, chacune avec une durée (ex. : 2 jours à pied).
2. **L'image du lieu** : la ville, l'auberge, la forêt, pour l'ambiance.
3. **Le plan de la scène** : un plan de l'auberge avec des **jetons** pour chaque héros et adversaire, une grille de cases, et des **déplacements limités** : selon D&D, un personnage parcourt 9 m par tour, soit 6 cases de 1,5 m. Il ne peut donc pas toujours atteindre l'ennemi ni tout faire en un tour.

Chaque héros a ses **caractéristiques** (Force, Dextérité…) et ses **compétences**. Les dés décident de la réussite.

**Le principe clé** : le code applique les règles (dés, déplacements, points de vie), l'IA raconte. L'IA ne peut donc ni tricher ni oublier une règle.

### Un tour de jeu, en exemple

1. L'IA décrit : « La porte de l'auberge s'ouvre, trois brigands entrent. » → l'image de l'auberge s'affiche.
2. La tension monte → l'IA sort le plan : jetons des héros et des brigands placés.
3. Le joueur de Kaelen clique « Attaquer le chef » : le jeu montre les 6 cases atteignables, vérifie la distance, lance le dé (d20 + bonus contre la classe d'armure).
4. Le jeu donne le résultat (touché, 7 dégâts) → l'IA le raconte et fait réagir le chef.

### Ce qu'on reprend d'ailleurs

- **Règles** : D&D 5e allégée, à partir des règles libres (SRD 5.1 / 5.2, licence CC-BY 4.0 : réutilisables en citant la source). Les livres complets servent de référence, on n'en copie pas le texte.
- **aiga_** (jeu de rôle IA en ligne, analysé dans `docs/aiga/`) : mémoire de chaque personnage, traits gagnés en jouant, carnet de partie, 3 choix proposés + texte libre.
- **Pas de Warhammer ni de D&D dans le nom ou l'univers** : ce sont des marques. On crée notre monde.

## L'expérience de jeu

### 1. Qui joue, et comment ?

- [ ] **Un seul écran partagé (PC ou TV), les joueurs autour** ⭐ — Comme une vraie table : un appareil, on dit ses actions, une personne les tape. Le plus simple à construire.
- [ ] **En ligne, chacun sur son appareil** — Plus moderne, mais il faut synchroniser tout le monde en direct : bien plus de travail.
- [ ] **Solo avec le MJ IA** — Le plus simple, mais on perd le côté soirée entre amis.
- [ ] Autre : …

> Conseil de Claude : On commence par l'écran partagé : c'est l'esprit des parties des captures de référence, et ça évite la synchronisation. Le jeu en ligne viendra après.

**Commentaire Wesley :**

**Commentaire Greg :**

### 2. Sur quel appareil ?

- [ ] **Une page web pensée en paysage (PC, tablette, TV), lisible au téléphone** ⭐ — Rien à installer, marche partout.
- [ ] **Une application téléphone** — Écran trop petit pour une carte et des jetons.
- [ ] **Un logiciel PC** — À installer, moins facile à partager.
- [ ] Autre : …

> Conseil de Claude : Le plan de combat a besoin de place : le paysage s'impose. Le web évite toute installation.

**Commentaire Wesley :**

**Commentaire Greg :**

### 3. Quel univers ?

- [ ] **Notre propre monde de fantasy médiévale** ⭐ — Les règles libres de D&D sont pensées pour ça.
- [ ] **Plusieurs univers au choix (fantasy, science-fiction, moderne)** — Plus riche, mais chaque univers demande ses images et ses règles.
- [ ] **Notre propre science-fiction** — Il faudrait adapter les règles.
- [ ] Autre : …

> Conseil de Claude : Warhammer et D&D sont des marques protégées : on crée notre monde. La fantasy colle aux règles qu'on reprend.

**Commentaire Wesley :**

**Commentaire Greg :**

### 4. Durée d'une séance ?

- [ ] **30 minutes** — Une scène, idéal pour tester.
- [ ] **1 à 2 heures** ⭐ — Une soirée, une aventure courte.
- [ ] **3 heures et plus** — Campagne façon stream.
- [ ] Autre : …

> Conseil de Claude : 1 à 2 heures tient dans une soirée et garde le coût IA raisonnable.

**Commentaire Wesley :**

**Commentaire Greg :**

## Les règles

### 5. Sur quelles règles on se base ?

- [ ] **D&D 5e allégée (règles libres SRD) + les bonnes idées d'aiga_** ⭐ — Dé à 20 faces, 6 caractéristiques, compétences, classe d'armure, points de vie, avantage/désavantage. Plus : mémoire des personnages, traits gagnés en jouant, carnet de partie.
- [ ] **D&D 5e complète** — Toutes les classes et tous les sorts : très lourd à coder.
- [ ] **Un système maison simple (dé à 100)** — Rapide à faire, mais on réinvente tout.
- [ ] Autre : …

> Conseil de Claude : Les règles libres de D&D (SRD 5.1 et 5.2, licence CC-BY 4.0) peuvent être reprises légalement en citant la source. Les livres complets, non.

**Commentaire Wesley :**

**Commentaire Greg :**

### 6. Qui lance les dés ?

- [ ] **Le jeu lance, avec des dés animés à l'écran** ⭐ — Impossible de tricher, tout le monde voit le résultat.
- [ ] **Les joueurs lancent de vrais dés et tapent le résultat** — Plus de sensations à la table, plus lent.
- [ ] **Au choix de la table** — Les deux modes.
- [ ] Autre : …

> Conseil de Claude : Le code lance pour que l'IA ne puisse jamais inventer un résultat. Les vrais dés peuvent venir en option.

**Commentaire Wesley :**

**Commentaire Greg :**

### 7. Création des personnages ?

- [ ] **Personnages prêts à jouer (prétirés) pour commencer** ⭐ — On choisit parmi 4 ou 5 héros et on joue tout de suite.
- [ ] **Création guidée complète (race, classe, caractéristiques)** — Riche mais long à coder et à faire en séance.
- [ ] **L'IA crée le héros à partir d'une description** — Rapide, mais moins de contrôle.
- [ ] Autre : …

> Conseil de Claude : Les prétirés suffisent pour le premier prototype. La création complète viendra quand les règles seront stables.

**Commentaire Wesley :**

**Commentaire Greg :**

## Les cartes et les déplacements

### 8. Combien de niveaux de carte ?

- [ ] **3 niveaux : carte du monde → image du lieu → plan de la scène** ⭐ — Le monde (où on est), la ville ou la forêt (l'ambiance), le plan de l'auberge avec les jetons (l'action).
- [ ] **2 niveaux : carte du monde → plan de la scène** — Moins d'images, moins d'ambiance.
- [ ] **Juste des illustrations, sans plan** — Le plus simple, mais pas de déplacements mesurés.
- [ ] Autre : …

> Conseil de Claude : C'est exactement la vision de Wesley : on situe le groupe, on montre le lieu, puis on passe au plan quand il faut agir.

**Commentaire Wesley :**

**Commentaire Greg :**

### 9. Comment on voyage sur la carte du monde ?

- [ ] **Des routes entre les lieux, chacune avec une durée en jours** ⭐ — Ex. : Port-Brume → Valcendre, 2 jours à pied, 1 à cheval. L'IA raconte les rencontres en chemin.
- [ ] **Déplacement libre avec une distance maximale par jour** — À pied, rythme normal : environ 38 km par jour (règles D&D). Plus libre, plus dur à gérer.
- [ ] **L'IA décide des trajets** — Risque d'incohérences.
- [ ] Autre : …

> Conseil de Claude : Des routes avec une durée restent cohérentes et simples. On garde les distances de D&D pour calculer ces durées.

**Commentaire Wesley :**

**Commentaire Greg :**

### 10. Le plan de la scène : quelle grille ?

- [ ] **Des cases carrées de 1,5 m** ⭐ — La règle D&D : un personnage se déplace de 9 m par tour, soit 6 cases. Il ne peut donc pas toujours atteindre l'ennemi.
- [ ] **Des hexagones** — Plus juste pour les diagonales, plus rare en D&D.
- [ ] **Sans grille, mesure libre** — Plus joli, plus dur à calculer et à afficher.
- [ ] Autre : …

> Conseil de Claude : Les cases rendent la portée de chaque personnage visible et facile à vérifier par le code.

**Commentaire Wesley :**

**Commentaire Greg :**

### 11. Le plan vu comment ?

- [ ] **Vu de dessus** ⭐ — Comme les captures Warhammer : simple à dessiner et à calculer.
- [ ] **En perspective (isométrique)** — Comme les captures de l'auberge D&D : très beau, mais les déplacements et les images sont plus durs à faire.
- [ ] **Pas de plan** — Tout se joue dans l'imagination.
- [ ] Autre : …

> Conseil de Claude : On commence vu de dessus pour que le jeu marche. L'isométrique pourra habiller certains lieux plus tard.

**Commentaire Wesley :**

**Commentaire Greg :**

### 12. Quand le plan apparaît-il ?

- [ ] **Seulement pour les combats et les scènes tendues** ⭐ — Le reste du temps : récit et illustration.
- [ ] **Tout le temps** — Chaque lieu a son plan.
- [ ] **Jamais**
- [ ] Autre : …

> Conseil de Claude : C'est ce que font les MJ en vrai : le plan sort quand la position compte.

**Commentaire Wesley :**

**Commentaire Greg :**

## Les images

### 13. D'où viennent les images ?

- [ ] **Un mélange : cartes et plans préparés à l'avance, illustrations de scène par l'IA** ⭐ — Les plans doivent être précis (cases, murs) : on les prépare. Les ambiances peuvent être générées.
- [ ] **Tout généré par l'IA pendant la partie** — Coûte cher, lent, et un plan généré n'a pas de cases fiables.
- [ ] **Tout préparé à la main** — Beau et fiable, mais limite les aventures.
- [ ] Autre : …

> Conseil de Claude : Une image générée coûte et prend du temps ; une bibliothèque réutilisable rend le jeu rapide et cohérent.

**Commentaire Wesley :**

**Commentaire Greg :**

### 14. Quel style graphique ?

- [ ] **Dessin à l'encre et au crayon, ton sépia** ⭐ — Comme les captures de l'auberge : élégant, et il pardonne les petites incohérences des images IA.
- [ ] **Peinture réaliste** — Spectaculaire, mais le moindre défaut se voit.
- [ ] **BD / dessin animé** — Plus léger, plus familial.
- [ ] **Pixel art** — Rétro, facile à animer.
- [ ] Autre : …

> Conseil de Claude : Un seul style pour tout le jeu, sinon les images ne vont pas ensemble.

**Commentaire Wesley :**

**Commentaire Greg :**

### 15. À quoi ressemblent les jetons ?

- [ ] **Un portrait rond, entouré de la couleur du joueur** ⭐ — On reconnaît son héros d'un coup d'œil.
- [ ] **Une figurine dessinée vue de dessus** — Comme les captures Warhammer.
- [ ] **Une pastille de couleur avec une initiale** — Le plus simple.
- [ ] Autre : …

> Conseil de Claude : Le portrait sert aussi dans la barre des personnages en bas de l'écran, comme sur les captures.

**Commentaire Wesley :**

**Commentaire Greg :**

## Le MJ IA

### 16. Que fait l'IA exactement ?

- [ ] **Elle raconte et met en scène ; le code gère les règles** ⭐ — L'IA choisit le lieu, l'image, le moment où sortir le plan, joue les personnages. Le code calcule dés, déplacements, points de vie.
- [ ] **Elle raconte seulement** — La mise en scène est fixée à l'avance.
- [ ] **Elle fait tout, règles comprises** — Elle finira par se tromper ou tricher.
- [ ] Autre : …

> Conseil de Claude : C'est la demande de Wesley : un narrateur qui met les bonnes scènes au bon endroit, sans pouvoir fausser les règles.

**Commentaire Wesley :**

**Commentaire Greg :**

### 17. Comment les joueurs agissent ?

- [ ] **Texte libre + 3 choix proposés** ⭐ — On clique pour aller vite, on écrit pour être créatif.
- [ ] **Seulement des choix proposés** — Rapide mais limité.
- [ ] **Seulement du texte (ou la voix)** — Libre mais plus lent à table.
- [ ] Autre : …

> Conseil de Claude : aiga_ fait ainsi et ça marche : les deux modes se complètent.

**Commentaire Wesley :**

**Commentaire Greg :**

### 18. De quoi l'IA se souvient ?

- [ ] **Un carnet de partie + la mémoire de chaque personnage** ⭐ — Lieux visités, alliés et ennemis, promesses faites. Un aubergiste se souvient de la bagarre.
- [ ] **Un simple résumé de la partie** — Plus facile, moins vivant.
- [ ] **Rien d'une séance à l'autre**
- [ ] Autre : …

> Conseil de Claude : C'est ce qui rend aiga_ marquant, et c'est faisable par étapes.

**Commentaire Wesley :**

**Commentaire Greg :**

## Le projet

### 19. Le tout premier prototype ?

- [ ] **« Une soirée à l'auberge » : 1 ville, 1 auberge, 4 héros prétirés, 1 bagarre sur le plan** ⭐ — Teste en une fois : carte du monde, image du lieu, plan, jetons, déplacements, dés, MJ IA.
- [ ] **Une quête courte complète (voyage + donjon + boss)** — Plus ambitieux : plusieurs semaines avant de jouer.
- [ ] **Seulement la carte du monde et le voyage** — Ne teste pas le combat.
- [ ] Autre : …

> Conseil de Claude : Petit, mais il touche à tout : on saura vite si la formule plaît.

**Commentaire Wesley :**

**Commentaire Greg :**

### 20. Budget IA par mois ?

- [ ] **0 € : modèles gratuits ou sur le serveur de Wesley** — Possible, mais images et récit de moindre qualité.
- [ ] **Jusqu'à 20 € pour le prototype** ⭐ — Suffit pour tester à quelques-uns.
- [ ] **Jusqu'à 50 €** — Confortable, avec beaucoup d'images.
- [ ] **Plus**
- [ ] Autre : …

> Conseil de Claude : Le récit coûte peu ; ce sont surtout les images générées qui coûtent. On mesure pendant le prototype.

**Commentaire Wesley :**

**Commentaire Greg :**

### 21. Qui fait quoi ? (Greg : qu'est-ce qui te plairait ?)

_Ex. : l'univers et ses lieux, les scénarios, les règles, les illustrations, les tests à la table…_

**Wesley :**

**Greg :**

### 22. Un nom pour le jeu ?

_Une idée, même provisoire._

**Wesley :**

**Greg :**

### 23. Autre chose ? Une idée, une inquiétude, une référence ?

_Un jeu, un stream, une mécanique que tu aimes._

**Wesley :**

**Greg :**

---

## Pour en discuter avec Claude (version gratuite)

Ouvre https://claude.ai, nouvelle conversation, joins ce fichier, puis colle :

```
Voici le cahier de décisions d'un jeu de rôle avec maître du jeu IA que je prépare avec Wesley.
Aide-moi à répondre aux questions une par une : pour chacune, explique-moi les options simplement,
donne ton avis, puis note ma réponse. À la fin, rends-moi le fichier complet en Markdown,
avec mes cases cochées [x] et mes commentaires sur les lignes « Commentaire Greg ».
```

Renvoie ensuite le fichier à Wesley (WhatsApp, mail…).
