name: Generate Contribution Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest

    steps:
      - name: Generate Snake
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: abhishekyadav1118
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark

      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


          ---

## 📊 GitHub Statistics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=abhishekyadav1118&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=abhishekyadav1118&layout=compact&theme=tokyonight&hide_border=true" />
</p>

---

## 🔥 GitHub Streak

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=abhishekyadav1118&theme=tokyonight&hide_border=true" />
</p>

---

## 🐍 Contribution Snake

<p align="center">
  <img src="https://raw.githubusercontent.com/abhishekyadav1118/abhishekyadav1118/output/github-snake.svg" />
</p>

---

## 🌐 My Portfolio

<p align="center">
  <a href="https://portfolio-ten-xi-qdq1qoacsx.vercel.app/">
    🚀 <b>View My Portfolio</b>
  </a>
</p>

---

## 🤝 Let's Connect

<p align="center">

<a href="https://github.com/abhishekyadav1118">
  <img src="https://img.shields.io/badge/GitHub-abhishekyadav1118-black?style=for-the-badge&logo=github" />
</a>

<a href="https://www.linkedin.com/in/abhishek-yadav-247858373/">
  <img src="https://img.shields.io/badge/LinkedIn-Abhishek_Yadav-blue?style=for-the-badge&logo=linkedin" />
</a>

<a href="mailto:abhishekyadav4203689@gmail.com">
  <img src="https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail" />
</a>

</p>
