# Installation — Profil GitHub XeroLe1er

Ce pack est prévu pour le repository de profil :

```text
XeroDroiD/XeroDroiD
```

Le **nom affiché** est `XeroLe1er`.  
Le login GitHub reste `XeroDroiD`, donc certaines URLs techniques contiennent obligatoirement `XeroDroiD`.

## Structure

```text
XeroLe1er-GitHub-Profile/
├── README.md
├── README_EN.md
├── INSTALLATION.md
├── PROFILE_CONFIG.md
├── assets/
│   ├── hero.svg
│   ├── terminal.svg
│   ├── focus.svg
│   ├── divider.svg
│   └── footer.svg
└── .github/
    └── workflows/
        └── snake.yml
```

## Installation rapide

1. Ouvre le repository `XeroDroiD/XeroDroiD`.
2. Copie **tout le contenu du dossier** à la racine du repository.
3. Remplace l'ancien `README.md`.
4. Commit/push sur la branche `main`.
5. Ouvre l'onglet **Actions**.
6. Lance manuellement **Generate contribution snake** une première fois.
7. Après la création de la branche `output`, recharge ton profil.

## Si le workflow Snake ne peut pas publier

Dans le repository :

```text
Settings
→ Actions
→ General
→ Workflow permissions
```

Vérifie que GitHub Actions est autorisé à écrire dans le repository.

Le workflow demande déjà :

```yaml
permissions:
  contents: write
```

## Langues

GitHub ne permet pas d'exécuter du JavaScript interactif dans un README.

Le sélecteur FR/EN est donc fait proprement avec deux documents :

- `README.md` → Français
- `README_EN.md` → English

Les boutons en haut permettent de passer de l'un à l'autre.

## Animations

Les animations principales sont locales :

- `assets/hero.svg`
- `assets/terminal.svg`
- `assets/focus.svg`
- `assets/divider.svg`
- `assets/footer.svg`

Elles utilisent du SVG/SMIL et sont directement versionnées avec le profil.

## Services externes utilisés

Le README utilise aussi quelques services uniquement pour les données dynamiques :

- `shields.io` — badges
- `komarev.com` — compteur de vues
- `skillicons.dev` — icônes technos
- `github-profile-summary-cards.vercel.app` — statistiques
- `github-readme-activity-graph.vercel.app` — graphe d'activité
- `readme-typing-svg.demolab.com` — texte animé
- `Platane/snk` — génération du Snake via GitHub Actions

Même si l'un de ces services tombe temporairement, les assets principaux du profil restent affichés.
