# NerveGear | Link Start 🧠

Landing page conceitual inspirada no universo de **Sword Art Online**, apresentando o **NerveGear** — um headset fictício de interface neural direta (BCI) que promete imersão total em realidade virtual via tecnologia FullDive.

---

## Visão Geral

Este projeto é uma página de produto imersiva e cinematográfica, construída inteiramente com HTML, CSS e JavaScript vanilla. A experiência simula um site real de lançamento de hardware futurista, com animações orientadas por scroll, efeitos visuais de HUD e uma narrativa de produto coesa.

---

## Funcionalidades

- **Hero com Scroll Animation** — O headset rotaciona e dá zoom conforme o usuário desce a página, em três fases distintas (rotação Y → zoom → transição para vídeo)
- **Canvas de Fundo Animado** — Partículas e efeitos neon renderizados em `<canvas>` fixo no background
- **Efeito Scanline & Digital Noise** — Overlays fixos que reforçam a estética cyberpunk/sci-fi
- **Carrossel de Jogos** — Apresenta títulos como *Elden Ring*, *The Witcher 3* e *CS2* em versões fictícias FullDive, com autoplay, navegação por botões, dots de paginação e suporte a swipe em toque
- **Seção de Especificações Técnicas** — Tabela com specs fictícias do hardware (processamento sináptico, resolução retinal, latência, etc.)
- **Protocolo de Inicialização** — Cards numerados em grid com animação de barra de progresso no hover
- **FAQ Accordion** — Perguntas frequentes com lógica de accordion (abre/fecha com animação de `maxHeight`)
- **Vídeo de Introdução** — Layer de vídeo (`assets/promotion.mp4`) que entra em fade ao final do scroll hero
- **Responsividade** — Layout adaptado para mobile e desktop com Tailwind CSS

---

## Estrutura de Arquivos

```
/
├── index.html          # Arquivo principal — toda a estrutura, estilos e scripts
└── assets/
    ├── ezgif-frame-001.jpg  # Frame inicial do headset
    ├── elden-ring.png        # Imagem do jogo Elden Ring
    ├── witcher3.png          # Imagem do jogo The Witcher 3
    ├── cs2.png               # Imagem do jogo CS2
    └── promotion.mp4         # Vídeo de promoção "Link Start"
```

> ⚠️ A pasta `assets/` **não está incluída** neste repositório. Os arquivos de mídia devem ser fornecidos separadamente para que a página funcione corretamente.

---

## Tecnologias Utilizadas

| Tecnologia | Uso |
|---|---|
| HTML5 | Estrutura semântica da página |
| CSS3 | Animações, variáveis customizadas, glassmorphism |
| JavaScript (Vanilla) | Scroll logic, canvas, carrossel, accordion |
| [Tailwind CSS (CDN)](https://tailwindcss.com) | Utilitários de estilo e layout responsivo |
| [Google Fonts](https://fonts.google.com) | Fontes *Inter* e *Space Grotesk* |
| Canvas API | Efeitos de partículas e neon no fundo |

---

## Como Usar

Por ser um arquivo HTML estático, basta servir localmente:

```bash
# Com Python
python -m http.server 8000

# Com Node.js (npx)
npx serve .

# Ou abrir diretamente no navegador
open index.html
```

Acesse `http://localhost:8000` e role a página para experimentar a animação completa.

---

## Lógica de Scroll (Hero Section)

O scroll controla três fases de animação do headset:

| Fase | Progresso | Efeito |
|---|---|---|
| 1 | 0% → 50% | Rotação Y de -90° até 0° (entrada do headset) |
| 2 | 50% → 92% | Zoom progressivo de 1× até 5× |
| 3 | 92% → 100% | Fade out do headset + fade in do vídeo |

Ao término do vídeo, o overlay some automaticamente e o restante da página fica acessível.

---

## Seções da Página

1. **Hero** — Animação de scroll com o headset e display de porcentagem de calibração
2. **Line-Up de Lançamento** — Carrossel com jogos compatíveis FullDive
3. **Especificações Técnicas** — Tabela de hardware e nota de segurança
4. **Protocolo de Inicialização** — Guia de 4 passos para uso do dispositivo
5. **FAQ** — Dúvidas frequentes em formato accordion

---

## Aviso

> Este é um projeto **fictício e conceitual**, criado com fins criativos e de portfólio. O NerveGear é uma tecnologia do universo da obra de ficção *Sword Art Online* e não representa nenhum produto real. Nenhuma tecnologia de interface neural direta descrita aqui existe comercialmente.

---

## Licença

Distribuído para fins educacionais e de portfólio. O conteúdo temático é baseado em propriedade intelectual fictícia de *Sword Art Online* (Reki Kawahara / A-1 Pictures).

Obrigado pela Atenção!
