# Portfolio Julia Huang

Un portfolio moderne et élégant pour une artiste IA, construit avec SvelteKit et Tailwind CSS. Ce projet présente les œuvres de Julia Huang, une artiste innovante qui redéfinit l'architecture avec des designs pilotés par l'IA.

## 📸 Aperçu

### Version Desktop
![Desktop](/static/images/screenshot.png)


## Demo Live

**[Voir le projet en live](https://julia-portfolio-seven.vercel.app/)**

> Découvrez le portfolio complet avec toutes les animations et interactions

## ✨ Fonctionnalités

- **Design Responsive** - Optimisé pour tous les appareils (mobile, tablette, desktop)
- **Animations Fluides** - Icônes rotatives, transitions hover, effets visuels subtils
- **Navigation Mobile** - Menu hamburger avec transitions Svelte
- **Grid Layout Moderne** - Mise en page dynamique avec CSS Grid
- **État Global** - Gestion centralisée de l'état de navigation
- **Optimisé SEO** - Structure sémantique et accessibilité

## 🛠️ Technologies Utilisées

- **[SvelteKit](https://kit.svelte.dev/)** - Framework full-stack moderne
- **[Tailwind CSS](https://tailwindcss.com/)** - Framework CSS utility-first
- **[Lucide](https://lucide.dev/)** - Icônes modernes et cohérentes
- **[Iconify](https://iconify.design/)** - Collection d'icônes pour les réseaux sociaux
- **Svelte Transitions** - Animations et transitions natives

## 🚀 Installation et Développement

### Prérequis
- Node.js (version 18 ou supérieure)
- npm ou pnpm

### Installation

```bash
# Cloner le repository
git clone https://github.com/votre-username/portfolio-julia-huang.git

# Naviguer dans le dossier
cd portfolio-julia-huang

# Installer les dépendances
npm install
```

### Développement

```bash
# Lancer le serveur de développement
npm run dev

# Ou avec pnpm
pnpm dev
```

Ouvrez [http://localhost:5173](http://localhost:5173) dans votre navigateur.

### Build de Production

```bash
# Créer le build de production
npm run build

# Prévisualiser le build
npm run preview
```

## 📱 Structure du Projet

```
src/
├── lib/
│   └── global state/
│       └── navbarState.svelte     # État global de la navigation
├── routes/
│   ├── +layout.svelte             # Layout principal
│   └── +page.svelte               # Page d'accueil
└── app.html                       # Template HTML

static/
└── images/                        # Assets statiques
    ├── flower.svg
    ├── julia.svg
    ├── circleIcon.svg
    └── image.svg
```

## 🎨 Fonctionnalités Visuelles

### Animations
- **Icône fleur** - Rotation continue (6 secondes)
- **Icône cercle** - Rotation continue (3 secondes)
- **Effets hover** - Transformations et changements de couleur
- **Navigation mobile** - Transitions slide fluides

### Layout Responsive
- **Mobile First** - Design optimisé pour mobile
- **Grid Adaptatif** - Layout qui s'adapte selon la taille d'écran
- **Breakpoints** - md: 768px, lg: 1024px

### Palette de Couleurs
- **Primary** - Couleur principale des cards
- **Secondary** - Couleur d'accent et hover
- Palette cohérente définie dans Tailwind

## 📄 Pages et Sections

### Page d'Accueil
- **Hero Section** - Présentation avec titre principal
- **Portrait** - Photo de Julia Huang
- **À Propos** - Description de l'artiste
- **Projet Musea** - Mise en avant du projet principal
- **Contact** - Liens vers les réseaux sociaux
- **Navigation Mobile** - Menu responsive

## 🔧 Personnalisation

### Couleurs
Modifiez les couleurs dans `tailwind.config.js` :

```js
module.exports = {
@import url('https://fonts.googleapis.com/css2?family=Alata&family=Barlow+Semi+Condensed:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Edu+AU+VIC+WA+NT+Arrows:wght@400..700&family=Figtree:ital,wght@0,300..900;1,300..900&family=Fraunces:ital,opsz,wght@0,9..144,100..900;1,9..144,100..900&family=Gilda+Display&family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&family=Karla:ital,wght@0,200..800;1,200..800&family=League+Spartan:wght@100..900&family=Manrope:wght@200..800&family=Montserrat:ital,wght@0,100..900;1,100..900&family=Mulish:ital,wght@0,200..1000;1,200..1000&family=Outfit:wght@100..900&family=Overpass:ital,wght@0,100..900;1,100..900&family=PT+Serif:ital,wght@0,400;0,700;1,400;1,700&family=Playfair:ital,opsz,wght@0,5..1200,300..900;1,5..1200,300..900&family=Playwrite+MX+Guides&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Roboto:ital,wght@0,100..900;1,100..900&family=Rubik:ital,wght@0,300..900;1,300..900&family=Space+Mono:ital,wght@0,400;0,700;1,400;1,700&family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&family=Work+Sans:ital,wght@0,100..900;1,100..900&family=Young+Serif&display=swap');


@import "tailwindcss";



@theme {
    --color-primary: #FADCD9;
    --color-secondary: #F8AFA6;
    --color-background: #F9F1F0;

    --font-inter: "Inter", sans-serif;

    --animate-duration: 6000;
}

@layer base {
    h1 {
        font-size: 56px;
    }

    h2 {
        font-size: 55px;
    }

    p {
        font-size: 20px;
        line-height: 1.5;
    }

    h1, h2 {
        color: black;
        line-height: normal;
    }

    img {
        max-width: 100%;
    }

}

body {
    background-color: var(--color-background);
    font-family: var(--font-inter);
    color: #000;
}


.container {
    max-width: 1480px;
    margin: 1.5em auto;

    @media screen and (max-width: 48rem) {
        max-width: 90%;
    }
}

```

### Images
Remplacez les images dans le dossier `static/images/` :
- `flower.svg` - Icône décorative
- `julia.svg` - Portrait de l'artiste
- `circleIcon.svg` - Icône décorative
- `image.svg` - Image du projet

## 📱 Navigation Mobile

Le menu mobile inclut :
- Transition slide fluide
- État global persistant
- Auto-fermeture sur navigation
- Liens vers toutes les sections

## 🌟 Améliorations Futures

- [ ] Système de routage pour About/Contact
- [ ] Galerie de projets interactive
- [ ] Mode sombre/clair
- [ ] Formulaire de contact fonctionnel
- [ ] Blog/actualités
- [ ] Multilingue (FR/EN)


## 📞 Contact

**Julia Huang** - Artiste IA
- Instagram: [@julia_huang](https://instagram.com/julia_huang)
- LinkedIn: [Julia Huang](https://linkedin.com/in/julia-huang)
- X (Twitter): [@julia_huang](https://x.com/julia_huang)

**Développeur** - [Votre nom]
- GitHub: [@NitiemaAllassane](https://github.com/NitiemaAllassane)

---

Fait avec ❤️ et SvelteKit