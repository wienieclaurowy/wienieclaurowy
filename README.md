<div align="center">
  <!-- Dark/Light header banner -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/gothic-banner.png" />
    <source media="(prefers-color-scheme: light)" srcset="assets/gothic-banner.png" />
    <img alt="Gothic banner with moonlit castle and bats" src="assets/gothic-banner.png" width="100%">
  </picture>
</div>

<h1 align="center">Wieniec</h1>
<p align="center"><em>Game developer crafting atmospheric worlds in Godot.</em></p>

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
I build games, tools and little experiments. I like moody lighting, readable code, and mechanics that feel gooooood.

- Engine: **Godot 4.x**
- Focus: **systems design**, **AI behaviors**, **procedural level dressing**
- Platform: **Linux (Arch)**

---

## ⚒️ Currently Building
> **TBA**
---

## ✅ Completed (to showcase)
> **TBA**
---

## 🧰 Tech Stack
<p>
  <!-- Swap or trim as needed -->
  <img src="https://skillicons.dev/icons?i=linux,godot,git,github,cs,python,js" alt="Tech icons">
</p>

---

## 📈 Stats
<!-- Replace USERNAME with your handle -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=wienieclaurowy&show_icons=true&theme=dracula&hide_title=true" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=wienieclaurowy&show_icons=true&hide_title=true" />
    <img alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=wienieclaurowy&show_icons=true&hide_title=true" />
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com?user=wienieclaurowy&theme=dark&hide_border=true" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-streak-stats.herokuapp.com?user=wienieclaurowy&hide_border=true" />
    <img alt="GitHub streak" src="https://github-readme-streak-stats.herokuapp.com?user=wienieclaurowy&hide_border=true" />
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

## 📫 Contact
- **Itch:** _tba_
- **X/Twitter:** _tba_
- **Email:** _tba_

---

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
        uses: crazy-max/ghacti on-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
</details>