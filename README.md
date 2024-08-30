 ## Olá! Eu sou o Kaique Rodrigues

- 🔭 Atualmente trabalho com mecânica industrial
- 🌱 Estou estudando Python e JavaScript desenvolvendo projetos e PHP na faculdade
- 😄 Pronouns: Ele/Dele

<div>
  <a href="https://github.com/KaiqueRodriguesL">
  <img height="180em" src=https://github-readme-stats.vercel.app/api?username=KaiqueRodriguesL&show_icons=true&theme=dark&include_all_comics=true&count_private=true"/>
  <img height="180em" src=https://github-readme-stats.vercel.app/api/top-langs/?username=KaiqueRodriguesL&lauout=compact&langs_count=16&theme=dark"/>
</div>

##

https://github-readme-stats.vercel.app/api/top-langs/?username=KaiqueRodriguesL&theme=blue-green

<div style="display: inline_block"><br>
  <img align="center" alt="Kaique-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="Kaique-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Kaique-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="Kaique-Python" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
</div>

 ##

<div> 
  <a href="https://wa.me/qr/37KTO3T7GW2RP1" target="_blank"><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" target="_blank"></a>
  <a href="https://www.instagram.com/kaiquelemee/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href = "mailto:kaique.leme@outlook.com"><img src="https://img.shields.io/badge/Microsoft_Outlook-0078D4?style=for-the-badge&logo=microsoft-outlook&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/kaique-rodrigues-43b439227" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  
</div>

! [Sanek animation]https://github.com/KaiqueRodriguesL/KaiqueRodriguesL/

name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
