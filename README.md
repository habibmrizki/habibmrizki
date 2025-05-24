<h1 align="center">
    <img src="https://readme-typing-svg.herokuapp.com/?font=Righteous&size=35&center=true&vCenter=true&width=500&height=70&duration=4000&lines=Hi+There!+👋;+I'm+Habib+Muhammad+Rizki!;" />
</h1>

<h3 align="center">A passionate software developer from Indonesia INA</h3>

<br/>

<div align="center">
 
 🔭 I’m currently working on **a marketplace**
 
 🌱 I’m currently learning **Docker.**

💬 Ask me about **Node.js, React, SQL... or anything [here](https://github.com/habibmrizki)**

⚡ Fun fact **Game of Thrones Night's Watch cloaks are made from Ikea rugs**

 </div>
 
<div align="center"> 
  <a href="https://www.linkedin.com/in/habib-rizki/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank" />
  </a>
</div>

 <hr/>
 
<h2 align="center">⚒️ Languages-Frameworks-Tools ⚒️</h2>
<br/>
<div align="center">
    <img src="https://skillicons.dev/icons?i=react,bootstrap,html,css,vscode,github,figma,tailwind,git,javascript,nodejs,go" />
</div>

<br/>
<hr/>

<div align="center">
  <h2>🐍 My Contributions 🐍</h2>
  <br>
   
![github contribution grid snake animation](https://raw.githubusercontent.com/fulsep/fulsep/output/github-snake-dark.svg#gh-dark-mode-only)![github contribution grid snake animation](https://raw.githubusercontent.com/fulsep/fulsep/output/github-snake.svg#gh-light-mode-only)

  <br/><br/><br/>
</div>


name: Generate pacman animation

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"

  workflow_dispatch:

  push:
    branches:
    - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: generate pacman-contribution-graph.svg
        uses: abozanona/pacman-contribution-graph@main
        with:
          github_user_name: ${{ github.repository_owner }}


      - name: push pacman-contribution-graph.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

<hr/>

<h2 align="center">⚡ Stats ⚡</h2>
<br>
<div align=center>
     <img width=390 src="https://github-readme-stats.vercel.app/api?username=habibmrizki&theme=react&show_icons=true&hide_border=true&count_private=true" alt="streak stats"/>
         <img width=390 src="https://github-readme-streak-stats.herokuapp.com/?user=habibmrizki&theme=react&hide_border=true" alt="streak stats"/>
  <br/>
     <img width=390 src="https://github-readme-stats.vercel.app/api/top-langs/?username=habibmrizki&theme=react&show_icons=true&hide_border=true&layout=compact" alt="streak stats"/>

</div>

<br/><br/>

<hr/>

<br/>
