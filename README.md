# App de Meditação Guiada 🧘‍♀️

Este é um aplicativo web simples e bonito para reproduzir meditações guiadas do YouTube. Desenvolvido apenas com HTML, CSS e um pouco de JavaScript, sem dependências externas além do Font Awesome e do embed do YouTube.

## Funcionalidades Principais

- **Design clean e relaxante**: Paleta de cores suaves em tons de roxo e lavanda, com gradientes, sombras sutis e elementos circulares que transmitem calma.
- **Player embutido**: Ao selecionar um vídeo da lista, ele é carregado automaticamente em um `<iframe>` do YouTube com autoplay ativado.
- **Lista de sessões**: 6 meditações guiadas populares (em português), com título, visualizações fictícias e destaque visual ao selecionar.
- **Informações detalhadas**: Ao escolher um vídeo, aparece o título, número de visualizações e uma descrição mais completa abaixo do player.
- **Responsivo**: Adapta-se bem a telas menores (mobile) e mantém um layout agradável em desktop.
- **Seleção automática**: Ao carregar a página, o primeiro vídeo ("Meditação para Iniciantes") é selecionado automaticamente.

## Lista de Vídeos Incluídos

1. **Meditação para Iniciantes** – ID: T59guY2g208
2. **Meditação para Relaxamento Profundo** – ID: B6mQUzmlZAo
3. **Meditação para Dormir** – ID: TPH5ynw5ukM
4. **Meditação para Redução da Ansiedade** – ID: ZNr-Jl4MZcw
5. **Meditação para Foco e Concentração** – ID: 28szq1vC7OY
6. **Meditação da Manhã Energética** – ID: jl7zmFPjUZk

## Como Funciona o JavaScript

- Um objeto `videoData` armazena título, descrição completa e visualizações de cada vídeo.
- A função `selectVideo(videoId, title, description)`:
  - Substitui o conteúdo do player por um `<iframe>` do YouTube.
  - Atualiza as informações do vídeo selecionado.
  - Destaca visualmente o item da lista clicado (mudança de cor de fundo e borda).
- Ao carregar a página (`window.onload`), o primeiro vídeo é selecionado automaticamente após um pequeno delay.

## Capturas de Tela (descrição visual)

- **Header**: Título grande com ícone de spa e emoji de meditação, fundo roxo com círculos decorativos translúcidos.
- **Player**: Área escura com bordas arredondadas; quando nenhum vídeo está selecionado, exibe um placeholder com ícone do YouTube.
- **Lista**: Cartões com número circular, título, visualizações e ícone do YouTube à direita. Hover levanta o cartão e aumenta o ícone.
- **Footer**: Mensagem simples com destaque no número de sessões disponíveis.

## Como Usar / Expandir

- Para adicionar mais vídeos, basta:
  - Inserir um novo `<div class="video-item">` na lista com o `onclick` correto.
  - Adicionar a entrada correspondente no objeto `videoData`.
- Pode ser hospedado em qualquer servidor estático (GitHub Pages, Netlify, Vercel etc.).
- Não requer backend nem API keys.

## Tecnologias Utilizadas

- HTML5
- CSS3 (Flexbox, Grid, media queries)
- JavaScript vanilla
- Font Awesome 6.4 (ícones)
- YouTube Embed API (iframe)

Um projeto leve, acessível e perfeito para quem quer uma interface tranquila para praticar meditação guiada diariamente. Namastê! 🧘‍♂️
