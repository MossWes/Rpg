# aiga_ — présentation

> Relevé le 2026-11-20 sur https://www.aiga.io et https://feedback.aiga.io/changelog/aigav2-is-here.

## En une phrase
Plateforme de jeux de rôle textuels : on crée un monde à partir d'une courte description (ou on joue
dans celui d'un autre), et un **maître du jeu IA** raconte chaque scène, l'illustre et se souvient de
ce que le joueur fait.

Slogan : « AI RPG Games That Remember Your Choices ».

## Fiche
| Élément | Valeur |
|---|---|
| Nom | aiga_ (avec le tiret bas) |
| Éditeur | AI Worx Ltd |
| Site | https://www.aiga.io |
| Retours / changelog | https://feedback.aiga.io (Featurebase) |
| Réseaux | X / Twitter `@aiga_io` · Discord : https://www.aiga.io/discord |
| Couleur de marque | vert fluo `#24FF00` |
| Technique visible | site Next.js, images stockées sur Google Cloud Storage (bucket `ai-game-agent`) |
| Version | v2, moteur **ECHOES**, en ligne depuis le 2026-10-12 |

## Modèle économique
- **Compte gratuit : 4 tours par jour.**
- Les offres payantes ne sont pas détaillées sur la page d'accueil (page tarifs non lue, voir `../sources.md`).

## Modes de jeu (types de monde)
Les mondes partagés portent une étiquette de mode :
- **RPG** (icône cheval) : aventure ouverte classique.
- **Objective / Single Objective** (icône étoile) : un but unique à atteindre.
- **Kingpin** : mode « monter en puissance » (empire, territoire, ascension).
- **Story / Interactive Story** (icône masques) : récit interactif plus guidé.

## Façons de jouer
| Mode | Comment ça marche |
|---|---|
| Solo | Une histoire à soi, à son rythme ; elle attend le retour du joueur. |
| Entre amis | Plusieurs joueurs dans une histoire ; chacun envoie son action, le MJ les joue toutes dans une seule scène (minuteur visible, ex. 12 s). |
| Tout le monde | Parties ouvertes : la communauté vote, le choix le plus populaire devient l'histoire (ex. 1 248 votants). |
| Discord | Un bot aiga_ poste les scènes dans un salon ; les membres votent avec des boutons. |

Saisie : texte libre (280 caractères max), `@` pour viser un personnage, `#` pour un objet, ou choix
proposés avec leur niveau de risque (« High risk », « Med risk »).

## Langues et styles
- 16 langues selon le changelog (le sélecteur de la page d'accueil en montre 12, dont le français).
- **12 styles graphiques** pour les illustrations. Vus dans les liens : `korean-manhwa`, `unfiltered-reality`,
  `neon-cyberpunk`, `cinematic-storybook`, `rendered-realism`, `pixel-art`, `retro-3d`, `anime`,
  `classic-cartoon` (9 sur 12 ; les 3 autres non relevés).
