# Ohmyfood 🍽️

Site vitrine **mobile-first** d'une start-up fictive de réservation de menus gastronomiques à Paris.
Réalisé en **HTML5 / Sass (SCSS)**, **sans aucun framework ni JavaScript** : toutes les animations sont en CSS pur.

> Projet n°3 du parcours *Développeur Web* (OpenClassrooms).

## ✨ Fonctionnalités

- **Page d'accueil** : localisation, présentation du fonctionnement en 3 étapes, liste des 4 restaurants partenaires.
- **4 pages menu** (entrées / plats / desserts) :
  - *La palette du goût* — `la_palette_du_gout.html`
  - *La note enchantée* — `note_enchantee.html`
  - *À la française* — `a_la_francaise.html`
  - *Le délice des sens* — `le_delice_des_sens.html`
- **Animations CSS** :
  - loader d'accueil (1 à 3 s) avant l'affichage de la page ;
  - apparition progressive des plats au chargement d'une page menu ;
  - coche ✔ qui glisse au survol/clic d'un plat ;
  - cœur « J'aime » qui se remplit en dégradé au survol.
- **Responsive** : mobile (dès 320 px), tablette (≥ 768 px), desktop (≥ 992 px).
- HTML et CSS validés avec le **W3C Validator**.

## 🛠️ Technologies

| Outil | Rôle |
|---|---|
| HTML5 | Structure des pages |
| Sass (SCSS) | Styles, variables, mixins, architecture modulaire |
| PostCSS + Autoprefixer | Ajout des préfixes navigateurs (`last 4 versions`) |
| normalize.css | Harmonisation des styles par défaut |
| Font Awesome 6 | Icônes |
| Google Fonts | Polices *Roboto* et *Shrikhand* |

## 📁 Structure du projet

```
P3/
├── index.html                  # Page d'accueil
├── la_palette_du_gout.html     # Pages menu
├── note_enchantee.html
├── a_la_francaise.html
├── le_delice_des_sens.html
├── sass/                       # Sources SCSS (pattern 7-1 simplifié)
│   ├── main.scss               # Point d'entrée
│   ├── utils/                  # Variables, mixins, keyframes
│   ├── base/                   # Base et typographie
│   ├── components/             # Liens, images, loader
│   ├── layout/                 # Header, formulaires, conteneurs, footer
│   └── pages/                  # Styles propres à l'accueil
└── public/
    ├── css/
    │   ├── style.css           # CSS compilé par Sass
    │   ├── prefixed/style.css  # CSS final préfixé (utilisé par les pages)
    │   └── normalize.css
    └── img/                    # Logo, favicon, photos des restaurants
```

## 🚀 Installation et lancement

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/Orkea/P3.git
   cd P3
   ```
2. Ouvrir `index.html` dans un navigateur (aucun serveur nécessaire).

### Modifier les styles

Installer les dépendances (Sass, PostCSS, Autoprefixer) :
```bash
npm install
```

Compiler le SCSS en continu :
```bash
npm run sass
```

Dans un second terminal, générer le CSS préfixé en continu :
```bash
npm run prefix
```

> ⚠️ Les pages HTML chargent `public/css/prefixed/style.css` : pense à lancer les **deux** scripts pour voir tes modifications.

## 🎨 Charte graphique

| Couleur | Code |
|---|---|
| Primaire | `#9356DC` |
| Secondaire | `#FF79DA` |
| Tertiaire | `#99E2D0` |

Polices : **Shrikhand** (titres), **Roboto** (texte).

## 📸 Crédits

Photos des restaurants : [Unsplash](https://unsplash.com).
