# Sabores que Ficam — site

Site de uma página da **Sabores que Ficam** (Chef Macuta), catering e buffet em Lisboa. HTML, CSS e JavaScript num só ficheiro (`index.html`), sem build. Publicado com GitHub Pages em https://diegoasmar.github.io/sabores-que-ficam-site/

Cores: branco, preto e caramelo (o mesmo caramelo do logótipo, `#C2935B`). Tipografia: Libre Caslon (títulos e texto) e Montserrat (etiquetas e botões), do Google Fonts.

## Ficheiros

Fotos e vídeos ficam na raiz do repositório, ao lado do `index.html`. Para trocar uma foto ou um vídeo, basta substituir o ficheiro mantendo o mesmo nome.

`sabores-logo.png` é o logótipo, que aparece sempre sobre caramelo, como foi desenhado.

`hero-reel.mp4` e `hero-reel-mobile.mp4` são o vídeo do topo: no computador aparece em três painéis, no telemóvel em ecrã inteiro.

`buffet-reel.mp4` e `buffet-reel-mobile.mp4` são o vídeo da secção "Como funciona".

`chef-portrait.jpg` é a foto da introdução. A galeria usa `chef-tray.jpg`, `gallery-prosciutto-1.jpg`, `gallery-prosciutto-2.jpg`, `gallery-blue-sliders.jpg`, `hero-tray.jpg`, `buffet-poster.jpg`, `food-cake.jpg` e `food-charcuterie.jpg`.

## Antes de divulgar: número de WhatsApp

No fim do `index.html`, dentro de `<script>`, está esta linha:

```js
const WHATSAPP = "351900000000"; // TODO
```

Trocar pelo número real, só dígitos e com `351` à frente (por exemplo `351912345678`). O formulário de orçamento e todos os links de WhatsApp usam este número.

## Preços

Estão na secção `id="ementa"`. Para mudar um preço, procurar o nome do prato no `index.html` e alterar o valor ao lado.

## Formulário de orçamento

Pede nome, telemóvel, tipo de evento, data, número de pessoas, o que procura, onde será o evento, cidade e detalhes. Ao enviar, abre o WhatsApp com uma mensagem já escrita com essas respostas; o cliente só tem de carregar em enviar. Não precisa de servidor.

## Domínio

Quando `saboresqueficam.pt` estiver pronto: Settings, Pages, Custom domain, e apontar o DNS do domínio para o GitHub Pages.
