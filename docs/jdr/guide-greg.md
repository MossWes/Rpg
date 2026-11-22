# Guide pour Greg : rejoindre le projet JDR sur GitHub

> Écrit pour toi, Greg, le 2026-11-22. Durée : 15 minutes la première fois, puis 2 minutes à chaque fois.
> Tu peux tout faire depuis ton téléphone.
> Si tu bloques : colle ce fichier dans ton Claude avec le texte de la section 7, il t'expliquera chaque étape.

## Pourquoi GitHub ?
Wesley et toi avez chacun votre Claude, mais deux comptes Claude ne peuvent pas partager une conversation.
Il faut donc **un endroit commun**. Ce sera le dépôt GitHub `MossWes/Rpg` : un dossier en ligne qui contient
tous les documents du jeu (décisions, règles, univers, plus tard le code), avec l'historique de chaque changement.

Ce que tu y feras :
- **lire** les documents à jour ;
- **poser une question ou donner ton avis** dans un « ticket » (on dit *Issue*) : Wesley et Claude te répondent dedans ;
- **corriger un document** directement, si tu veux.

Rien à installer sur un ordinateur. Rien à payer.

---

## 1. Créer ton compte GitHub (5 min)
1. Ouvre https://github.com/signup
2. Entre ton adresse mail, choisis un mot de passe, puis un **nom d'utilisateur** (ex. : `lsykenn`).
   Ce nom sera visible par Wesley : choisis-en un que tu reconnais.
3. Recopie le code que GitHub t'envoie par mail.
4. Si GitHub te propose une offre payante : choisis **Free** (gratuit). Tu peux passer les questions de bienvenue.
5. **Envoie ton nom d'utilisateur à Wesley** (WhatsApp). Il en a besoin pour t'inviter.

Conseillé : installe l'application **GitHub** sur ton téléphone (App Store ou Play Store) et connecte-toi.
Tu recevras les notifications quand quelqu'un te répond.

## 2. Accepter l'invitation de Wesley (1 min)
Une fois que Wesley t'a invité :
1. Ouvre le mail « invited you to collaborate on MossWes/Rpg », ou va directement sur
   https://github.com/MossWes/Rpg/invitations
2. Touche **Accept invitation**.
3. Tu arrives sur le dépôt : https://github.com/MossWes/Rpg

Si le lien affiche « 404 », c'est que l'invitation n'est pas encore partie, ou que tu n'es pas connecté au bon compte.

## 3. Lire les documents (2 min)
Sur https://github.com/MossWes/Rpg :
- Le texte sous la liste des fichiers est le **README** : le sommaire du dépôt.
- Le jeu est dans le dossier **`docs/jdr/`**. Les fichiers importants :

| Fichier | Ce que c'est |
|---|---|
| `cahier-de-decisions.md` | L'idée du jeu et les 23 premières questions |
| `reponses-2026-11-22.md` | Tes réponses, celles de Wesley, ce qui est décidé et ce qui reste à trancher |
| `tour-2.md` | Les 12 questions du tour 2 |
| `guide-greg.md` | Ce guide |

Touche un fichier pour le lire. Sur téléphone, si le texte est petit, tourne l'écran.

## 4. Poser une question ou répondre : les Issues (le plus important)
Une **Issue** est un fil de discussion sur un sujet. Une Issue = un sujet (« Le style graphique », « Le mode décalé »…).

**Ouvrir une nouvelle Issue :**
1. Va sur https://github.com/MossWes/Rpg/issues/new
2. **Title** : le sujet en quelques mots (ex. : `Idée : les PNJ ont des horaires`).
3. **Description** : ton idée, ta question ou ta réponse. Tu peux coller du texte venant de ton Claude.
4. Touche **Submit new issue** (ou **Create**).

**Répondre dans une Issue existante :**
1. Va sur https://github.com/MossWes/Rpg/issues
2. Touche l'Issue, écris en bas dans **Add a comment**, puis **Comment**.

**Pour appeler quelqu'un** dans un message : écris `@` suivi de son nom GitHub (Wesley est `@MossWes`). Il reçoit une notification.

Quand un sujet est réglé, Wesley ferme l'Issue. Elle reste lisible dans l'onglet *Closed*.

## 5. Corriger un document directement (facultatif)
1. Ouvre le fichier sur GitHub.
2. Touche l'icône **crayon** (« Edit this file »). Sur téléphone, elle peut être dans le menu `…`.
3. Modifie le texte.
4. Touche **Commit changes…**, écris en une ligne ce que tu as changé, puis **Commit changes**.

Pas de panique : chaque version est gardée, on peut toujours revenir en arrière.
Pour un gros changement, préfère une Issue : on en discute d'abord.

## 6. Le rythme de travail entre nous
1. **Wesley** a la vision et décide en dernier.
2. **Toi** : tu testes et tu vérifies que l'univers tient la route.
3. **Claude** (côté Wesley) écrit les documents et le code, lit tes Issues et y répond.
4. Une décision prise → elle est écrite dans un fichier du dépôt. Si ce n'est pas dans le dépôt, ce n'est pas décidé.
5. Tu reçois une notification quand on te répond (application GitHub ou mail).

**Ta première mission :** ouvre une Issue `Tour 2 — réponses de Greg` et colle tes réponses aux 12 questions de `tour-2.md`.

## 7. Te faire aider par ton Claude
Claude ne peut pas lire le dépôt tout seul (il est privé). Il faut lui donner le texte :
1. Ouvre le fichier sur GitHub, touche **Raw** (le texte brut s'affiche), sélectionne tout et copie.
   Ou télécharge le fichier et joins-le dans Claude avec le trombone.
2. Ouvre https://claude.ai, nouvelle conversation, colle le texte ou joins le fichier.
3. Colle ce message :

```
Je participe à un projet de jeu de rôle avec mon ami Wesley. On travaille ensemble sur GitHub
(dépôt privé MossWes/Rpg) et je débute complètement avec GitHub.
Voici un document du projet. Explique-moi étape par étape, simplement, ce que je dois faire,
une action à la fois, et attends que je te dise « fait » avant de passer à la suite.
Si je te donne des questions à remplir, aide-moi à y répondre, puis rends-moi mes réponses
dans un texte prêt à coller dans une Issue GitHub.
```

## 8. Si quelque chose ne marche pas
| Problème | Solution |
|---|---|
| Je ne trouve pas l'invitation | https://github.com/MossWes/Rpg/invitations, en étant connecté. Sinon demande à Wesley de la renvoyer. |
| « 404 » sur le dépôt | Tu n'es pas encore invité ou pas connecté au bon compte. |
| Je ne vois pas le crayon | Ouvre le fichier dans le navigateur (pas l'application), ou passe par une Issue. |
| Je ne sais pas où écrire | Dans une Issue. Toujours. |
