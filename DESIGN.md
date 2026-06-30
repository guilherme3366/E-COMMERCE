---
name: E-Commerce Slides
description: Apresentação técnica e visual da solução de e-commerce integrada.
colors:
  primary: "#8b5cf6"
  secondary: "#3b82f6"
  neutral-bg: "#090d16"
  neutral-card: "#131a2c"
  neutral-card-hover: "#1b253d"
  neutral-border: "#24304f"
  neutral-text: "#f8fafc"
  neutral-text-muted: "#94a3b8"
  accent-success: "#10b981"
  accent-warning: "#f59e0b"
typography:
  display:
    fontFamily: "Plus Jakarta Sans, sans-serif"
    fontSize: "clamp(2rem, 5vw, 4rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Plus Jakarta Sans, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
rounded:
  xs: "2px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "20px"
  xxl: "24px"
  full: "30px"
spacing:
  xs: "8px"
  sm: "10px"
  md: "22px"
  lg: "40px"
  xl: "60px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral-bg}"
    rounded: "{rounded.md}"
    padding: "14px 28px"
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
---

# Design System: E-Commerce Slides

## 1. Overview

**Creative North Star: "The Neon Engine Room"**

O sistema visual é projetado como uma cabine de controle de alto desempenho, empregando um tema escuro e profundo que remete à robustez e estabilidade dos fluxos de dados de backend. Elementos interativos se comportam como instrumentos analíticos: superfícies planas por padrão que se iluminam e se elevam ao toque do cursor, utilizando tons vibrantes de violeta e azul elétrico como guias de foco e transições fluidas.

Rejeitamos designs corporativos tradicionais baseados em fundos claros genéricos ou layouts repletos de texto estático e cinza sem contraste. O foco é a legibilidade e o impacto tecnológico inovador.

**Key Characteristics:**
- Fundo escuro e imersivo com contraste tipográfico nítido.
- Gradientes violeta-azul dinâmicos que sinalizam interações de sucesso e fluxos de dados.
- Elementos modulares com bordas semi-transparentes que se iluminam sob foco.
- Micro-animações baseadas em curvas exponenciais suaves (ease-out-quint).

## 2. Colors

O esquema de cores utiliza uma paleta escura de alto contraste com tons vibrantes de neon para foco estratégico.

### Primary
- **Nebula Purple** (#8b5cf6): O tom principal usado para marcas de foco, botões de ação e títulos de slides. Transmite inovação e exclusividade tecnológica.

### Secondary
- **Electric Cyan** (#3b82f6): Usado para conectar fluxos, setas indicadoras e rotas de backend (como AppMax e Magi5), sinalizando transições operacionais.

### Neutral
- **Deep Space Slate** (#090d16): O fundo principal da apresentação, garantindo conforto visual.
- **Card Navy** (#131a2c): Cor de preenchimento dos blocos modulares e cards.
- **Border Blue** (#24304f): Tom para contorno de divisões e caixas de texto.
- **Ink White** (#f8fafc): Cor do texto de leitura primário.
- **Muted Slate** (#94a3b8): Cor para textos de apoio e descrições secundárias.

### Named Rules
**The 10% Accent Rule.** O gradiente violeta vibrante e o cian neon devem ser reservados para elementos críticos (botões, ícones e fluxos ativos), ocupando menos de 10% da área útil visual do slide.

## 3. Typography

**Display Font:** Plus Jakarta Sans (with sans-serif fallback)
**Body Font:** Plus Jakarta Sans (with sans-serif fallback)

A tipografia é moderna, geométrica e limpa, garantindo máxima leitura à distância ou em projeção de tela.

### Hierarchy
- **Display** (ExtraBold (800), clamp(2rem, 5vw, 4rem), 1.1): Usado para títulos principais dos slides.
- **Headline** (Bold (700), 24px, 1.3): Usado para títulos de subseções e cards.
- **Body** (Regular (400), 16px, 1.6): Usado para parágrafos descritivos. Limite de comprimento de linha recomendado de 70 caracteres.
- **Label** (Bold (700), 12px, 0.05em letter-spacing, uppercase): Usado em badges de progresso ou identificadores técnicos rápidos.

### Named Rules
**The Heading Balance Rule.** Todos os cabeçalhos H1, H2 e H3 devem usar `text-wrap: balance` para evitar linhas órfãs feias em visualizações responsivas.

## 4. Elevation

O sistema visual é essencialmente plano em repouso, simulando um console virtual. A profundidade física é criada como resposta imediata às interações e toques do usuário.

### Shadow Vocabulary
- **Glow Primary** (rgba(139, 92, 246, 0.25)): Um brilho violeta difuso projetado sob o botão ativo.
- **Elevated Hover** (0 8px 30px rgba(0, 0, 0, 0.3)): Usado em cards sob foco do mouse para separá-los fisicamente do fundo escuro.

### Named Rules
**The Hover Glow Rule.** Sombras e brilhos neon não devem ser usados de forma estática; eles devem atuar exclusivamente como resposta de estado ativo ou hover.

## 5. Components

### Buttons
- **Shape:** Borda arredondada suave (12px)
- **Primary:** Preenchimento com gradiente Nebula Purple a Electric Cyan. Texto em Deep Space Slate (#090d16) com peso negrito.
- **Hover:** Transforma e desloca verticalmente 2px para cima (`translateY(-2px)`) com adição de sombra de destaque Nebula.

### Cards / Containers
- **Corner Style:** Borda arredondada moderada (16px)
- **Background:** Card Navy (#131a2c) com borda fina de 1px em Border Blue (#24304f).
- **Hover:** Transição suave da borda para Nebula Purple e elevação leve.

### Interactive Checklist
- **Checkbox:** Caixa circular de 20px com contorno fino. Preenche com ícone SVG de check em verde esmeralda ao ser ativado.

## 6. Do's and Don'ts

### Do:
- **Do** manter contraste mínimo de 4.5:1 em todos os textos sobre o fundo escuro.
- **Do** usar `text-wrap: balance` nos títulos dos slides.
- **Do** garantir transições de slides baseadas em curvas de atenuação rápidas (ease-out-quint).

### Don't:
- **Don't** usar texto em cinza claro sem contraste sobre fundos cian ou violeta.
- **Don't** aplicar listras de bordas coloridas laterais como decoração (proibido o uso de side-stripes).
- **Don't** utilizar fontes genéricas de sistema sem carregamento apropriado.
- **Don't** criar grids de cards idênticos sem variação de ritmo visual ou ícones adequados.
