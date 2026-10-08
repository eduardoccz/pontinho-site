# Placar do Pontinho

Placar para o jogo de baralho Pontinho, com as regras da casa: coringa 20, ás 15, K 13, Q 12, J 11 e as demais cartas valem o número.

É um site estático de um arquivo só (`index.html`), sem build e sem servidor. As partidas ficam guardadas no navegador de cada aparelho (`localStorage`).

## Publicar no GitHub Pages

1. No repositório, abra Settings > Pages e escolha publicar a partir do branch `main`, pasta raiz.
2. Em Custom domain, informe `pontinho.cazangi.com` (o arquivo `CNAME` já traz esse valor).
3. No DNS do domínio, crie um registro CNAME com nome `pontinho` apontando para `eduardoccz.github.io`.
4. Quando o certificado estiver pronto, marque Enforce HTTPS.

## Arquivos

- `index.html`: a página inteira (estilos e código juntos).
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `icon.svg`: ícones e dados para "Adicionar à tela inicial".
- `CNAME`: o domínio personalizado.
- `.nojekyll`: faz o GitHub Pages servir os arquivos como estão.
