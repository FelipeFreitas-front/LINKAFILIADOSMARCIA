# Achadinhos da Márcia

Site vitrine (estático, sem build) com os produtos da Shopee indicados pela Márcia.
Detalhes de conteúdo e de como adicionar produtos: `CONTEXTO-achadinhos-da-marcia.md`.

## Arquivos

| Arquivo | Para que serve |
|---|---|
| `index.html` | O site inteiro (CSS, JS e dados embutidos) |
| `404.html` | Página de "não encontrado" |
| `favicon.ico`, `favicon.svg` | Ícone da aba do navegador |
| `apple-touch-icon.png` | Ícone ao salvar na tela inicial do iPhone |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | Ícones do Android / PWA |
| `site.webmanifest` | Nome, cores e ícones para "Adicionar à tela inicial" |
| `og-image.jpg` | Imagem que aparece ao compartilhar o link (WhatsApp, Instagram, Facebook) |
| `robots.txt`, `sitemap.xml` | Indexação no Google |
| `vercel.json` | Cabeçalhos de segurança, cache e URLs limpas |
| `.vercelignore` | Arquivos que não vão para o site publicado |

## Publicar na Vercel

**Opção 1: arrastar a pasta**
1. Entre em vercel.com → *Add New* → *Project*.
2. Envie esta pasta (ou importe o repositório do GitHub).
3. *Framework Preset*: **Other**. Deixe *Build Command* e *Output Directory* vazios.
4. Nome do projeto: `achadinhos-da-marcia` (assim o endereço fica `achadinhos-da-marcia.vercel.app`).

**Opção 2: linha de comando**
```bash
npm i -g vercel
vercel          # primeira vez, cria o projeto
vercel --prod   # publica em produção
```

## Se o endereço for outro

Troque `https://achadinhos-da-marcia.vercel.app` pelo endereço real em:
`index.html` (canonical e metatags og/twitter), `robots.txt` e `sitemap.xml`.

## Testar localmente
```bash
npx serve .
```
