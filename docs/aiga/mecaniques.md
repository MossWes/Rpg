# aiga_ — les mécaniques

> Les 6 piliers mis en avant sur la page d'accueil (relevé 2026-11-20), complétés par le changelog v2.

## 1. Récit dynamique (Dynamic Storytelling)
- Aventure textuelle **sans chemin fixe** : le joueur tape ce qu'il fait ou dit, le MJ écrit la suite.
- Les personnages répondent, les **stats et objets changent**, l'histoire suit le choix fait.
- Chaque tour affiche un **titre de scène**, le lieu, le jour et l'heure, une ambiance
  (ex. « Grimjaw's forge · Day 1 · dusk · coal smoke, snow at the door »).
- Les échanges d'objets s'affichent (objet donné →, objet reçu ←) ainsi que les variations de relation
  (« Grimjaw Trust »).

## 2. Mémoire longue (Long-Term Memory)
- **Chaque personnage a sa propre mémoire** du joueur. Une promesse au tour 1 peut ressortir au tour 132.
- Les personnages ne savent que ce qu'ils ont vu ou ce qu'on leur a dit.
- En v2 : plus de limite de « quelques dizaines de faits » ; tout moment important est gardé et
  **recherché par le sens** (recherche sémantique), pour faire remonter le bon souvenir au bon moment.
- La démo montre un PNJ avec **614 souvenirs** listés par tour.

## 3. Traits gagnés (Earned Traits)
- Le héros gagne des traits par ce qu'il fait (ex. courir sur les toits → « Rooftop Runner »).
- Progression en **étoiles (jusqu'à 4)** : Learning → Earned → +1 étoile… ; une action contraire
  (une mauvaise chute) **retire une étoile** ; à force d'agir contre, le trait disparaît.
- Un grand moment peut changer le héros d'un coup (malédiction, récompense).
- Les traits **ajoutent un bonus aux jets** : de +5 à +10 selon le niveau dans la démo,
  **jusqu'à +22** pour un trait maîtrisé (v2). Le jeu montre quels traits ont aidé.

## 4. Risque réel (Meaningful Risk)
- Choix entre action risquée (plus grosse récompense) et action sûre.
- **Jet de dé d100 visible**, en 3D plein écran ; les traits s'ajoutent ; l'histoire repart du résultat.
- Niveaux de risque affichés : faible / moyen / élevé.

Paliers relevés dans la démo (colonne « sans trait » et « avec un trait +10 ») :

| Résultat | Sans bonus | Avec +10 |
|---|---|---|
| Échec (Fail) | 0–19 | 0–9 |
| Presque (Near Miss) | 20–54 | 10–44 |
| Réussite partielle | 55–79 | 45–69 |
| Réussite | 80+ | 70+ |

Exemple : « Cross the failing skybridge », risque élevé, jet 75 + Rooftop Runner +10 → Réussite.

## 5. Continuité de l'image (Image Continuity)
- On **envoie une photo, un dessin ou un jouet** ; aiga_ en fait le héros et dessine **le même visage**
  dans chaque scène et dans chacun des 12 styles graphiques.

## 6. Livre de jeu vivant (Living Game Book)
Chaque partie tient un livre consultable à côté de l'histoire :
- **Toi** : héros, portrait, traits (ex. Shadowborn, Quick-Witted, Night Walker).
- **Parcours** : phases (Phase 1, Phase 2 « en cours », Finale) avec objectifs typés :
  *Story Goal*, *Solve Mystery*, *Faction Standing*.
- **Lieux** : lieu actuel, qui est avec toi, lieux précédents avec la plage de tours (ex. tours 9–27).
- **Personnages** : classés **Allié / Neutre / Hostile**, avec leur rôle (maire, courtier en informations…).
- **Factions** : même classement, avec leur mission
  (ex. « Contrôler toutes les routes commerciales par la force »).

## Création de monde
- Une courte description suffit (« A kingdom where heroes rise to face legendary dragons »)
  + tags de genre, de ton et de difficulté (ex. Epic · Fantasy · Medium).
- Le générateur produit : étapes, jalons, lieux, personnages, factions, et un découpage en
  **3 phases + une finale**.
- Fiche personnage : rôle, attitude (Neutre…), jalon lié (« gagner la confiance du forgeron »),
  stats chiffrées (ex. Force 74), objets.
- Le créateur peut réécrire tout personnage, dessiner chaque lieu, choisir où tout se termine, définir les quêtes,
  puis **publier** dans les mondes partagés. Détail de l'éditeur v2 : `moteur-echoes-v2.md`.
