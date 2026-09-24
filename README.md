# 41 Little Gifts — Birthday Bunny 🎂🐰

A small browser-based birthday game built with **Three.js**. Explore a meadow as a purple bunny, find all **41 gifts**, and read the little messages attached to them.

## Features

- 🎁 41 collectible birthday gifts
- 🐰 Cute purple bunny character
- 🏃 Walking/running animation with moving legs and a small body bounce
- 🌳 Randomly placed trees
- 🌱 Dense clustered grass instead of isolated grass sticks
- ✨ Gift animations and collection effects
- 🖱️ Desktop FPS-style controls
- 📱 Mobile joystick and swipe-to-look controls
- 🔒 Pointer-lock mouse look on desktop
- 🌈 Procedural rolling meadow terrain
- 💜 Birthday messages for each gift
- 📦 No build step required — it runs directly in a modern browser

## Controls

### Desktop

- **W / ↑** — move forward
- **S / ↓** — move backward
- **A / ←** — move left
- **D / →** — move right
- **Mouse** — look around within a 180° horizontal view
- **Click the game** — enable mouse/pointer lock
- **Esc** — release pointer lock

### Mobile

- **Left joystick** — move
- **Swipe on the right side** — look around within a 180° horizontal view
- **Tap Start** — begin the game

## Run locally

The game is a single HTML file, but using a small local web server is recommended because the page imports Three.js as an ES module.

### Option 1 — Python

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

### Option 2 — VS Code

Install the **Live Server** extension and open `index.html` with Live Server.

## GitHub Pages

1. Create a new GitHub repository.
2. Upload:
   - `index.html`
   - `README.md`
3. Commit the files.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
6. Save and wait for GitHub Pages to publish the site.

Your game should then be available at your GitHub Pages URL.

## Project structure

```text
41-little-gifts/
├── index.html
└── README.md
```

## Technology

- HTML5
- CSS3
- JavaScript
- [Three.js](https://threejs.org/)

Three.js is loaded from jsDelivr, so an internet connection is required when the game starts.

## Notes

The game uses procedural geometry for the bunny, terrain, trees, grass, gifts, and other scenery. There are no separate image, model, or texture assets required.

The game is intended as a personal birthday project and can be customized directly in `index.html`.

## Customizing the game

Useful areas to edit in `index.html` include:

- **Birthday messages** — edit the gift/message data.
- **Bunny appearance** — edit `makeBunny()`.
- **Terrain** — edit `terrainHeight()`.
- **Grass** — edit `addGrass()`.
- **Trees** — edit `addTrees()`.
- **Movement speed** — change the `speed` value in `update()`.
- **Colors and lighting** — adjust the Three.js materials and lights.

Enjoy the birthday adventure! 💜🐰🎁
