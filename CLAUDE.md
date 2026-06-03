# Landing Page — Astec Corte & Dobra

## Visão Geral

Criar uma landing page de alta conversão B2B para a **nova divisão de corte, dobra e acabamento metálico da Astec**, empresa com 30 anos de mercado em pontes rolantes e talhas elétricas.

Objetivo: gerar leads qualificados (engenheiros de compras, gestores industriais) via pedido de orçamento por WhatsApp ou formulário.

---

## Arquivo de Referência de Design

O design system completo está em:

```
design_system2.html
```

(já presente nesta pasta — use como template base, copie a estrutura HTML/CSS/JS e adapte para a Astec Corte & Dobra)

---

## Paleta de Cores

| Token          | Hex       | Uso                                        |
|----------------|-----------|--------------------------------------------|
| `brand-blue`   | `#355CA1` | Cor primária — azul exato da logomarca Astec |
| `brand-yellow` | `#FACC15` | Cor de destaque/CTA — amarelo industrial   |
| `brand-dark`   | `#0A0A0A` | Background principal                       |
| `brand-gray`   | `#171717` | Background de cards/seções alternadas      |
| `brand-card`   | `#222222` | Background de cards internos               |
| `white`        | `#FFFFFF` | Textos primários                           |
| `muted`        | `#9CA3AF` | Textos secundários                         |

> O azul `#355CA1` foi extraído diretamente da logomarca via análise de pixel.  
> Onde o template usa amarelo como acento principal, manter `#FACC15`. Substituir azuis genéricos por `#355CA1`.

---

## Logomarca

```
logomarca/logo_Astec.png
```

- Usar no **header fixo** e no **rodapé**
- Fundo transparente — funciona em dark background
- Altura recomendada no header: `40–48px`

---

## Tipografia

- **Fonte principal:** `Inter`, sans-serif
- **Headlines:** `Space Grotesk` peso 700 ou `Inter` 800
- Carregar via Google Fonts: `Inter` (400, 500, 600, 700) + `Space Grotesk` (700)

---

## Estrutura da Página

### 1. Header Fixo
- Logo Astec (esquerda)
- Nav: Serviços | Capacidade Técnica | Sobre | Contato
- CTA botão: **"Solicitar orçamento"** → âncora ao formulário/WhatsApp
- Dark, semi-transparente com `backdrop-blur`

---

### 2. Hero Section

**Headline:**
> Corte e dobra qualquer um faz. Só a Astec entrega a peça pronta para montagem.

**Sub-headline:**
> Fabricação completa com solda, caldeiraria e pintura (eletrostática, líquida ou galvanizada) — além de corte plasma, oxicorte (até 25mm) e dobra. Tudo em um único fornecedor, com entrega rápida.

- **CTA primário:** botão amarelo `#FACC15` → "Solicitar Orçamento"
- **CTA secundário:** botão outline → "Falar no WhatsApp"
- Background: padrão dot-grid sutil (extrair do template de referência)

---

### 3. Barra de Autoridade (trust bar)

Faixa horizontal com texto centralizado:

> A precisão da nova divisão de corte e dobra com a garantia de quem já movimenta cargas pesadas há 30 anos. Empresas que confiam na Astec para içar toneladas agora têm acesso à mesma exigência de qualidade nas peças que precisam.

---

### 4. Agitação do Problema

> Você corta, dobra e ainda precisa mandar soldar em outro lugar — e depois pintar em um terceiro. Cada etapa é um prazo, um frete e um risco de atraso. Na Astec, a peça entra como projeto e sai pronta para montagem.

Layout: texto centralizado, tipografia grande, destacar as dores ("outro lugar", "terceiro", "prazo", "frete", "risco de atraso").

---

### 5. Capacidade Técnica — O Que Fazemos

Grid 2×2 em desktop, 1 coluna em mobile. Cada card com ícone SVG inline, título em `#355CA1`, texto em muted:

| # | Título | Conteúdo |
|---|--------|----------|
| 1 | **Corte** | Oxicorte, plasma e serra de fita. Aço carbono e inox até 25mm (1 polegada). |
| 2 | **Dobra** | Prensa dobradeira CNC — ângulos precisos para peças de caldeiraria leve e média, com rastreabilidade do aço. |
| 3 | **Solda e Caldeiraria** | Fabricação e montagem completa de estruturas metálicas. Do componente isolado ao conjunto finalizado. |
| 4 | **Acabamento Premium** | Pintura eletrostática e galvanização (prata ou amarela) — sua peça sai pronta para uso, sem etapas externas. |

