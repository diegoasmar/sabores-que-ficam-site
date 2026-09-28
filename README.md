# Sabores que Ficam — site

Site de uma página da **Sabores que Ficam** (Chef Macuta), catering e buffet em Lisboa. HTML, CSS e JavaScript num só ficheiro (`index.html`), sem build. Publicado com GitHub Pages em https://www.saboresqueficam.pt/ (e também em https://diegoasmar.github.io/sabores-que-ficam-site/).

Cores: branco, preto e caramelo (o mesmo caramelo do logótipo, `#C2935B`). Tipografia: Libre Caslon (títulos e texto) e Montserrat (etiquetas e botões), do Google Fonts.

## Ficheiros

Fotos e vídeos ficam na raiz do repositório, ao lado do `index.html`. Para trocar uma foto ou um vídeo, basta substituir o ficheiro mantendo o mesmo nome.

`sabores-logo.png` é o logótipo, que aparece sempre sobre caramelo, como foi desenhado.

`hero-reel.mp4` e `hero-reel-mobile.mp4` são o vídeo do topo: no computador aparece em três painéis, no telemóvel em ecrã inteiro.

`buffet-reel.mp4` e `buffet-reel-mobile.mp4` são o vídeo da secção "Como funciona".

`chef-portrait.jpg` é a foto da introdução. A galeria usa `chef-tray.jpg`, `gallery-prosciutto-1.jpg`, `gallery-prosciutto-2.jpg`, `gallery-blue-sliders.jpg`, `hero-tray.jpg`, `buffet-poster.jpg`, `food-cake.jpg` e `food-charcuterie.jpg`.

## Serviços e preços

A secção `id="servicos"` mostra os kits e a carta apenas com as descrições (sem valores); o site não apresenta preços, só o que está incluído em cada opção. Para editar o texto de um kit ou de um item da carta, procurar o nome no `index.html` e alterar o texto ao lado.

O orçamento é sempre calculado à medida, pelo pedido no formulário.

## Formulário de orçamento

Pede nome, telemóvel, email (opcional), tipo de evento, data, número de pessoas, o que procura, onde será o evento, cidade e detalhes. Ao enviar, o pedido é entregue por email através do serviço [FormSubmit](https://formsubmit.co/), sem precisar de servidor próprio:

- Vai para `diego.asmar@gmail.com`, com cópia (`cc`) para `suporte@tenantflow.com.br`.
- O endereço de email do próprio serviço fica configurado no `index.html`, dentro do `<script>`, nas constantes `LEAD_TO` e `LEAD_CC`.
- Tem um campo escondido (`_honey`) para reduzir spam automático.

**Importante — ativação do FormSubmit:** da primeira vez que um pedido for enviado para `diego.asmar@gmail.com`, o FormSubmit manda um email de confirmação/ativação para essa caixa de correio, que tem de ser aberto e confirmado (um clique) antes de os pedidos seguintes chegarem de facto. Sem esse passo, o formulário parece funcionar no site (mostra a mensagem de sucesso) mas o primeiro email de teste pode não aparecer até a ativação ser feita — por isso convém fazer um pedido de teste assim que o site for divulgado e confirmar essa ativação.

## Domínio

O domínio `saboresqueficam.pt` já está apontado para este GitHub Pages (DNS configurado na Amen.pt) e o site responde em `https://www.saboresqueficam.pt/`. Os registos de email do domínio (MX, SPF, DKIM, etc.) não foram alterados.
