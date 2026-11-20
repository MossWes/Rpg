# Idées à reprendre pour nos jeux

> Ce qu'aiga_ fait bien, traduit en mécaniques génériques. On reprend des **idées de système**,
> jamais leurs noms, personnages, textes ou images. Rien n'est décidé : à voter.

## Les idées, de la plus simple à la plus lourde

| # | Idée | Pourquoi c'est fort | Coût pour nous |
|---|---|---|---|
| 1 | **Paliers de résultat sur un d100** (échec / presque / partiel / réussite) au lieu de réussi/raté | Un « presque » fait avancer l'histoire avec un prix, jamais de cul-de-sac | Faible : une table de seuils |
| 2 | **Traits gagnés par l'usage, en étoiles (0 à 4), qui peuvent baisser** | Le héros devient ce que le joueur fait ; bonus visible au jet | Faible à moyen |
| 3 | **Journal de bord / Game Book** : lieux visités par plage de tours, PNJ et factions en allié/neutre/hostile, objectifs par phase | Le joueur voit sa progression d'un coup d'œil | Moyen (écran dédié) |
| 4 | **Mémoire par PNJ** : une liste `tour — fait court` par personnage, relue avant chaque réponse | Effet « il se souvient de ma promesse » très marquant | Moyen : stockage + recherche par le sens (embeddings) |
| 5 | **Structure en 3 phases + finale** avec objectifs typés (histoire, mystère, faction) | Donne un fil à une IA qui sinon part dans tous les sens | Faible : c'est du contenu |
| 6 | **Collection de dés débloqués par succès** | Récompense cosmétique, zéro impact sur l'équilibre | Faible à moyen |
| 7 | **Vote de groupe** (amis ou communauté, choix majoritaire) | Jeu social sans synchroniser tout le monde | Moyen à lourd |
| 8 | **Héros à partir d'une photo, même visage partout** | Très fort pour les enfants (jouet, dessin) | Lourd : génération d'images cohérente |

## Pour Braisemont (RPG idle de ForgeLab)
Braisemont tourne déjà avec forge, quêtes, coffres, énigmes, compagnons et expéditions (voir
`MossWes/ForgeLab`, branche `claude/pixelio-rpg-webapp-yufh9g`, `docs/rpg/`). Les idées qui collent sans IA
générative :
- **#2 Traits par l'usage** : relier un trait à la régularité d'entraînement (ex. 4 séances d'affilée → +1 étoile),
  et le perdre doucement si on arrête.
- **#1 Paliers d100** pour les expéditions : un « presque » rapporte moins mais rapporte.
- **#3 Journal** : une page « mon parcours » avec régions, compagnons et phases.
- **#6 Dés / cosmétiques à collectionner** liés aux succès réels (séances, records).

Le jeu est en pause (priorité ForgeLab du 2026-11-19 : s'entraîner avec ses programmes) : ces idées
attendent la reprise.

## Pour un futur jeu narratif à nous (MJ IA)
Briques minimales, dans l'ordre :
1. Un MJ qui écrit la scène et **propose 3 choix avec niveau de risque** + saisie libre.
2. Le jet d100 avec paliers (idée #1) fait **par le code**, pas par l'IA : l'IA ne fait que raconter le résultat.
3. Un état du monde en JSON (stats, objets, relations) mis à jour à chaque tour.
4. La mémoire par PNJ (idée #4).
5. Le Game Book (idée #3) généré depuis cet état.

Point clé d'aiga_ v2 à retenir : **tout en une seule passe** (rappel des souvenirs, jugement du risque, jet,
écriture) pour répondre en 5 à 10 s au lieu de 30.