---

### 6. Por Que a Astec

Dois blocos lado a lado (stacked em mobile):

**Bloco A:**
> **Um fornecedor. Uma entrega. Peça pronta.**
> Da chapa crua ao acabamento final, tudo sob o mesmo teto. Sem intermediários, sem etapas externas.

**Bloco B:**
> **30 anos de indústria pesada**
> A Astec nasceu fabricando e mantendo pontes rolantes e talhas elétricas. Rigor técnico não é diferencial para nós — é obrigação.

---

### 7. Prova Visual (placeholders)

Grid de imagens com placeholders comentados para substituição:

```html
<!-- TODO: substituir por foto real do maquinário -->
<!-- Legenda: "Nossa prensa dobradeira CNC em operação" -->

<!-- TODO: substituir por foto da equipe com nome e cargo -->

<!-- TODO: substituir por embed de vídeo (30s) mostrando ciclo completo: corte → acabamento -->
```

Usar `<div>` com aspect-ratio correto, fundo `#222`, texto de instrução em muted.

---

### 8. FAQ Técnico

Accordion expandível com 3 perguntas:

**P: Vocês trabalham com inox?**
R: Sim. Trabalhamos com aço carbono e inox, com disponibilidade conforme pedido.

**P: Qual a espessura máxima que vocês cortam?**
R: Até 25mm com plasma e oxicorte — o range ideal para caldeiraria leve e média.

**P: Qual o prazo para receber o orçamento?**
R: Em até 24 horas após o envio do projeto. Para projetos simples, retornamos no mesmo dia.

---

### 9. CTA Final / Formulário

- Título: **"Solicite seu orçamento agora"**
- Formulário: Nome | Empresa | WhatsApp | Descrição da peça | Botão "Enviar"
- Alternativa/adicional: botão grande WhatsApp
- Background: gradiente ou sólido `#355CA1`

```html
<!-- TODO: substituir número do WhatsApp em todos os links wa.me/55XXXXXXXXXXX -->
<!-- TODO: conectar endpoint do formulário (action="#" enquanto não definido) -->
```

---

### 10. Rodapé Institucional

> **Astec — divisão de corte, dobra e acabamento metálico**
> Endereço completo | Telefone | WhatsApp | CNPJ
> Parte do grupo Astec, referência em pontes rolantes e talhas elétricas há 30 anos na indústria brasileira.

- Logo Astec menor
- Links de navegação
- Ícones sociais (placeholders)

```html
<!-- TODO: preencher endereço, telefone, CNPJ e links de redes sociais -->
```

---

## Regras de Copy

> ⚠️ **NÃO ALTERAR A COPY.** Reproduzir os textos exatamente como escritos neste documento. Aplicar apenas formatação visual (peso, tamanho, cor) para hierarquia — sem reescrever, resumir ou parafrasear nenhum trecho.

---

## Regras de Implementação

1. **Um único arquivo `index.html`** — CSS e JS inline, sem dependências externas além de Google Fonts e ícones SVG inline.
2. **Responsivo:** mobile-first. Breakpoints: 375px / 768px / 1280px.
3. **Acessibilidade:** `alt` em todas as imagens, `aria-label` em botões de ícone, contraste WCAG AA.
4. **Animações:** suaves, mesmas do template de referência (fadeIn, slide-up). Sem excessos.
5. **Performance:** lazy load em imagens, JS mínimo.
6. Formulário estático (`action="#"`) — deixar comentário TODO para conexão de backend.

---

## Contexto Estratégico (não vai para a página)

- **Público-alvo:** engenheiros de compras, gestores industriais, compradores técnicos B2B
- **Principal diferencial:** fornecedor único (corte + dobra + solda + acabamento) — concorrentes fazem só parte do processo
- **Prazo de entrega:** 3 dias úteis (concorrente CBC entrega em 5)
- **Área de atendimento:** região metropolitana, raio ~100 km; demais por frete
- **Materiais:** 90% chapa carbono; também inox; galvanização prata ou amarela
- **Capacidade:** oxicorte/plasma até 25mm, prensa dobradeira CNC
- **Sem certificações ISO** — não mencionar nem sugerir
- **Produto novo:** sem cases de clientes ainda; autoridade vem dos 30 anos da marca Astec em pontes rolantes
