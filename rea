# 🚀 AstroCore: Abandoned But Not Forgotten

> **NASA Space Apps Challenge 2026** — An interactive digital museum and planetary archaeology archive exploring humanity's discarded equipment and historical relics preserved on the Moon and Mars.

[![NASA Space Apps](https://img.shields.io/badge/NASA_Space_Apps-Challenge_2026-0B3D91?style=for-the-badge&logo=nasa&logoColor=white)](https://www.spaceappschallenge.org/)
[![React](https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Three.js](https://img.shields.io/badge/Three.js-black?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS_v4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Vite](https://img.shields.io/badge/Vite_8-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

---

## 🌌 Overview

Between 1959 and today, humanity has dispatched hundreds of robotic landers, rovers, ascent/descent stages, and scientific instruments beyond Earth. While their active operations eventually concluded, **these machines never returned**. They remain perfectly preserved in the vacuum of the Moon and the hyper-arid deserts of Mars—constituting humanity's very first interplanetary archaeological record.

**AstroCore** transforms this dormant history into a futuristic NASA mission-control interactive experience. Users can explore high-resolution 3D planetary spheres, track orbital artifacts in 3D perspective, inspect verified landing coordinates, and read chronicles of the machines that paved the path for human space exploration.

---

## ✨ Key Features

### 🪐 1. 3D Planetary Visualization (Three.js / WebGL)
- **Dynamic 3D Celestial Spheres**: Real-time rendering of the Moon and Mars with realistic day/night solar terminator shading, axial rotation, and subtle orbital rings.
- **Custom Shader Atmospheres**:
  - **Moon**: Stark regolith, realistic crater bump mapping, and crisp terminator line with subtle limb scattering.
  - **Mars**: Rust-orange terrain variation and thin atmospheric Rayleigh scattering glow.
- **Smooth Planetary Transitions**: Seamless crossfade between Moon and Mars textures, lighting schemes, and telemetry data.
- **Desktop Parallax**: Mouse tracking applies subtle 3D tilt and depth to the planet and orbital plane.

### 🛰️ 2. Orbital Relics 3D Perspective Carousel
- **Orbital Trajectory Motion**: Mission artifact cards physically orbit around the 3D planet along an elliptical path.
- **Depth-Adaptive Visuals**:
  - **Front Card**: Larger scale (1.1×), sharp focus, glowing aerospace accent border, and priority z-index.
  - **Side Cards**: Tangent rotation (`rotateY`), subtle depth blur, and dimmed opacity.
  - **Back Cards**: Soft background focus behind the planet.
- **Interactive Controls**:
  - Mouse drag or touch swipe with momentum to manually spin the orbit.
  - Click any card to bring it directly to the front.
  - Play/Pause orbital motion, Previous/Next navigation, and Hover-to-Read freeze.
  - Telemetry inspector opening full historical mission chronicles.

### 📍 3. Verified Historical Telemetry & Equipment Data
Every relic features verified coordinates from NASA Lunar Reconnaissance Orbiter Camera (LROC) and Mars Reconnaissance Orbiter (MRO) datasets:
- **Moon**:
  - `Apollo 15 Lunar Roving Vehicle 001`: Hadley-Apennine (`26.132° N, 3.634° E`) — *Status: LEFT BEHIND*
  - `Lunokhod 1 Soviet Rover (Luna 17)`: Mare Imbrium (`38.315° N, 35.008° W`) — *Status: MISSION COMPLETE*
  - `Apollo 11 LM-5 Descent Stage "Eagle"`: Tranquility Base (`0.674° N, 23.473° E`) — *Status: LEFT BEHIND*
  - `Surveyor 3 Retrieval Site`: Oceanus Procellarum (`3.012° S, 23.422° W`) — *Status: LEFT BEHIND*
- **Mars**:
  - `Opportunity Rover (MER-B)`: Perseverance Valley, Meridiani Planum (`1.948° S, 354.474° E`) — *Status: MISSION COMPLETE*
  - `Perseverance Rover & Ingenuity`: Jezero Crater Delta (`18.445° N, 77.451° E`) — *Status: ACTIVE*
  - `Viking 1 Lander`: Chryse Planitia (`22.48° N, 47.97° W`) — *Status: STATIONARY*
  - `Curiosity Rover (MSL)`: Gale Crater / Mount Sharp (`4.589° S, 137.441° E`) — *Status: ACTIVE*

### 🗺️ 4. Interactive Surface Maps
- 2D topographic landing maps for both the Moon and Mars.
- Interactive radar pins for landing sites with coordinates, status filters (Active, Left Behind, Mission Complete, Retired), and deep links to mission dossiers.

### ☀️ 5. Solar System Gateway
- High-fidelity visual showcase of all 8 major planets (Mercury to Neptune).
- Clean transparent-background planetary spheres with authentic colors, atmospheric properties, orbital distance, and surface temperatures.

### 📖 6. Narrative Chronicles & Chronological Timeline
- Rich historical accounts detailing the engineering triumphs, final transmissions, and archaeological significance of each abandoned machine.
- Interactive timeline tracking exploration missions across the decades from 1959 to present.

### ⚡ 7. Instant Search & Command Palette (`⌘K` / `Ctrl+K`)
- Global keyboard shortcut to instantly search artifacts by hardware name, mission name, target body, or operational status.

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| **Frontend Framework** | [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) |
| **Build Tool** | [Vite 8](https://vitejs.dev/) |
| **3D Graphics** | [Three.js](https://threejs.org/) (WebGL Canvas, Custom Shaders, Texture Mapping) |
| **Styling** | [Tailwind CSS v4](https://tailwindcss.com/) (Glassmorphism, Dark Aerospace Theme) |
| **Animation** | [Motion](https://motion.dev/) & CSS 3D Transforms |
| **Icons** | [Lucide React](https://lucide.dev/) |
| **Optimization** | Progressive WebP / JPEG texture compression with alpha masking |

---

## 📁 Project Structure

```text
astrocore/
├── public/                     # Static assets and production fallback files
│   ├── images/                 # Optimized planet globes & artifact renders
│   └── .htaccess               # Apache / cPanel SPA rewrite configuration
├── src/
│   ├── assets/                 # Asset imports and manifest
│   │   ├── images/             # WebP and JPEG imagery
│   │   └── index.ts            # Centralized image exports
│   ├── components/             # Reusable UI & 3D visualization components
│   │   ├── Navigation.tsx      # Top aerospace glassmorphism header
│   │   ├── OrbitalPlanetCanvas.tsx # Three.js WebGL 3D planet sphere canvas
│   │   ├── OrbitalRelicsSection.tsx # 3D rotating artifact cards experience
│   │   ├── PlanetOrbitalCarousel.tsx # Solar System 8-planet carousel
│   │   ├── PlanetSphereVisual.tsx # Single planet visual with glow & terminator
│   │   ├── InteractiveSurfaceMap.tsx # Surface maps with radar landing pins
│   │   ├── MoonPage.tsx        # Dedicated lunar artifacts explorer
│   │   ├── MarsPage.tsx        # Dedicated Martian artifacts explorer
│   │   ├── StoryTimeline.tsx   # Chronological mission timeline
│   │   ├── StoriesSection.tsx  # Editorial chronicles & narratives
│   │   ├── WhereAreTheyNowSection.tsx # Equipment whereabouts catalog
│   │   ├── StoryModal.tsx      # In-depth story reading modal
│   │   ├── ArtifactModal.tsx   # Detailed artifact telemetry modal
│   │   ├── SearchModal.tsx     # ⌘K instant search modal
│   │   ├── CinematicTransit.tsx # Planetary transit warp transition
│   │   └── Footer.tsx          # NASA challenge attribution footer
│   ├── data/                   # Verified missions & planetary data
│   │   ├── planets.ts          # 8 planets scientific data & textures
│   │   ├── orbitalRelics.ts    # Moon & Mars orbital relics data & coordinates
│   │   ├── moonArtifacts.ts    # Complete lunar catalog
│   │   ├── marsArtifacts.ts    # Complete Mars catalog
│   │   └── stories.ts          # Archival narrative stories
│   ├── types/                  # TypeScript interfaces and type definitions
│   ├── App.tsx                 # Root application controller & router
│   ├── main.tsx                # Entry point
│   └── index.css               # Global styles & Tailwind CSS configuration
├── index.html                  # HTML entry point with meta tags & SEO
├── package.json                # Dependencies & scripts
├── tsconfig.json               # TypeScript compiler configuration
└── vite.config.ts              # Vite configuration
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (version 18 or higher recommended)
- `npm` or `yarn` or `pnpm`

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/astrocore.git
   cd astrocore
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Open your browser:**
   Navigate to `http://localhost:3000` to explore AstroCore.

---

## 📦 Building for Production

To create an optimized, minified production build:

```bash
npm run build
```

The compiled output will be generated inside the `dist/` directory.

### Previewing the Production Build Locally
```bash
npm run preview
```

---

## 🌐 Deployment (cPanel / Apache / Vercel / Netlify)

### Deploying to cPanel / Apache
1. Run `npm run build` locally.
2. Upload the contents of the `dist/` folder into your cPanel `public_html` directory (or subdomain folder).
3. Ensure the included `.htaccess` file is uploaded to handle SPA client-side routing:
   ```apache
   <IfModule mod_rewrite.c>
     RewriteEngine On
     RewriteBase /
     RewriteRule ^index\.html$ - [L]
     RewriteCond %{REQUEST_FILENAME} !-f
     RewriteCond %{REQUEST_FILENAME} !-d
     RewriteRule . /index.html [L]
   </IfModule>
   ```

### Deploying to Vercel or Netlify
- **Vercel**: Import the GitHub repository; Vite will be auto-detected with build command `npm run build` and output directory `dist`.
- **Netlify**: Set build command to `npm run build` and publish directory to `dist`. Add a `_redirects` file with `/* /index.html 200`.

---

## 🛰️ Data Citations & Verification

All telemetry, coordinates, and historical records are cross-referenced with public scientific archives:
- **NASA Planetary Data System (PDS)**: [pds.nasa.gov](https://pds.nasa.gov/)
- **NASA Lunar Reconnaissance Orbiter (LRO / LROC)**: Landing site imaging and retroreflector verification.
- **NASA Mars Reconnaissance Orbiter (HiRISE)**: High-resolution surface verification of Mars rovers and landers.
- **NASA Jet Propulsion Laboratory (JPL)**: Mission timelines, odometer readings, and telemetry logs.
- **Soviet Space Program Archives**: Luna 17 / Lunokhod 1 coordinates and traverse logs.

---

## 📜 License

This project is open-source under the [MIT License](LICENSE).

---

## 👨‍🚀 Acknowledgments

- Developed for the **NASA International Space Apps Challenge 2026**.
- Dedicated to the engineers, scientists, and flight controllers whose machines continue to stand silent watch on distant worlds.
