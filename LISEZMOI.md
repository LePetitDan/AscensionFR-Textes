# AscensionFR — les textes français

Ce dépôt contient **les traductions** du projet AscensionFR : le texte français
du jeu, et rien d'autre. Les programmes qui fabriquent l'add-on restent chez le
mainteneur — ici, on écrit du français.

**Tu n'as besoin d'aucun outil.** Ce sont des fichiers JSON. Un éditeur de texte
suffit.

---

## Proposer une correction en 4 étapes

1. **Trouve le fichier.** Ils sont dans `traductions/`, un par famille de texte :

   | fichier | ce qu'il contient |
   |---|---|
   | `sorts.json` | noms et descriptions de sorts |
   | `objets.json`, `objets_dbc.json` | objets |
   | `quetes.json` | quêtes (titre, description, objectifs) |
   | `creatures.json` | noms de PNJ et de créatures |
   | `textes_pnj.json`, `gossip.json`, `pages.json` | dialogues et livres |
   | `gisement_brut.json` | **textes d'interface** (boutons, menus, infobulles) |

2. **Corrige la valeur française.** Ne touche **jamais** à la clé — c'est elle qui
   relie le texte au jeu.

3. **Ouvre une pull request** avec une phrase disant pourquoi.

4. Le mainteneur relit, fusionne, et ta correction part dans la version suivante.

---

## Les quatre choses à savoir avant de commencer

**1. La règle par défaut : l'officiel Blizzard gagne.**
Quand une traduction officielle française existe pour le même sort, le même lieu
ou le même titre, on prend celle de Blizzard. On garde la nôtre seulement quand
l'officiel *perd une information* (une couleur de monture, une mention utile) ou
se trompe de sort. Le vocabulaire propre à Ascension — ce qui n'existe pas chez
Blizzard — est arbitré par le mainteneur. Voir `GLOSSAIRE.md`.

**2. Ne touche pas aux codes de format.**
`$s1`, `$d`, `%s`, `%d`, `|cffffffff…|r`, `$b`, `$n` : ce sont des trous que le
jeu remplit. En ajouter, en retirer ou en changer l'ordre **casse l'affichage**,
et une vérification automatique rejettera la contribution.

**3. Les textes d'interface se corrigent dans `gisement_brut.json`.**
C'est le seul piège du dépôt et il vaut la peine d'être lu deux fois. Le fichier
`interface_maison.json` — que tu ne trouveras pas ici, exprès — est **reconstruit
automatiquement** à partir de `gisement_brut.json`. Une correction écrite dans le
fichier reconstruit serait effacée sans un mot au passage suivant.
`gisement_brut.json` est rangé par **texte anglais** : tu vois les deux côtés.

**4. Certaines chaînes d'interface ne servent à rien.**
Environ **une sur sept** (838 sur 5 974) est déjà couverte par la traduction
officielle de Blizzard, qui l'emporte. Les corriger ne change rien en jeu. En cas
de doute, demande avant de passer du temps dessus.

---

## Ce qui fait une bonne contribution

- **Un contresens, une phrase incompréhensible, un accord faux** : corrige, c'est
  toujours bienvenu.
- **Un choix de goût** (« Déchaînement » ou « Libération » ?) : ouvre plutôt une
  *issue* pour en discuter. Le vocabulaire est arbitré, pas voté — mais il se
  discute.
- **Petites PR plutôt qu'une grosse.** Vingt corrections dans un thème se relisent ;
  deux mille lignes ne se relisent pas.
- **Ne cite jamais le pseudo d'un joueur** dans un texte, un commentaire ou une PR.

## Ce que tu ne trouveras pas ici, et pourquoi

- **La chaîne de fabrication** — elle reste chez le mainteneur ;
- **Les rapports des joueurs** — ils contiennent des données de jeu personnelles ;
- **Les fichiers reconstruits automatiquement** (`interface_maison.json`,
  `emotes.json`, `taxinodes.json`, `interieurs.json`, `sorts_references.json`) —
  les publier ferait perdre les corrections qu'on y écrirait ;
- **Les textes anglais d'origine** — ils sont regénérés à chaque cycle et
  provoqueraient des conflits permanents.

## Merci

Chaque ligne relue par un humain vaut mieux que dix traduites par une machine.
