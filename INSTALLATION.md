# Installation — XeroLe1er GitHub Profile

Cette version ne contient **aucune image custom**.

Tout le visuel repose sur des projets/services existants :

- Capsule Render — vagues, headers, footer et transitions
- Readme Typing SVG — texte animé
- Shields.io — badges
- Skill Icons — stack
- GitHub Profile Summary Cards — statistiques animées
- GitHub Readme Streak Stats — séries de contributions
- GitHub Profile Trophy — trophées
- GitHub Readme Activity Graph — activité
- Platane/snk — snake des contributions
- GitHub Profile 3D Contrib — calendrier 3D

## Fichiers

```text
XeroLe1er-GitHub-Profile-NoCustom/
├── README.md
├── README_EN.md
├── INSTALLATION.md
├── conf/
│   └── github-profile-3d-contrib.json
└── .github/
    └── workflows/
        ├── profile-3d.yml
        └── snake.yml
```

## Installation

Copie simplement le **contenu** du dossier à la racine de :

```text
XeroDroiD/XeroDroiD
```

Puis commit/push sur `main`.

## Actions à lancer une première fois

Dans l'onglet **Actions** du repository :

1. Lance `Generate contribution snake`.
2. Lance `Generate 3D contribution calendar`.

Le premier crée la branche :

```text
output
```

Le second crée :

```text
output-3d-contrib
```

Après ça, le snake et le calendrier 3D apparaissent dans le README.

## Permissions

Si une Action obtient une erreur d'écriture :

```text
Repository
→ Settings
→ Actions
→ General
→ Workflow permissions
→ Read and write permissions
```

Les deux workflows contiennent déjà :

```yaml
permissions:
  contents: write
```

## FR / EN

- `README.md` = français par défaut
- `README_EN.md` = anglais

Les boutons en haut permettent de passer de l'un à l'autre.

## Important concernant le nom

Le nom affiché est :

```text
XeroLe1er
```

Le login GitHub utilisé dans les URLs dynamiques reste :

```text
XeroDroiD
```

tant que le compte GitHub n'est pas renommé.

## Ancienne version

Si tu avais copié la version précédente, tu peux supprimer entièrement :

```text
assets/
```

Elle n'est plus utilisée dans cette version.
