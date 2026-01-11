<!-- ===== Typing Header ===== -->
<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=28&duration=4000&color=00F7A5&center=true&vCenter=true&width=600&lines=Hi+There!+👋;I'm+AQSA KHAN;Full+Stack+Developer;UI/UX+Designer;WordPress+Expert" />
</p>

<!-- ===== Profile Stats ===== -->
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=aqsa2403&style=flat-square" alt="Profile Views"/>
  <img src="https://img.shields.io/github/followers/aqsa2403?style=social" alt="Followers"/>
  <img src="https://img.shields.io/github/stars/aqsa2403?style=social" alt="Stars"/>
</p>

---

### 🧾 About Me
- 💻 Web Developer (WordPress + PHP + JS + Tailwind)
- 🎨 UI/UX Designer (Figma + Illustrator)
- 🌱 Learning AI & Cloud
- 📌 Based in Pakistan 🇵🇰
- 📬 Reachme: **aqsaakhan2244@gmail.com**

---

### 🛠 Tech Skills
<p align="center">
 <img src="https://img.shields.io/badge/HTML5-fff?style=for-the-badge&logo=html5&logoColor=E44D26" />
 <img src="https://img.shields.io/badge/CSS3-fff?style=for-the-badge&logo=css3&logoColor=1572B6" />
 <img src="https://img.shields.io/badge/JavaScript-fff?style=for-the-badge&logo=javascript&logoColor=F7DF1E" />
 <img src="https://img.shields.io/badge/PHP-fff?style=for-the-badge&logo=php&logoColor=787CB5" />
 <img src="https://img.shields.io/badge/MySQL-fff?style=for-the-badge&logo=mysql&logoColor=4479A1" />
 <img src="https://img.shields.io/badge/WordPress-fff?style=for-the-badge&logo=wordpress&logoColor=21759B" />
 <img src="https://img.shields.io/badge/TailwindCSS-fff?style=for-the-badge&logo=tailwindcss&logoColor=38B2AC" />
 <img src="https://img.shields.io/badge/Figma-fff?style=for-the-badge&logo=figma&logoColor=F24E1E" />
 <img src="https://img.shields.io/badge/Illustrator-fff?style=for-the-badge&logo=adobeillustrator&logoColor=FF9A00" />
</p>

---

### 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=aqsa2403&show_icons=true&theme=radical" height="160"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=aqsa2403&theme=radical" height="160"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=aqsa2403&layout=compact&theme=radical" height="160"/>
</p>

---

### 🏆 Trophies
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=aqsa2403&theme=radical&margin-w=15&margin-h=15" />
</p>

---

### 🐍 Snake Contributions
<p align="center">
  <img src="https://raw.githubusercontent.com/aqsa2403/aqsa2403/output/github-contribution-grid-snake.svg" />
</p>

---

### 🌐 Connect With Me
<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/LinkedIn-fff?style=for-the-badge&logo=linkedin&logoColor=0A66C2"/></a>
  <a href="#"><img src="https://img.shields.io/badge/Twitter-fff?style=for-the-badge&logo=twitter&logoColor=1DA1F2"/></a>
  <a href="#"><img src="https://img.shields.io/badge/Instagram-fff?style=for-the-badge&logo=instagram&logoColor=E4405F"/></a>
  <a href="#"><img src="https://img.shields.io/badge/Behance-fff?style=for-the-badge&logo=behance&logoColor=1769FF"/></a>
  <a href="#"><img src="https://img.shields.io/badge/Dribbble-fff?style=for-the-badge&logo=dribbble&logoColor=EA4C89"/></a>
</p>

<p align="center">⭐ If you like my work, consider following!</p>

name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: Platane/snk@v3
        with:
          github_user_name: aqsa2403
          outputs: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
