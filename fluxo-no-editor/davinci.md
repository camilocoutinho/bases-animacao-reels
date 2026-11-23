# DaVinci Resolve

Use este guia para importar o MP4 com `_effects` no nome, ou a gravação de tela de um HTML, e terminar o Reel no DaVinci Resolve.

## 1. Acertar o projeto para vertical

O Resolve abre muitos projetos em 1920 por 1080. Um Reel precisa do contrário.

1. Crie um projeto novo.
2. Abra a engrenagem no canto inferior direito.
3. Em **Master Settings**, na resolução da timeline, use largura **1080** e altura **1920**.
4. Deixe a taxa de quadros igual à do clipe que você vai importar.

Faça isso antes de criar a timeline. Mudar depois mexe no enquadramento que você já ajustou.

## 2. Importar e montar

1. Na página **Media**, importe o MP4. Na versão que junta as páginas no menu Corte, a importação fica nessa área.
2. Vá para a página **Edit** (ou Corte).
3. Arraste o clipe para uma timeline nova.
4. Se a gravação de tela trouxer barra preta, use o corte no inspetor até o quadro vertical encostar nas bordas. Não estique o clipe por um eixo só.

## 3. Som

O MP4 da skill traz a voz e não traz música.

1. Importe a música para o media pool.
2. Coloque numa faixa de áudio abaixo da voz.
3. Baixe o volume da música.

Dá para fazer esse ajuste na página Edit. A página **Fairlight** entra quando a mixagem pedir mais do que um volume só.

A gravação do HTML pode estar sem áudio. A narração entra como clipe separado.

## 4. Legenda

1. Na página Edit, crie a legenda pela ferramenta de títulos ou de legendas da sua versão.
2. Leia no quadro. A legenda automática erra nome e número.
3. Posicione no miolo, fora da faixa de cima e da de baixo.

## 5. Entregar

1. Abra a página **Deliver**.
2. Escolha um preset de MP4 e, se precisar, ajuste para **H.264** ou **H.265**.
3. Confira a resolução: **1080 × 1920**. O número trocado (1920 × 1080) devolve um vídeo deitado.
4. Adicione à fila de render, exporte e assista o arquivo fora do Resolve.
