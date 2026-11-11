# Pixel Fury (protótipo v0.9.7)

Jogo de plataforma 2D de tiro, feito em HTML5 Canvas + JavaScript (um único `index.html`).
Esta pasta é a versão PWA: pode ser instalada no celular ou no computador e funciona offline.

## Publicar no GitHub Pages
1. Suba todos os arquivos desta pasta para a raiz do repositório (branch `main`).
2. No repositório: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
3. Em 1 a 2 minutos o jogo fica em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Instalar
- **Android (Chrome):** menu ⋮ → *Instalar app* / *Adicionar à tela inicial*.
- **iPhone (Safari):** botão Compartilhar → *Adicionar à Tela de Início*.
- **Computador (Chrome/Edge):** ícone de instalar na barra de endereço.

## Atualizações
O jogo busca a versão nova sempre que abre com internet. Se não aparecer, feche e abra o app de novo.

## Telemetria e save (debug oculto)
No menu principal, **segure a engrenagem ⚙️ por 5 segundos**. Lá dá pra:
- **Enviar/Copiar runs novas:** exporta só as partidas desde a última exportação (arquivo `.json` para mandar ao Claude).
- **Enviar/Copiar todas:** exporta todas as partidas salvas (até 150).
- **Copiar save / Colar save:** leva o progresso de um aparelho (ou do artifact) para outro.
- **Apagar telemetria.**

## Arquivos
- `index.html`: o jogo inteiro.
- `manifest.webmanifest`: nome, ícones e modo tela cheia/horizontal.
- `sw.js`: service worker (offline + atualização automática).
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png`: ícones do app (ficam soltos na raiz, sem pasta, para funcionar mesmo subindo pelo iPhone).
