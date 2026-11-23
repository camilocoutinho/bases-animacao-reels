# Efeitos no vídeo falado

Esta pasta é o caminho para aplicar um efeito em cima de um vídeo em que você aparece falando. O nome em inglês para esse tipo de vídeo é talking head. O resultado é outro MP4. A voz não é trocada. Música, efeito sonoro e legenda ficam para o editor, no guia [`../fluxo-no-editor/README.md`](../fluxo-no-editor/README.md).

A skill que faz isso é de Vibha Ramprakash, licença MIT, Copyright (c) 2026 Vibha Ramprakash. O código não está copiado aqui. Você instala a versão atual no repositório dela, ou a tradução de Paulo Cauhi. Os dois links e o que a licença cobre estão em [`../CREDITOS.md`](../CREDITOS.md).

O catálogo no fim desta página resume o README público dessa skill. As frases foram reescritas para quem edita. O texto integral da licença está em [github.com/Vibha-Ramprakash/claude-video-effects/blob/main/LICENSE](https://github.com/Vibha-Ramprakash/claude-video-effects/blob/main/LICENSE).

## Instalar

Escolha uma das duas. As duas podem ficar instaladas: o comando muda.

### Tradução em português

É o caminho mais direto se você quer ler as instruções em português. O nome que você digita depois do comando continua em inglês, como `orbit` ou `spotlight`.

No terminal:

```bash
git clone https://github.com/pcauhi/efeitos ~/.claude/skills/efeitos
```

No Windows, a pasta é `%USERPROFILE%\.claude\skills\efeitos`.

Se o terminal não for o seu jeito, abra o Claude Code e cole:

```text
Instala a skill de efeitos a partir de https://github.com/pcauhi/efeitos na pasta ~/.claude/skills/efeitos e me avisa quando terminar.
```

Feche o Claude Code e abra de novo. O comando passa a ser `/efeitos`.

Em 23/11/2026, o README dessa tradução lista 45 efeitos.

### Skill original, em inglês

```bash
git clone https://github.com/Vibha-Ramprakash/claude-video-effects ~/.claude/skills/effects
```

No Windows (PowerShell), a pasta publicada no README é `$HOME\.claude\skills\effects`.

Ou cole no Claude Code:

```text
Instala a skill de efeitos a partir de https://github.com/Vibha-Ramprakash/claude-video-effects na pasta ~/.claude/skills/effects e me avisa quando terminar.
```

Feche o Claude Code e abra de novo. O comando passa a ser `/effects`.

Em 23/11/2026, o README original lista 51 efeitos. Os seis que a tradução ainda não listava nesse dia estão marcados na tabela.

A documentação do Paulo Cauhi lembra que a skill é grátis e que o Claude Code entra no plano pago do Claude: [cauhi.com/pt-br/learn/efeitos-video-claude](https://cauhi.com/pt-br/learn/efeitos-video-claude).

## Pedir o efeito

1. Separe um vídeo vertical, filmado no celular, com o rosto dentro do quadro.
2. Arraste o MP4 para o chat do Claude Code.
3. Digite o efeito e o tempo, do jeito que você falaria com quem está editando ao seu lado.

Tradução em português:

```text
/efeitos orbit do segundo 3 ao 6
```

Skill em inglês:

```text
/effects orbit from 3 to 6 seconds
```

Outros jeitos de marcar o tempo, que os dois READMEs ensinam:

```text
/efeitos spotlight quando eu falar "apaga a luz", com a palavra AULA atrás de mim
/efeitos comment-box no final, digitando a frase que eu te passar
/efeitos glass-widgets nos primeiros 3 segundos
```

Dá para juntar mais de um efeito no mesmo pedido:

```text
Coloca locked-on do segundo 6 ao 10, depois orbit do 10 ao 13, e um reject-stamp quando eu falar "não".
```

Na primeira vez, o README da skill descreve uma preparação de cerca de dois minutos. Ele diz que o Claude precisa de `ffmpeg` e de Python, e que instala os dois se estiverem faltando.

O Claude confere alguns frames, tira da frente o que cobriria o rosto e grava um arquivo novo ao lado do original. O nome leva `_effects` antes de `.mp4`. O áudio permanece o do arquivo que você arrastou.

O README também publica estas variações, escritas depois do nome: `glitter-spotlight`, `cover-star` com `look=editorial`, e `liquid-glass-graph` com `look=bento`.

## Conferir antes de levar ao editor

A própria skill avisa que isto é um rascunho. Você aprova. Assista antes de postar.

- O rosto continua livre? O que cobriria o rosto deve ir para trás da cabeça.
- O efeito entra na frase certa?
- O áudio é o mesmo do original?
- Som de efeito e legenda ainda não existem nesse MP4. Eles entram no CapCut, no Premiere ou no DaVinci.

Se algo sair errado, descreva o que você está vendo. Por exemplo: "a palavra cobre meu rosto" ou "entrou cedo demais". O README da skill diz que o Claude ajusta o plano e renderiza de novo.

Mais alguns avisos publicados no README da skill, em linguagem de edição:

- Vídeo vertical, com você no quadro, é o caso para o qual a skill foi feita.
- Pode falar o tempo em frase ("quando eu falar olha"). O Claude procura o segundo.
- Em `orbit`, `noise`, `phone-fan` e `profile-wall`, dá para entregar uma pasta de prints se aqueles cards forem os seus reels.
- Gráfico, contador e manchete devem usar número real. Diga ao Claude qual é o número. Não deixe um exemplo no ar.
- O render descrito no README sai em 1080p. 4K é um pedido à parte, e mais lento.

## Catálogo para digitar

A coluna do meio é o nome que entra depois de `/efeitos` ou de `/effects`. A descrição é um resumo, escrito neste repositório, do que o README da skill publica. Se o texto de lá mudar, vale o repositório da Vibha.

| # | Digite | O que o README descreve |
|---|---|---|
| 1 | `noise` | Vários reels empilhados atrás da cabeça |
| 2 | `lineup` | Cartões numerados em arco acima da cabeça |
| 3 | `locked-on` | Uma mira trava no rosto e o enquadramento acompanha |
| 4 | `orbit` | Reels giram em volta da cabeça, passando por trás |
| 5 | `lean-in` | Um zoom curto em cima de uma palavra |
| 6 | `backdrop-word` | Uma palavra enorme entra atrás da pessoa |
| 7 | `spotlight` | O fundo apaga e a pessoa continua iluminada |
| 8 | `the-bill` | O pedido aparece impresso como uma conta |
| 9 | `moody` | Uma cor de clima, no jeito de uma imagem de cinema |
| 10 | `swipe` | Uma divisória de antes e depois atravessa o quadro |
| 11 | `todo` | Um checklist ao lado vai sendo marcado durante a fala |
| 12 | `comment-box` | Um comentário é digitado e publicado na tela |
| 13 | `tap` | O botão Seguir passa para Seguindo |
| 14 | `pause-point` | A imagem congela e uma seta desenhada aponta |
| 15 | `uninstall` | Uma barra de desinstalar atravessa o quadro, com falha de imagem |
| 16 | `reel-frame` | O vídeo encolhe para dentro de um card de reel |
| 17 | `shortcut-rain` | Teclas caem atrás da pessoa |
| 18 | `reject-stamp` | Um carimbo vermelho bate na tela |
| 19 | `countdown-flip` | Um 3, 2, 1 vira acima da cabeça |
| 20 | `rabbit-hole` | O fundo se afasta como um túnel |
| 21 | `cover-star` | A pessoa entra numa capa de revista |
| 22 | `scribble` | Rabiscos de caneta aparecem em volta |
| 23 | `glass-widgets` | Janelas de vidro fosco flutuam em volta da cabeça |
| 24 | `red-collage` | Pessoa em preto e branco, palavra vermelha atrás e linhas que entram |
| 25 | `split-headline` | Uma manchete empurra a pessoa para a parte de baixo |
| 26 | `pastel-word` | Fundo lilás, palavra gigante atrás e um card de perfil |
| 27 | `check-pills` | Fundo quadriculado, reels atrás e botões que recebem clique |
| 28 | `timeline` | Visual de filme, com uma timeline e o indicador de play aceso |
| 29 | `headline-box` | Um zoom com uma manchete de duas linhas |
| 30 | `profile-wall` | A grade de reels cobre o fundo e um contador sobe |
| 31 | `tier-list` | Uma lista de ranking entra e um item vai para o topo |
| 32 | `broll-split` | Imagem de apoio em cima, com uma etiqueta, e a pessoa embaixo |
| 33 | `phone-fan` | Os reels abrem como um leque de celulares |
| 34 | `dot-reveal` | A imagem se forma em pontos e depois entra em foco |
| 35 | `headline-wall` | Manchetes se empilham atrás e um total aparece na frente |
| 36 | `checklist` | Uma lista de tarefas abaixo do queixo, cada item fica marcado |
| 37 | `liquid-glass-graph` | Um card de vidro com gráfico que sobe e número que conta |
| 38 | `carousel-spin` | Os reels giram num carrossel em volta da pessoa |
| 39 | `match-cut` | Páginas cortam numa palavra, presas atrás da cabeça |
| 40 | `apple-toggles` | Interruptores ligam um a um, abaixo do queixo |
| 41 | `led-sign` | A luz cai e um letreiro se escreve atrás |
| 42 | `slow-push` | Uma aproximação lenta, com o fundo saindo de foco |
| 43 | `over-the-shoulder-zoom` | O quadro vai a um canto, aparece um gráfico, depois ao outro canto |
| 44 | `messages` | Avisos no estilo de mensagem entram um depois do outro |
| 45 | `place-in-grid` | A pessoa encolhe para o centro de uma grade 3×3 |
| 46 | `tape-label` | Uma fita amarela com uma frase pousa no peito |
| 47 | `select-resize` | Uma seleção pega um número e um cursor aumenta esse número |
| 48 | `wave-trim` | Os silêncios aparecem cortados até sobrarem as falas |
| 49 | `huge-strike` | Uma palavra enorme atrás, com um risco vermelho por cima |
| 50 | `crayon-write` | Um giz escreve uma palavra atrás da cabeça e sublinha |
| 51 | `fan-build` | Capas de reel entram uma a uma num leque atrás da cabeça |

Os itens 46 a 51 constam do README em inglês consultado em 23/11/2026. No mesmo dia, o README da tradução em português lista 45 efeitos e termina em `place-in-grid`. Se a tradução não reconhecer um desses seis nomes, use a skill em inglês ou olhe de novo o README dela. Os dois repositórios podem ganhar efeito novo depois desta página.

## O próximo passo

Abra [`../fluxo-no-editor/capcut.md`](../fluxo-no-editor/capcut.md) se a legenda e a música forem no CapCut. Para Premiere ou DaVinci, use o guia com o nome do programa na mesma pasta.
