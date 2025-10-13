<!--
  Profile README for a gothic, game-dev vibe.
  Replace USERNAME with your GitHub handle.
  Place your header art at: assets/gothic-banner.png
-->

<div align="center">
  <!-- Dark/Light header banner -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/gothic-banner.png" />
    <source media="(prefers-color-scheme: light)" srcset="assets/gothic-banner.png" />
    <img alt="Gothic banner with moonlit castle and bats" src="assets/gothic-banner.png" width="100%">
  </picture>
</div>

<h1 align="center">Wieniec</h1>
<p align="center"><em>Stoic game developer crafting atmospheric worlds in Godot.</em></p>

<p align="center">
  <!-- Godot badge -->
  <a href="https://godotengine.org">
    <img alt="Made with Godot" src="https://img.shields.io/badge/Made%20with-Godot-478CBF?style=flat&logo=godot%20engine&logoColor=white">
  </a>
  <!-- Optional extra badges (uncomment if wanted) -->
  <!-- <img alt="Arch Linux" src="https://img.shields.io/badge/OS-Arch%20Linux-1793D1?logo=arch-linux&logoColor=white"> -->
  <!-- <img alt="Fish shell" src="https://img.shields.io/badge/Shell-fish-00A6FF?logo=fish-shell&logoColor=white"> -->
</p>

---

## 🕯️ About
I build games, tools and little experiments. I like moody lighting, readable code, and mechanics that feel good.

- Engine: **Godot 4.x**
- Focus: **systems design**, **AI behaviors**, **procedural level dressing**
- Platform: **Linux (Arch)** with **fish** shell

---

## ⚒️ Currently Building
> Working title: **TBA**  
Dark survival micro-immersion prototype in Godot.

- Core loop: stealthy scavenging, stamina-pacing combat
- Systems: lightweight inventory, noise/vision cones, dynamic fog volumes
- Status: greybox maps; AI patrol + investigate; interaction bus

**Dev Notes**
- [ ] Scene tree refactor (signals vs. event bus)
- [ ] Finite State Machine for enemies (patrol → suspect → pursue → search)
- [ ] Save system (binary blobs with versioning)

---

## ✅ Completed (to showcase)
> You said you’ve got “nothing yet.” No problem. Pin these as soon as they exist.

- **TBH: Project Slot #1**  
  A tiny Godot demo that proves out your input, camera, and interaction pattern.

- **TBH: Project Slot #2**  
  A tool or plugin: e.g., “Godot Fog Volumes Tweaker,” “Dialogue Graph Exporter.”

- **TBH: Project Slot #3**  
  A microgame: 2–5 minutes of polished mechanics with sound and juice.

---

## 🧰 Tech Stack
<p>
  <!-- Swap or trim as needed -->
  <img src="https://skillicons.dev/icons?i=godot,linux,git,github,cpp,cs,python,js" alt="Tech icons">
</p>

---

## 📈 Stats
<!-- Replace USERNAME with your handle -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&theme=dracula&hide_title=true" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&hide_title=true" />
    <img alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&hide_title=true" />
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com?user=USERNAME&theme=dark&hide_border=true" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-streak-stats.herokuapp.com?user=USERNAME&hide_border=true" />
    <img alt="GitHub streak" src="https://github-readme-streak-stats.herokuapp.com?user=USERNAME&hide_border=true" />
  </picture>
</p>

---

## 🐍 Contribution Snake
<!-- If you enable the action below, these files will exist at ./dist/ -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="dist/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="dist/github-snake.svg" />
    <img alt="Contribution snake" src="dist/github-snake.svg" />
  </picture>
</p>

---

## ✒️ Design Pillars
- **Monochrome first,** with one accent (deep violet or cyan)
- **Readable type,** strong spacing, minimal ornaments
- **Diegetic UI:** tooltips and HUD edges feel like props

---

## 📫 Contact
- **Itch:** _tba_
- **X/Twitter:** _tba_
- **Email:** _tba_

---

### How to Use (quick)
1. Create a repo named exactly `USERNAME`.
2. Add this file as `README.md`.
3. Put your banner at `assets/gothic-banner.png`.  
4. Replace `USERNAME` in stat URLs.
5. Optionally add the contribution snake workflow (below) to auto-generate `dist/github-snake*.svg`.

<details>
<summary>Optional: Contribution Snake GitHub Action</summary>

Create `.github/workflows/snake.yml`:

```yaml
name: Generate Snake
on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
      - name: Push snake files
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
</details>