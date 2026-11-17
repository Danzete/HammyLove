# HammyLove 🐹💕

Site estático (um único `index.html`, sem dependências nem build).

## Rodar localmente
Opção 1: dê dois cliques em `index.html`.

Opção 2 (servidor local):
```bash
python -m http.server 8080
# abra http://localhost:8080
```

## Deploy no GitHub Pages
1. Crie um repositório vazio no GitHub (ex.: `hammylove`), sem README.
2. Na pasta do projeto:
```bash
git init
git add .
git commit -m "HammyLove: primeira versão"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/hammylove.git
git push -u origin main
```
3. No GitHub: **Settings > Pages > Build and deployment > Source: GitHub Actions**.
4. Aba **Actions**: aguarde o workflow "Deploy GitHub Pages" ficar verde.
5. Site no ar em `https://SEU_USUARIO.github.io/hammylove/`.

Cada `git push` na `main` publica de novo.
