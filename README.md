### oiii ╰(*°▽°*)╯

- 🙂 Estudante de ADS
- 🤫 Estudando java e python
- 😁 Tenho 18 anos de idade
- 📫 Meu email-laura0719carvalho@gmail.com
- 😄 Meu insta lauracarvalho28__


           nome: Gerar dados

em:
  agendamento: # executar a cada 12 horas
    - cron: "* */12 * * *"
  workflow_dispatch:

empregos:
  construir:
    nome: Trabalhos para atualizar dados
    runs-on: ubuntu-mais recente
    passos:
      # Animação de cobras
      - usos: Platane/snk@master
        id: cobra-gif
        com:
          github_user_name: lauracar2
          svg_out_path: dist/github-contribution-grid-snake.svg

      - usa: crazy-max/ghaction-github-pages@v2.1.3
        com:
          target_branch: saída
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ segredos. GITHUB_TOKEN }}       
