# Glossaire AscensionFR — vocabulaire arbitré

La **référence** pour traduire. Elle grandit au fil des décisions de Dan.
Règle d'or : en cas de doute sur un terme de goût, **proposer, ne pas figer**.

---

## ⭐ La règle par défaut — décidée par Dan le 26/07/2026

> **Quand notre traduction et l'officiel Blizzard divergent, l'officiel gagne —
> SAUF quand l'officiel perd une information.**

C'est-à-dire : on prend le mot de Blizzard quand c'est le même sort, le même lieu ou le
même titre. On garde le nôtre quand l'officiel fait disparaître une précision utile
(couleur d'une monture, mention « (Animal) », détail d'un effet) ou quand il se trompe de
sort.

**Ce que ça change :** je n'ai plus besoin de demander pour chaque terme. Cette règle
tranche seule les **121 divergences officielles** et guide les **1 762 conflits de noms
Glayna**. Elle a déjà réglé « Starcaller » sans arbitrage supplémentaire.

**Ce qui reste soumis à Dan :** les termes propres à Ascension, qui n'ont pas d'équivalent
officiel (Draft, Manastorm, les cartes de compétence…) — là, il n'y a pas de référence
extérieure, donc c'est un choix de goût.

> 🔴 **La règle ne s'applique pas encore EN MASSE — mesuré le 26/07/2026.**
> L'outil d'arbitrage (`appliquer_divergences_officielles.py`) croise le nom anglais
> d'Ascension avec le français de Blizzard **au même numéro de sort, sans vérifier que
> Blizzard nommait ce sort pareil**. Or Ascension renomme des sorts en place : l'ID 2831
> s'appelait « Armor +8 » chez Blizzard, Ascension l'a rebaptisé « Armor (Light) » — et on
> récupérait « Armure +8 ». Résultat mesuré : **45 % de régressions** si la passe partait
> en l'état. Le garde-fou (comparer d'abord le nom anglais de Blizzard) est posé au lot 7 ;
> la passe partira après la 3.4. **Le cœur du pipeline, lui, est sain.**
> *Leçon : une règle juste appliquée par un outil faux fait plus de dégâts que pas de règle.*

---

## Termes fixés

