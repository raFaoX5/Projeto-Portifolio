# Fluxo Git (commits em inglês, uma branch por fase)

git init && git branch -M main
git add . && git commit -m "chore: initial project setup"
git remote add origin https://github.com/SEU-USUARIO/nft-cardlist.git

# Fase 1.0
git checkout -b feature/nft-card
git commit -am "feat: add NFT preview card with hover effect"
git checkout main && git merge feature/nft-card 

# Fase 1.1
git checkout -b feature/card-list
git commit -am "feat: add card list with Leonardo.ai images and animate.css"
git checkout main && git merge feature/card-list

# Fase 1.2
git checkout -b feature/header
git commit -am "feat: add header, logo and project README"
git checkout main && git merge feature/header

git push -u origin --all

# GitHub Pages: Settings > Pages > Branch: main / (root)
