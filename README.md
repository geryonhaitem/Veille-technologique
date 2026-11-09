# Veille technologique

Projet de veille technologique mené dans le cadre du BTS. Il a trois objectifs : préparer l'épreuve orale, recevoir automatiquement l'actualité (tech et générale), et suivre ce qui touche chacun de mes projets.

Tout est versionné dans ce dépôt : l'historique git prouve que la veille est régulière dans le temps.

## Objectifs

### 1. Thème de l'épreuve orale du BTS

Choisir un thème spécifique, le suivre dans la durée et le présenter à l'oral lors de l'épreuve du BTS.

- **Thème retenu :** _à définir_
- **Justification du choix :** _à compléter_
- **Méthode :** une fiche par article notable (source, date, résumé, avis, lien), puis une synthèse qui servira de support à l'oral.

### 2. Remontée d'informations automatique

L'actualité arrive automatiquement, répartie sur deux canaux :

| Canal | Contenu |
|---|---|
| **Tech ciblée** | La plupart des sujets tech qui me concernent directement |
| **Général** | Les informations importantes au-delà de la tech : géopolitique, économie, droit, politique |

#### Canal Général

Objectif : savoir répondre à « vous avez vu ce qu'il s'est passé hier ? » et faire le lien avec mon métier (et avec la CEJM).

| Rubrique | Exemples | Sources |
|---|---|---|
| **Géopolitique** | guerres, sanctions, tensions sur les semi-conducteurs | France Info, Le Monde, Le Grand Continent |
| **Économie & entreprises** | levées de fonds, rachats, introductions en Bourse, faillites | Les Echos, Maddyness, FrenchWeb, Siècle Digital |
| **Marchés publics** | appels d'offres IT | BOAMP (alertes « informatique », « logiciel », « cybersécurité ») |
| **Politique & droit** | élections, lois, RGPD, AI Act, NIS2 | Vie-publique.fr, CNIL, Next.ink |
| **Cyber grand public** | grosses fuites, attaques d'hôpitaux ou de collectivités | CERT-FR, Cybermalveillance.gouv, ZATAZ |

Brief du matin (5 min) : *Le 7/9* (France Inter), *L'Heure du Monde*, *Brief.me* ou *Le Brief Éco*.

Chaque actu notée suit ce format :

```
## AAAA-MM-JJ — Titre de l'actu
Rubrique : Économie
Angle CEJM : économique / juridique / managérial
Lien avec mon métier : en quoi ça concerne un informaticien
```

### 3. Veille par projet

Remonter les informations des secteurs liés à mes projets (par exemple une faille de sécurité dans un framework que j'utilise) et tenir un **journal d'intérêt** pour chacun de mes projets.

- **Failles :** Dependabot activé sur les dépôts des projets (alertes CVE sur les dépendances).
- **Mises à jour :** « Watch → Releases » sur GitHub pour les frameworks clés.

| Projet | Technologies / frameworks suivis | Journal |
|---|---|---|
| _à compléter_ | _à compléter_ | _à compléter_ |

## Rythme

- **Quotidien (5 min) :** brief du matin et survol des deux canaux.
- **Hebdomadaire (30 min) :** fiches pour l'oral, journal Général, journaux projets, en un commit.
- **Mensuel :** relecture de la synthèse de l'oral et sélection des actus majeures « à retenir ».

## Organisation du dépôt

```
Veille technologique/
├── README.md
├── sources.md          # sources suivies, classées par canal
├── oral-bts/
│   ├── theme.md        # thème choisi, justification, problématique
│   ├── fiches/         # une fiche par article notable
│   └── synthese.md     # support de l'oral
├── general/
│   ├── AAAA-MM.md      # journal mensuel des actus générales
│   └── a-retenir.md    # actus majeures de l'année (révisions CEJM)
├── projets/
│   └── <projet>.md     # journal d'intérêt par projet
└── digests/            # remontées automatiques archivées
```

_Structure cible : les dossiers seront créés au fur et à mesure._

## Workflow git

Issue → branche → commits → push → pull request (avec `Closes #N`) → merge.
