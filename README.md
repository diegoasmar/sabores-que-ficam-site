# Sabores que Ficam — Site

Site institucional de uma página (landing page) para captação de leads da **Sabores que Ficam** (Chef Macuta — catering/buffet em Lisboa).

Feito em HTML/CSS/JS puro, sem build step — basta editar o `index.html` num editor de texto e publicar. Design flat (sem gradientes/efeitos "de IA"), só três cores: branco, preto e caramelo, com logo, fotos e menu reais da Chef Macuta.

## Estrutura

```
sabores-que-ficam/
├── index.html   ← todo o site (estrutura, estilo e scripts)
├── images/      ← logo e fotos reais (ver lista abaixo)
├── videos/      ← vídeos em loop (topo da página e secção "Uma mesa a ganhar vida")
└── README.md
```

### Vídeos

Há dois vídeos em loop, sem som, feitos a partir de clips reais da Chef Macuta:

- `videos/hero-reel.mp4` (+ `hero-reel-mobile.mp4`) — no topo da página, a Chef a preparar e a servir petiscos.
- `videos/buffet-reel.mp4` (+ `buffet-reel-mobile.mp4`) — na secção "Uma mesa a ganhar vida", um relance de uma mesa de buffet completa.

Cada vídeo tem duas versões — uma mais leve para telemóvel e outra para computador — trocadas automaticamente pelo próprio navegador (não precisa de fazer nada). Para trocar algum vídeo, basta substituir o ficheiro mantendo o mesmo nome (ou mudar o `src` dentro da tag `<video>` correspondente no `index.html`).

### Imagens usadas

| Ficheiro | Onde aparece |
|---|---|
| `sabores-logo.png` | Cabeçalho e rodapé |
| `hero-tray.jpg` | Topo da página e galeria |
| `chef-portrait.jpg` | Secção "Sobre a Chef" |
| `chef-tray.jpg` | Galeria |
| `gallery-prosciutto-1.jpg` / `gallery-prosciutto-2.jpg` | Galeria |
| `gallery-blue-sliders.jpg` | Galeria |
| `food-fish.jpg`, `food-charcuterie.jpg`, `food-salgados.jpg`, `food-brigadeiros.jpg`, `food-cake.jpg` | Fotos entre as secções do Menu & Preços, e galeria |

## O que falta preencher antes de publicar "a sério"

1. **Número de WhatsApp** — no fim do `index.html`, dentro da tag `<script>`, existe:
   ```js
   const WHATSAPP_NUMBER = "351900000000"; // TODO: substituir pelo número real
   ```
   Trocar pelo número real, no formato internacional só com dígitos (ex.: `351912345678`). Todos os botões "Pedir Orçamento" / "Falar no WhatsApp" já usam essa variável automaticamente.

2. **Preços do menu** — os preços em `#menu` foram tirados dos cardápios/flyers reais enviados. Se algum preço mudar, basta procurar o item pelo nome no `index.html` e editar o valor ao lado (formato `65€`).

3. **Depoimentos reais** — a secção de prova social aponta para o destaque "Feedback" do Instagram (não inventamos citações). Se quiser depoimentos escritos diretamente no site, envie os textos reais dos clientes para adicionar.

4. **Mais fotos/vídeos** — para trocar ou adicionar:
   - Colocar o ficheiro dentro da pasta `images/`;
   - Usar `<img src="images/nome-do-ficheiro.jpg" alt="descrição">` no sítio desejado;
   - Para vídeo: `<video src="images/video-1.mp4" autoplay muted loop playsinline></video>`.

## GitHub Pages

O repositório já existe em `github.com/diegoasmar/sabores-que-ficam-site` com o `index.html` publicado. Falta só enviar as pastas `images/` e `videos/` (arrastar os ficheiros em **Add file → Upload files**), e depois ativar em **Settings → Pages** (branch `main`, pasta `/ (root)`). O site fica disponível em `https://diegoasmar.github.io/sabores-que-ficam-site/`.

Quando o domínio `saboresqueficam.pt` estiver pronto, basta configurá-lo em **Settings → Pages → Custom domain** e apontar o DNS do domínio para o GitHub Pages.

## Editar depois (sem precisar de programador)

- Textos: procurar a frase no `index.html` e editá-la diretamente entre as tags.
- Cores: no topo do ficheiro há um bloco `:root { --caramel: ...; --ink: ...; }` — mudar os códigos de cor ali muda o site inteiro.
- Secções: cada parte do site está dentro de um `<section>` comentado (ex. `<!-- ===== SOBRE ===== -->`), facilitando encontrar o que editar.
