# 👋 Olá, eu sou o Isaque!  

💻 Estudante 2ºano CEEP de Desenvolvimento de Sistemas  
📚 Atualmente aprendendo **JavaScript**  
⚡ Apaixonado por vôlei🏐, xadrez♟ 

---

## 🚀 Tecnologias e Ferramentas  
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)  
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)  
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)  
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)  
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  

---

## 📌 Projetos em Destaque  
🔹 [**Meu Projeto 1**](https://github.com/seu-usuario/projeto1) - Pequena descrição do projeto  
🔹 [**Meu Projeto 2**](https://github.com/seu-usuario/projeto2) - Pequena descrição do projeto  

---

## 📊 Estatísticas do GitHub  
![Isaque's GitHub stats](https://github-readme-stats.vercel.app/api?username=canetinha1&show_icons=true&theme=midnight-purple)
![Linguagens mais usadas](https://github-readme-stats.vercel.app/api/top-langs/?username=canetinha1&layout=compact&theme=midnight-purple)  

---

## 📬 Entre em Contato  
<div align="left">
  <a style="text-decoration: none; !important" href="https://www.instagram.com/t0rres.isaq/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="instagram logo"  />
  </a>
  <a style="text-decoration: none; !important" href="mailto:isaquefelipe420@gmail.com" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="gmail logo"  />
  </a>
</div>

---

🛠️ Sempre buscando evoluir e criar algo novo! 🚀  
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
          github_user_name: canetinha1
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