| Anglais | Français retenu | Note |
|---|---|---|
| Skill Card | Carte de compétence | |
| Golden (Skill Card) | dorée | « Golden Skill Card » → « Carte de compétence dorée » |
| Lucky (Skill Card) | chanceuse | |
| Darkmoon | Sombrelune | |
| **PvP / PvE** | **PvP / PvE** *(on n'écrit pas JcJ/JcE)* | *Décidé le 26/07/2026.* Écriture déjà majoritaire (3 254 + 983 contre 507) et mot employé par les joueurs entre eux. **510 textes en « JcJ/JcE » sont à aligner.** |
| **Draft** *(Build Draft, Draft Mode)* | **Draft** — on garde l'anglais | *Décidé le 26/07/2026.* Nom de la mécanique d'Ascension, comme au jeu de cartes. On fige « mode Draft » et « Draft de build » sur les **730 occurrences**. ⚠️ Corriger au passage les « draft » traduits par **« rédiger »** (« rédiger de nouveaux sorts ») : contresens. |
| **Manastorm** | **Tempête de mana** | *Décidé le 26/07/2026.* Majoritaire chez nous (574 contre 266) et cohérent avec les autres lieux traduits (Stormwind → Hurlevent). **266 textes à basculer** — aujourd'hui les deux formes se mélangent dans la même phrase. |
| **Starcaller** | **Mande-étoiles** | *Décidé le 26/07/2026 — premier cas réglé par la règle par défaut.* Titre officiel Blizzard. Remplace « Héraut stellaire » (39 occurrences) ; 185 textes encore en anglais à traiter. |
| **to draft** *(le verbe)* | **composer** | *Décidé le 26/07/2026.* « Composez de nouveaux sorts de départ ». Le **nom** du mode reste « Draft » ; seul le verbe est français. Corrige « rédiger », « reformuler », « remanier », « réécrire » — **39 entrées**, pas 16 : les gardes cherchaient `drafted` en minuscules alors que le jeu écrit « **D**rafted ». |
| **Shanked!** | **Coup de surin !** | *Décidé le 26/07/2026.* Blizzard traduit « shank » par **surin** (6 objets officiels sur 7), mais jamais au participe — et « Suriner » est déjà le nom de *Gouge*. On reprend donc le substantif attesté. Avant : « Pourfendre », qui était la traduction de *Rend*. |
| **Abyssal Draft** | **Souffle abyssal** | ⚠️ **Rien à voir avec le mode Draft** : c'est un réactif d'artisanat où *draft* veut dire **courant d'air**. Sa famille le prouve : Droplet→Eau, Spark→Feu, Fragment→Terre, Draft→**Air**. Était livré « Draft abyssal ». |
| **Millhouse Manastorm** | **Millhouse Manastorm** *(inchangé)* | ⚠️ **C'est un personnage** (le gnome de l'Arcatraz), pas le donjon. Blizzard le laisse tel quel en français. Corrige « Tempête de mana du moulin » — quelqu'un avait lu « mill house ». **Exclu de la règle Manastorm.** |
| **Casting** *(nom, dans l'interface)* | **Incantation** | *26/07/2026.* « Mouseover Casting » → « Incantation au survol ». Le **verbe** reste « Lancer ». **10 libellés, pas 6** : quatre étaient traduits par « **diffusion** » (le traducteur avait lu *broadcast*) — chercher le mot du côté français ne les voyait pas. Exception : « Casting Damage Dealer » → **« Attaquant incantateur »**, aligné sur son libellé court frère. |
| **Static** *(ressource de classe Ascension)* | **Statique** *(majuscule)* | *Décidé le 26/07/2026.* « Génère 20 **Statique** ». La majuscule dit que c'est une ressource et pas un adjectif. Corrige « Génère 20 statiques », qui ne veut rien dire. |
| **Arathi Basin** | **bassin Arathi** *(sans apostrophe)* | *26/07/2026.* Nom officiel Blizzard. Ce qu'on supprime, c'est **l'apostrophe** de « bassin **d'**Arathi » — **83 occurrences** dans 6 bases livrées, harmonisées au point d'écriture. ⚠️ **On ne force pas la majuscule** : l'usage livré est à 185 minuscules contre 41, et « dans le Bassin Arathi » au milieu d'une phrase serait fautif. Le nom est le même dans les deux casses. |
| **Warsong Gulch** | **Goulet des Warsong** | *26/07/2026 — réglé par la règle par défaut.* Nom officiel Blizzard ; était resté en anglais. |
| **Light Lash** | **Fouet de Lumière** | *Décidé le 26/07/2026.* ⚠️ Corrige un **contresens** : c'était « Cils légers » / « Cils clairs » — « lash » compris comme un cil d'œil au lieu d'un coup de fouet. Aligné sur la série existante : Lava Lash = Fouet de lave, Wind Lash = Fouet des vents, Ice Lash = Fouet de glace. 6 textes. |
| **Unleash:** *(mot-clé, suivi de deux-points)* | **Déchaînement :** | *Décidé le 25/07/2026.* Mot-clé de mécanique en tête de ligne : un nom, comme en anglais. |
| **Unleash** *(verbe dans une phrase)* | **Déchaînez / Déchaîner** | *Corrigé le 25/07/2026.* ⚠️ **Les deux cas ne se traduisent pas pareil.** « Unleash a devastating Oath Breaker » → « **Déchaînez** un Brise-Serment dévastateur ». Y appliquer « Déchaînement : » donnerait une phrase cassée. Dans `sorts.json`, les 73 occurrences étaient **toutes** des verbes. |
| **Soulbound** | **lié** | *Décidé le 25/07/2026.* L'usage WoW habituel. |
| **Realm Bound** | **lié au royaume** | *Décidé le 25/07/2026.* Mécanique propre à Ascension, à distinguer de `Soulbound`. |
| **Keeper's Scroll** | **Parchemin du gardien** | *Décidé le 25/07/2026.* **Minuscule à « gardien »** (ce n'est pas un titre). |
| **Dreadnought / Dreadnaught** | **Cuirassé** | *Acté le 25/07/2026 par cohérence :* c'est déjà la traduction dans toutes nos sources (« Cuirassier », « cuirassé sanguin »…). « Redoutable cuirassé » vu en jeu est une anomalie isolée. |
| Food Crate | Caisse de nourriture | Proposé par un joueur (« Boite de nouriture ») — idée juste, orthographe corrigée. |

