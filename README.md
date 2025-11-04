<h1 align="center">Hi there 👋, I'm Ajiputra!</h1>
<h3 align="center">A passionate developer from Indonesia</h3>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=ajiputra001&style=flat-square&color=blue" alt="ajiputra001 profile views" />
</p>

---

<h2 align="center">About Me</h2>

- 🔭 I’m currently working on **Open Source Projects**.
- 🌱 I’m currently learning **new development techniques**.
- 💬 Ask me about **JavaScript, Linux, or any tech-related topics!**

---

<h2 align="center">Technologies I Use</h2>

<div align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=js,vscode" />
  </a>
</div>

---

<h2 align="center">My GitHub Stats</h2>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=ajiputra001&show_icons=true&theme=gotham&hide_border=true&rank_icon=github" height="150" alt="stats graph" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=ajiputra001&layout=compact&langs_count=5&theme=gotham&hide_border=true" height="150" alt="languages graph" />
</div>

---

<div align="center">
  <a href="https://github.com/ajiputra001" target="_blank">
    <img src="https://img.shields.io/badge/Follow%20me%20on%20GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Follow me on GitHub" />
  </a>
  <a href="https://t.me/ajiputra001" target="_blank"> 
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" />
  </a>
</div>

---

<div align="center">
  <h3>Thanks for visiting!</h3>
  <img src="https://raw.githubusercontent.com/ajiputra001/ajiputra001/output/snake.svg" alt="Snake animation" />
</div>
# snake.yml
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *" # Runs every day at midnight UTC
  workflow_dispatch: # Allows manual trigger

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Generate Snake SVG
        uses: Platane/snk@v3
        with:
          github_user_name: ajiputra001 # Ganti dengan username GitHub Anda
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
