# Motion em HTML

Esta pasta é a animação que nasce num arquivo e abre no navegador: texto que entra, número que conta, card que aparece, desenho que se faz na tela. Você grava essa tela e trata a gravação como um clipe no CapCut, no Premiere ou no DaVinci.

Há duas maneiras de usar:

- Abrir um exemplo pronto, trocar a frase e as cores, gravar.
- Copiar um prompt, colar no Claude e gerar uma variação. O exemplo da mesma pasta serve de referência do que o pedido descreve.

São dez pares. O prompt `01` combina com o HTML `01`, e assim por diante. Tudo isso foi escrito para este repositório. A licença MIT está na raiz.

Um outro pack, em inglês e malaio, reúne prompts abertos no repositório [sasateguh/awesome-claude-motion-prompts](https://github.com/sasateguh/awesome-claude-motion-prompts), licença CC0. Ele não foi colado aqui. Serve como leitura extra, com o crédito no [`../CREDITOS.md`](../CREDITOS.md). Os prompts que o @zeeuiux envia por mensagem direta também não estão aqui.

## Abrir um exemplo

1. Baixe o repositório (no GitHub: **Code**, depois **Download ZIP**) e extraia a pasta.
2. Entre em `motion-html/exemplos/`.
3. Abra `index.html` com dois cliques. Escolha um exemplo.
4. A animação fica em loop. Grave essa tela quando o quadro estiver limpo.

A página do GitHub mostra o código. A animação só aparece quando o arquivo abre no navegador.

## Trocar cor e frase sem programar

1. Abra o HTML num editor de texto. O Bloco de Notas serve. No Mac, o TextEdit em modo texto puro também.
2. No começo do arquivo, dentro de `:root`, estão as cores. Cada uma é um código que começa com `#`.

```css
--fundo: #14161c;      /* cor de trás */
--texto: #f3efe6;      /* cor da letra */
--destaque: #ff4b3a;   /* cor que chama a atenção */
```

3. Troque o código pela cor do seu vídeo. Salve.
4. Volte ao navegador e atualize a página.

A frase está no miolo do arquivo, entre as tags, escrita em português. Troque as palavras e mantenha o restante das tags. Se o texto for muito maior que o original, a letra pode sair do quadro: encurte a frase ou peça ao Claude uma versão com o texto novo, usando o prompt da mesma numeração.

Essas cores são uma paleta de exemplo, escolhida para o arquivo ser legível. Troque pelas cores do vídeo em que o motion vai entrar.

## Pedir uma variação ao Claude

1. Abra o arquivo em `prompts/` com o mesmo número do exemplo.
2. Copie o bloco de pedido.
3. Cole no Claude. Se quiser, troque antes a frase que está entre aspas.
4. Peça para ele devolver um único arquivo `.html`.
5. Salve como `meu-motion.html` e abra no navegador.

Cada prompt pede um HTML só, no formato vertical 1080 por 1920, sem imagem externa e com as cores fáceis de achar no topo.

## Gravar para o editor

O HTML não é um projeto do CapCut. Ele vira clipe quando você grava a tela.

1. Abra o arquivo e deixe o quadro vertical ocupando a tela. F11 esconde a barra do navegador.
2. Grave só essa região.
   - No Windows, a Barra de Jogo grava com `Win` + `Alt` + `R`.
   - No Mac, `Command` + `Shift` + `5` abre a gravação de tela.
3. Pare a gravação no fim de um ciclo, para o corte ficar fácil.
4. Importe o vídeo no editor e corte a barra preta, se a gravação pegou a mesa em volta do quadro.

O passo a passo de cada programa está em [`../fluxo-no-editor/README.md`](../fluxo-no-editor/README.md). Um render automático, sem gravar a tela, pede outras ferramentas. Este repositório não inclui esse passo.

Deixe título e frase no miolo do quadro. A faixa de cima e a de baixo do Reels ficam cobertas pela interface do aplicativo.

## Os dez pares

| Prompt | Exemplo | Família | O que você vê |
|---|---|---|---|
| [01-tipo-cinetico.md](prompts/01-tipo-cinetico.md) | [01-tipo-cinetico.html](exemplos/01-tipo-cinetico.html) | Tipo | Três palavras entram com impacto e a última ganha um risco |
| [02-faixa-destaque.md](prompts/02-faixa-destaque.md) | [02-faixa-destaque.html](exemplos/02-faixa-destaque.html) | Tipo | Uma frase na base, com uma palavra acesa de cada vez |
| [03-pergunta-e-resposta.md](prompts/03-pergunta-e-resposta.md) | [03-pergunta-e-resposta.html](exemplos/03-pergunta-e-resposta.html) | Tipo | Uma pergunta é digitada e uma resposta entra em seguida |
| [04-notas-de-corte.md](prompts/04-notas-de-corte.md) | [04-notas-de-corte.html](exemplos/04-notas-de-corte.html) | Interface | Três notas de edição empilham na tela |
| [05-checklist-do-reel.md](prompts/05-checklist-do-reel.md) | [05-checklist-do-reel.html](exemplos/05-checklist-do-reel.html) | Interface | Uma lista vai sendo marcada |
| [06-timecode-do-gancho.md](prompts/06-timecode-do-gancho.md) | [06-timecode-do-gancho.html](exemplos/06-timecode-do-gancho.html) | Dados | Um relógio conta os primeiros segundos |
| [07-barras-da-estrutura.md](prompts/07-barras-da-estrutura.md) | [07-barras-da-estrutura.html](exemplos/07-barras-da-estrutura.html) | Dados | Quatro barras de uma estrutura de roteiro |
| [08-storyboard-em-linha.md](prompts/08-storyboard-em-linha.md) | [08-storyboard-em-linha.html](exemplos/08-storyboard-em-linha.html) | Arte | Um quadro de storyboard se desenha |
| [09-fita-adesiva.md](prompts/09-fita-adesiva.md) | [09-fita-adesiva.html](exemplos/09-fita-adesiva.html) | Arte | Uma fita com uma frase pousa no centro |
| [10-arco-de-atos.md](prompts/10-arco-de-atos.md) | [10-arco-de-atos.html](exemplos/10-arco-de-atos.html) | 3D simples | Três cards, gancho, meio e fim, entram em arco |

Número, gráfico e manchete de um Reel de verdade precisam ser os seus. Os valores nestes HTML são exemplo visual para a animação funcionar. Troque antes de publicar.
