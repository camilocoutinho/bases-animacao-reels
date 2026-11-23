# Créditos e referências

Este arquivo diz de onde cada coisa veio, o que pode ser copiado e o que este repositório de propósito deixou de fora.

A consulta às fontes abaixo foi feita em 23/11/2026. Repositórios de outras pessoas continuam mudando. Na dúvida, vale o README e a licença no link original.

## Material original deste repositório

Entram aqui os textos de orientação, os dez prompts em `motion-html/prompts/` e os HTML em `motion-html/exemplos/`.

- Copyright (c) 2026 Camilo Coutinho
- Licença MIT, no arquivo [`LICENSE`](LICENSE)

Você pode usar o resultado nos seus Reels. Isso não transfere para você a autoria da skill de efeitos nem de prompts de terceiros.

## Skill de efeitos para vídeo falado

O comando `/effects` (e a tradução `/efeitos`) não foi escrito neste repositório. O código, as fontes e os modelos continuam nos repositórios de origem. Não há uma cópia da skill nesta pasta, para o aluno instalar a versão atual em vez de uma cópia velha.

### Original, em inglês

- Autora: Vibha Ramprakash
- Repositório: [Vibha-Ramprakash/claude-video-effects](https://github.com/Vibha-Ramprakash/claude-video-effects)
- Licença: [MIT](https://github.com/Vibha-Ramprakash/claude-video-effects/blob/main/LICENSE)
- Copyright (c) 2026 Vibha Ramprakash

Em 23/11/2026, o README dessa skill lista 51 efeitos. Ele descreve o resultado como versão inicial, sem som e sem legenda, e indica o CapCut para essa etapa. Também informa render em 1080p.

A própria licença avisa que as fontes em `fonts/` e os modelos em `models/` mantêm as licenças próprias (ver o README, `fonts/*.txt` e `models/NOTICE.md` naquele repositório). Os créditos publicados lá incluem:

- rastreamento de rosto: OpenCV YuNet (MIT)
- recorte da pessoa: MediaPipe Selfie Segmenter (Apache 2.0)
- fontes: Archivo Black, Instrument Serif, Space Mono, Inter, Anton, Montserrat (SIL OFL) e Permanent Marker (Apache 2.0)

O catálogo de nomes em [`efeitos-talking-head/README.md`](efeitos-talking-head/README.md) resume esse README para quem edita. As frases da tabela foram reescritas aqui. O código da skill não está incluído. Se algum dia for preciso espelhar o código, a MIT exige manter o aviso de copyright e o texto da licença, e também as licenças das fontes e dos modelos.

O produto pago da mesma autora não faz parte deste repositório.

Comando de instalação publicado no README dela:

```bash
git clone https://github.com/Vibha-Ramprakash/claude-video-effects ~/.claude/skills/effects
```

### Tradução para português

- Tradução: Paulo Cauhi
- Repositório: [pcauhi/efeitos](https://github.com/pcauhi/efeitos)
- Licença: [MIT](https://github.com/pcauhi/efeitos/blob/main/LICENSE), ainda com Copyright (c) 2026 Vibha Ramprakash
- Documentação dele: [cauhi.com/pt-br/learn/efeitos-video-claude](https://cauhi.com/pt-br/learn/efeitos-video-claude)

Em 23/11/2026, o README dessa tradução lista 45 efeitos e o comando `/efeitos`. A documentação lembra que a skill é grátis e que o Claude Code entra no plano pago do Claude.

Comando de instalação publicado no README dele:

```bash
git clone https://github.com/pcauhi/efeitos ~/.claude/skills/efeitos
```

## Pack aberto de prompts de motion

- Repositório: [sasateguh/awesome-claude-motion-prompts](https://github.com/sasateguh/awesome-claude-motion-prompts)
- Licença: [CC0 1.0](https://github.com/sasateguh/awesome-claude-motion-prompts/blob/main/LICENSE)

São prompts daquele repositório, em inglês e malaio, para legendas, intros, gráficos, transições e demos de app, pensados para HTML e CSS. O README deles diz que as prévias foram renderizadas com HyperFrames. Não são os prompts enviados no direct do @zeeuiux.

Nenhum prompt desse pack foi colado aqui. Os dez prompts de `motion-html/prompts/` foram escritos para este repositório.

A CC0 dispensa a obrigação de crédito. Mesmo assim, se você copiar um prompt de lá, cite o repositório de origem.

## Só o link: nada disto foi copiado

O material abaixo circula por mensagem direta e não tem uma licença pública que permita redistribuir o guia, os slides, os prompts ou a arte. Este repositório só registra o crédito e o link.

### Pedro Augusto (@gut1n)

- Post: [instagram.com/p/DgAySIoIAQW](https://www.instagram.com/p/DgAySIoIAQW/) (21/11/2026)
- O que o post público é: um carrossel sobre efeitos grátis no Claude Code, aplicados em cima de um vídeo falado. A pessoa arrasta o vídeo e digita o comando do efeito.
- A linha de instalação e os exemplos prontos para copiar saem no direct, para quem comenta no post. Isso não está neste repositório.
- A página de links dele é [gutin.app](https://www.gutin.app/). É a página de links, não o código dos efeitos.
- Os nomes que o carrossel mostra também existem na skill MIT da Vibha. O post funciona como curadoria. A lista de comandos usada neste repositório saiu do README dessa skill, não dos slides.

### Zeeshan Ahmed (@zeeuiux)

- Reel: [instagram.com/reel/Dfpf3T_gxSp](https://www.instagram.com/reel/Dfpf3T_gxSp/) (12/11/2026)
- O que o reel público é: animações feitas a partir de um prompt, com resultado em HTML. O autor pede um comentário e envia os prompts no direct.
- Não entram aqui os prompts, o kit, os prints do reel nem a arte da marca dele.

## O que também não entra

- Imagens do Instagram.
- Qualquer pacote cuja licença não tenha sido aberta e conferida.
- Templates `.mogrt`, `.aep` ou `.drfx`. Não há uma base licenciada desses formatos nas fontes acima.

## Outro repositório do Camilo

[Checklist de segurança para quem programa com IA](https://github.com/camilocoutinho/checklist-seguranca-vibecoding). Primeiro produto público no GitHub, para quem publica com IA. A nota curta para o aluno de edição está em [`SEGURANCA.md`](SEGURANCA.md).
