# Placar do Pontinho

Placar para o jogo de baralho Pontinho, com as regras da casa: coringa 20, ás 15, K 13, Q 12, J 11 e as demais cartas valem o número.

É um site estático de um arquivo só (`index.html`), sem build e sem servidor. As partidas ficam guardadas no navegador de cada aparelho (`localStorage`).

## Publicar no GitHub Pages

O deploy é feito pelo workflow `.github/workflows/deploy.yml`, o mesmo do repositório `eduardoccz.github.io`: a cada push no branch `main`, o GitHub Actions publica o site.

Na primeira vez:

1. No repositório, abra Settings > Pages e, em Source, selecione **GitHub Actions**.
2. Em Custom domain, informe `pontinho.cazangi.com`.
3. No DNS do domínio, crie um registro CNAME com nome `pontinho` apontando para `eduardoccz.github.io`.
4. Quando o certificado estiver pronto, marque Enforce HTTPS.

## Arquivos

- `index.html`: a página inteira (estilos e código juntos).
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `icon.svg`: ícones e dados para "Adicionar à tela inicial".
- `CNAME`: o domínio personalizado.
- `.nojekyll`: faz o GitHub Pages servir os arquivos como estão, caso o deploy seja feito por branch.
- `.github/workflows/deploy.yml`: deploy automático pelo GitHub Actions.