## Noms de lieux — l'officiel Blizzard s'applique

Ces noms sont **déjà présents dans nos sources** ; quand un joueur les voit en anglais,
c'est un **trou d'application**, pas un manque de vocabulaire.

| Anglais | Français officiel | Présence dans nos sources |
|---|---|---|
| Stormwind | Hurlevent | 784 occurrences |
| Booty Bay | Baie-du-Butin | 228 occurrences |
| Stranglethorn | Strangleronce | 136 occurrences |

## Corrections de sorts appliquées (vers l'officiel Blizzard)
Exemples de nos traductions cassées corrigées — logique à reproduire :

| Anglais | Avant (cassé) | Corrigé |
|---|---|---|
| Holy Light | Sacré Lumière | Lumière sacrée |
| Life Tap | Vie Tap | Connexion |
| Soul Tap | Âme Tap | Connexion d'âme |
| Corrupted Blood | Corrompu sang | Sang vicié |
| Bash (druide) | Coup | Sonner |
| Lifeblood | Sang vital | Sang-de-vie |
| **Touch of Moonlight** | Touch de clair de lune | **Toucher du clair de lune** |
| **Briar Veil** | Briar voile | **Voile de ronces** |
| **Angelic Touch** | Angélique Touch | **Toucher angélique** |
| **Arrow Storm** | Flèche Storm | **Tempête de flèches** |
| **Light Lash** | Cils légers / Cils clairs | **Fouet de Lumière** |

## Principes de vocabulaire (appris)

- **La règle par défaut d'abord** (voir en haut) : l'officiel gagne, sauf perte de sens.
  Ne poser une question que pour les termes **propres à Ascension**, sans équivalent officiel.
- **Ne pas prendre l'officiel les yeux fermés.** Souvent l'officiel est PIRE :
  il perd de l'info (couleur d'une monture, « (Animal) »…), se trompe de sort,
  ou porte un artefact de rang (« Armure +8 »). Comparer le SENS, pas juste le nom.
- **Vérifier l'usage existant avant de poser une question.** Deux arbitrages se sont réglés
  seuls en regardant nos propres sources : « Cuirassé » y était déjà partout, et « Lash »
  y était déjà « Fouet ». Une question évitée vaut mieux qu'une question bien posée.
- **Concordance de mots obligatoire** avant de remplacer une trad : si les deux
  versions n'ont aucun mot en commun, méfiance (souvent un mauvais appariement).
  *Exemple trouvé le 25/07 :* `Worldforged Scroll: Dreadnaught` → « Mystic Scroll:
  Mongoose Fury ». Aucun rapport : appariement faux, à corriger.
- **Jamais de remplacement global sur un mot français.** Toujours vérifier la clé
  anglaise d'abord. Sur 165 « Libérez », 73 seulement traduisaient « Unleash » —
  un remplacement en masse en aurait cassé les 91 autres.
- **Vérifier la FONCTION du mot, pas seulement sa présence.** Un même mot anglais peut être
  un mot-clé de mécanique ou un verbe de phrase, et les deux ne se traduisent pas pareil.
  *Leçon du 25/07 :* j'avais lu « Unleash: » dans les signalements (mot-clé) et généralisé
  la règle à toutes les occurrences — or elles étaient toutes des verbes. Regarder les
  textes réels avant de fixer une règle.
- **Filtrer sur le mot entier.** « Unleash » en sous-chaîne attrape « Unleash**ing** this
  Seal » : 143 faux positifs au lieu de 73.
- Le jeu affiche des **nombres calculés** (formules) : ne jamais inventer un chiffre.
- **Un mot anglais resté dans un nom français** est un contresens, pas un choix de goût :
  il se corrige sans arbitrage, et se signale.
- **Un mot mal compris** (« lash » → cil au lieu de fouet) est aussi un contresens : même
  traitement. Le goût, c'est choisir entre deux formulations justes.

*(À compléter au fil des arbitrages — c'est cette table qui sert de vérité.)*
