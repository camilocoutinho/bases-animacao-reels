# Bases de Animação para Reels

Efeitos de talking head e motion em HTML, para alunos de edição usarem com o Claude e terminarem no editor.

**Você grava ou pede um motion em HTML, o Claude aplica o efeito, e você termina no editor.**

Este repositório é material de apoio para quem edita vídeo. Ele explica o caminho em português, com prompts e exemplos que dá para abrir, copiar e adaptar. Você não precisa saber programar para usar.

## O que é

São duas formas de chegar num motion para Reels, e as duas terminam no editor que você já usa.

1. **Efeito em cima de um vídeo falado.** Você arrasta um MP4 vertical para o Claude Code, pede um efeito pelo nome, e recebe outro MP4 ao lado do original. A voz continua a mesma. Som de efeito e legenda entram depois, no CapCut, no Premiere ou no DaVinci.
2. **Animação feita em HTML.** Você cola um prompt, o Claude devolve um arquivo que abre no navegador, e você grava essa tela para usar como clipe de motion.

O efeito de vídeo falado vem de uma skill gratuita, mantida nos repositórios de quem a criou. Aqui está o passo a passo e o nome de cada comando. O código dessa skill fica lá, para você instalar a versão atual. As animações em HTML desta pasta são originais deste repositório: dá para abrir os exemplos agora e para pedir variações com os prompts.

## Como usar

As dez animações juntas estão na galeria: [https://camilocoutinho.github.io/bases-animacao-reels/](https://camilocoutinho.github.io/bases-animacao-reels/). O arquivo é o [`index.html`](index.html) da raiz. A página de código do GitHub mostra este texto e não roda a animação.

Baixe a pasta para o seu computador se quiser gravar ou editar os arquivos. No GitHub, use o botão verde **Code** e depois **Download ZIP**. Extraia o ZIP.

### Receita 1. Efeito no vídeo falado

Use esta receita quando a pessoa está no quadro e o efeito entra por cima da fala.

1. Instale a skill. O passo a passo, com o comando pronto, está em [`efeitos-talking-head/README.md`](efeitos-talking-head/README.md).
2. Feche o Claude Code e abra de novo.
3. Arraste um vídeo vertical, com o rosto no quadro.
4. Cole um pedido como este:

```text
/efeitos orbit do segundo 3 ao 6
```

Se você instalou a skill original, em inglês, o comando é `/effects orbit from 3 to 6 seconds`. O nome do efeito, `orbit`, é o mesmo nos dois casos.

5. Espere o arquivo novo aparecer ao lado do original. O nome ganha `_effects` antes de `.mp4`.
6. Assista. Se algo cobrir o rosto ou o tempo estiver fora da fala, diga isso para o Claude e peça outro render.
7. Leve o MP4 para o editor. Som e legenda ficam para essa etapa: [`fluxo-no-editor/README.md`](fluxo-no-editor/README.md).

### Receita 2. Motion em HTML

Use esta receita quando o motion é um gráfico, um texto animado ou uma vinheta, sem precisar de um vídeo filmado.

1. Abra a [galeria](https://camilocoutinho.github.io/bases-animacao-reels/) ou o [`index.html`](index.html). A lista arquivo a arquivo continua em [`motion-html/exemplos/index.html`](motion-html/exemplos/index.html).
2. Para gerar uma variação, copie um prompt de [`motion-html/prompts/`](motion-html/prompts/) e cole no Claude.
3. Salve o HTML que o Claude devolver e abra no navegador.
4. Grave a tela e importe essa gravação no editor, como um clipe.

Pedido mínimo, se você quiser testar agora:

```text
Faça um único arquivo HTML, vertical, 1080 por 1920.
Fundo escuro e três palavras grandes no centro: GRAVA, ANIMA, EDITA.
Cada palavra entra com um impacto, uma depois da outra.
A última ganha um risco embaixo.
Use só HTML e CSS, sem imagens externas.
Deixe as cores no topo, fáceis de trocar: fundo, texto e destaque.
A animação dura cerca de 5 segundos e fica em loop.
```

O exemplo correspondente, já pronto, é [`motion-html/exemplos/01-tipo-cinetico.html`](motion-html/exemplos/01-tipo-cinetico.html).

## O que você precisa

| Caminho | O que precisa estar no computador |
|---|---|
| Efeito no vídeo falado | Claude Code, `ffmpeg` e Python. A documentação da tradução em português lembra que a skill é grátis e que o Claude Code entra no plano pago do Claude. |
| Motion em HTML | Um navegador (Chrome, Edge ou o navegador do sistema) para abrir o arquivo. O Claude, para gerar uma variação a partir de um prompt. |

No primeiro uso da skill de efeitos, o README dela descreve uma preparação de cerca de dois minutos. Ele também diz que o Claude instala `ffmpeg` e Python se os dois ainda não estiverem na máquina. Se essa instalação automática não acontecer, os dois programas precisam ser instalados antes de renderizar.

## Mapa das pastas

```
├── index.html                galeria das 10 animações
├── README.md                 você está aqui
├── LICENSE                   licença MIT do material original
├── CREDITOS.md               fontes, links e o que não foi copiado
├── efeitos-talking-head/
│   └── README.md             instalar a skill e pedir o efeito
├── motion-html/
│   ├── README.md             pedir um HTML e gravar a tela
│   ├── prompts/              10 prompts originais, prontos para colar
│   └── exemplos/             os mesmos 10, em HTML que abre no navegador
└── fluxo-no-editor/
    ├── README.md             qual guia abrir
    ├── capcut.md
    ├── premiere.md
    └── davinci.md
```

Não há pasta de template do CapCut, do Premiere, do DaVinci, do After Effects nem do Remotion. O que sai daqui é um MP4 ou uma gravação de tela.

## O que fica de fora

- O editor continua sendo o lugar da música, da legenda e do corte fino. Este repositório entrega o rascunho do motion.
- O material que o [@gut1n](https://www.instagram.com/p/DgAySIoIAQW/) e o [@zeeuiux](https://www.instagram.com/reel/Dfpf3T_gxSp/) enviam por mensagem direta não está aqui. Não há licença pública para republicar esses pacotes. O crédito e o link ficam em [`CREDITOS.md`](CREDITOS.md).

## Créditos e referências

A skill de efeitos é de **Vibha Ramprakash**, licença MIT: [Vibha-Ramprakash/claude-video-effects](https://github.com/Vibha-Ramprakash/claude-video-effects). A tradução para português é de **Paulo Cauhi**: [pcauhi/efeitos](https://github.com/pcauhi/efeitos), com o mesmo copyright e a mesma licença MIT.

Os posts de **Pedro Augusto** ([@gut1n](https://www.instagram.com/p/DgAySIoIAQW/)) e de **Zeeshan Ahmed** ([@zeeuiux](https://www.instagram.com/reel/Dfpf3T_gxSp/)) são inspiração. O conteúdo que eles mandam no direct não foi copiado.

O pack aberto de prompts em inglês e malaio está em [sasateguh/awesome-claude-motion-prompts](https://github.com/sasateguh/awesome-claude-motion-prompts), licença CC0. Os prompts desta pasta são outros, escritos para este repositório. A lista completa, com o que cada licença permite, está em [`CREDITOS.md`](CREDITOS.md).

## Licença

O texto, os prompts e os exemplos em HTML deste repositório estão na licença MIT. O arquivo legal, em inglês, é o [`LICENSE`](LICENSE). Copyright (c) 2026 Camilo Coutinho.

Em português claro: você pode usar estes arquivos nos seus Reels, alterar cores e frases, e levar para trabalho de cliente. Se for republicar os arquivos, mantenha o aviso de copyright e a licença.

Essa MIT vale para o que foi escrito aqui. Ela não transfere a autoria da skill da Vibha, nem dos prompts de outras pessoas, nem cobre o material que só circula por mensagem direta. Usar o vídeo pronto no seu Reel também não torna você autor dessa skill.

## Para os alunos do Camilo

Camilo Coutinho é estrategista de vídeo e YouTube e fundador da Double Play Media.

O site da Double Play é [https://doubleplay.com.br](https://doubleplay.com.br).
