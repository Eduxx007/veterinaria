# Design System — Clínica Veterinária e Pet Shop Bicho Feliz

> **Nota:** Todos os dados comerciais, profissionais e institucionais apresentados neste documento são fictícios e foram estruturados exclusivamente para fins de desenvolvimento, demonstração e estudo.

Este documento define o sistema de design oficial para o desenvolvimento do site institucional e comercial da **Clínica Veterinária e Pet Shop Bicho Feliz**, situada no Centro de Campina Grande-PB.

Todas as diretrizes visuais foram calibradas com base nas diretrizes do `briefing.md`, `mapa_site.md`, `conteudo.md` e nas melhores práticas de experiência de usabilidade voltada à conversão no WhatsApp e clareza informativa.

---

## 1. Princípios de Design

1. **Profissionalismo e Saúde:** Transmitir a seriedade e o cuidado médico veterinário nas áreas clínicas e cirúrgicas.
2. **Acolhimento e Vitalidade:** Incorporar o lado caloroso e alegre dos animais de estimação, presente nas áreas de estética (banho e tosa) e pet shop.
3. **Clareza e Honestidade:** Tipografia de fácil leitura, com horários e aviso explícito de ausência de emergência 24h sempre visíveis, evitando qualquer ambiguidade.
4. **Mobile-First e Conversão Ágil:** Navegação pensada prioritariamente para telas de smartphones, com acesso ao WhatsApp em um único toque em qualquer página.
5. **Acessibilidade (WCAG 2.1 AA):** Relação de contraste mínima de 4.5:1 para textos comuns e 3:1 para textos grandes e componentes interativos.

---

## 2. Paleta de Cores e Tokens de Cor

A paleta oficial harmoniza o **Verde Floresta** da tipografia da marca e da área médica com o **Vermelho Coral** de destaque, complementados pelo **Amarelo Dourado** lúdico e neutros limpos.

### 2.1. Tabela de Cores

| Token / Variável | HEX | Amostra | Finalidade / Aplicação | Contraste |
|---|---|---|---|---|
| `--color-primary` | `#1B4D2E` | 🟢 Verde Floresta | Cor principal da marca; títulos principais, cabeçalho de destaque, botões primários clínicos. | > 7:1 em fundo branco (AAA) |
| `--color-primary-dark` | `#123520` | 🟢 Verde Escuro Profundo | Hover de botões primários, textos sobre fundos verdes claros, rodapé institucional. | > 10:1 em branco |
| `--color-primary-light` | `#2D7A49` | 🟢 Verde Médio | Ícones, bordas ativas, tags e detalhes secundários. | > 4.5:1 em branco |
| `--color-primary-soft` | `#EAF4EE` | ⚪ Verde Menta Claro | Fundo de badges, fundos de cards clínicos, áreas de destaque suave. | Base p/ texto escuro |
| `--color-secondary` | `#D93829` | 🔴 Vermelho Coral | Cor de destaque da marca; badges de atenção, promoções e detalhes visuais. | > 4.5:1 em branco |
| `--color-secondary-hover` | `#B8281A` | 🔴 Vermelho Escuro | Hover de elementos com destaque secundário. | > 5:1 em branco |
| `--color-secondary-soft` | `#FDF2F0` | ⚪ Rosa/Coral Claro | Fundos sutis para avisos leves e tags de pet shop. | Base p/ texto escuro |
| `--color-accent-yellow` | `#F6C90E` | 🟡 Amarelo Dourado | Cor acolhedora; detalhes de banho e tosa, estrelas e selos visuais. | Usar c/ texto escuro |
| `--color-accent-yellow-soft`| `#FEF9E7` | ⚪ Amarelo Muito Claro | Fundo do banner de aviso de funcionamento (`EmergencyNotice`). | Base p/ texto escuro |
| `--color-whatsapp` | `#25D366` | 🟢 Verde WhatsApp | Botão flutuante oficial e CTAs de conversão direta para o aplicativo. | Oficial Meta |
| `--color-whatsapp-hover` | `#1EBE5D` | 🟢 Verde WhatsApp Escuro | Hover do botão de WhatsApp. | Oficial Meta |
| `--color-instagram` | `#E1306C` | 🟣 Rosa Instagram | Ícone e links oficiais do Instagram. | Oficial Meta |
| `--color-bg` | `#FFFFFF` | ⚪ Branco Puro | Fundo padrão das páginas e do corpo de cards. | - |
| `--color-bg-alt` | `#F8FAFC` | ⚪ Gelo / Cinza Neutro | Fundo de seções alternadas para criar respiro visual e profundidade. | - |
| `--color-surface` | `#FFFFFF` | ⚪ Superfície | Fundo de cards, modais e menus de navegação. | - |
| `--color-border` | `#E2E8F0` | ⚪ Cinza Claro | Bordas de cards, divisores e inputs de formulário. | 3:1 |
| `--color-border-hover` | `#CBD5E1` | ⚪ Cinza Médio | Hover de bordas e divisores. | - |
| `--color-text-main` | `#1E293B` | ⚫ Grafite Escuro | Texto principal de leitura, parágrafos e legendas escuras. | > 10:1 em branco |
| `--color-text-muted` | `#64748B` | 🔘 Cinza Ardósia | Subtítulos, metadados, dicas auxiliares e horários secundários. | > 4.5:1 em branco |
| `--color-text-inverse` | `#FFFFFF` | ⚪ Branco | Textos aplicados sobre botões escuros ou rodapé escuro. | > 7:1 em primário |
| `--color-alert-border` | `#F59E0B` | 🟠 Âmbar | Borda de destaque para o aviso de fechamento dominical e ausência de emergência 24h. | - |
| `--color-alert-text` | `#78350F` | 🟤 Marrom Âmbar Escuro | Texto legível para o banner de aviso de funcionamento. | > 7:1 em fundo suave |

---

## 3. Tipografia

A hierarquia tipográfica utiliza fontes modernas do catálogo oficial do Google Fonts, garantindo carregamento rápido, excelente legibilidade e compatibilidade em qualquer plataforma:

- **Fonte de Títulos e Destaque:** `'Montserrat'`, sans-serif  
  *Justificativa:* Robusta, geométrica e acolhedora, com pesos encorpados que dialogam diretamente com a identidade visual da marca ("Bicho Feliz").
- **Fonte de Corpo de Texto e Interface:** `'Inter'`, sans-serif  
  *Justificativa:* Fonte de sistema altamente legível, desenhada especificamente para telas digitais e interfaces de usuário.

### 3.1. Escala Modular de Tipografia

| Nível | Tamanho (Mobile) | Tamanho (Desktop) | Peso (Weight) | Altura de Linha (Line-height) | Aplicação |
|---|---|---|---|---|---|
| **H1** | `2rem` (32px) | `2.75rem` (44px) | 800 (Extra Bold) | 1.2 | Título principal de cada página (Hero Section). |
| **H2** | `1.5rem` (24px) | `2rem` (32px) | 700 (Bold) | 1.25 | Títulos de seções (`SectionTitle`). |
| **H3** | `1.25rem` (20px) | `1.375rem` (22px) | 600 (Semi Bold) | 1.3 | Títulos de cards, serviços e categorias. |
| **H4** | `1.125rem` (18px) | `1.125rem` (18px) | 600 (Semi Bold) | 1.4 | Títulos de itens de FAQ e blocos internos. |
| **Body (Padrão)** | `1rem` (16px) | `1rem` (16px) | 400 (Regular) | 1.6 | Textos de leitura contínua, descrições e parágrafos. |
| **Body Lead** | `1.125rem` (18px) | `1.25rem` (20px) | 500 (Medium) | 1.5 | Subtítulos de introdução em seções hero. |
| **Small** | `0.875rem` (14px) | `0.875rem` (14px) | 500 (Medium) | 1.5 | Metadados, endereços no rodapé e legendas. |
| **Badge / Tag** | `0.75rem` (12px) | `0.75rem` (12px) | 700 (Bold) | 1.0 | Etiquetas de status, categorias e chips de destaque. |

---

## 4. Espaçamento, Grid e Dimensões

Sistema construído sobre múltiplos de **4px / 8px**:

### 4.1. Escala de Espaçamento

```css
--space-1:  4px;
--space-2:  8px;
--space-3:  12px;
--space-4:  16px;
--space-5:  20px;
--space-6:  24px;
--space-8:  32px;
--space-10: 40px;
--space-12: 48px;
--space-16: 64px;
--space-20: 80px;
--space-24: 96px;
```

### 4.2. Layout e Breakpoints

- **Container Máximo:** `1200px` centralizado com `margin: 0 auto;`.
- **Preenchimento de Margem (Padding do Container):**
  - Mobile (< 640px): `16px` (`--space-4`)
  - Tablet (640px – 1024px): `24px` (`--space-6`)
  - Desktop (> 1024px): `32px` (`--space-8`)
- **Breakpoints Responsivos:**
  - `sm`: `640px` (Smartphones em modo paisagem / phablets)
  - `md`: `768px` (Tablets / telas intermediárias)
  - `lg`: `1024px` (Laptops / desktops comuns)
  - `xl`: `1280px` (Telas grandes)

---

## 5. Bordas, Sombras e Transições

### 5.1. Raio de Borda (Border Radius)

- `--radius-sm`: `6px` (Tags, badges pequenos, inputs compactos)
- `--radius-md`: `10px` (Botões de ação, caixas de diálogo)
- `--radius-lg`: `16px` (Cards de serviços, containers de destaque)
- `--radius-xl`: `24px` (Banners principais e containers de imagem)
- `--radius-full`: `9999px` (Pills, botões flutuantes, botões redondos)

### 5.2. Sombras (Box Shadow)

- `--shadow-sm`: `0 1px 2px 0 rgba(0, 0, 0, 0.05)` (Elementos sutis e botões em repouso)
- `--shadow-md`: `0 4px 6px -1px rgba(0, 0, 0, 0.08), 0 2px 4px -2px rgba(0, 0, 0, 0.05)` (Cards de serviços e pet shop)
- `--shadow-lg`: `0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.05)` (Cards em hover e modais)
- `--shadow-whatsapp`: `0 8px 24px -4px rgba(37, 211, 102, 0.45)` (Botão flutuante do WhatsApp)

### 5.3. Transições

- Padrão de velocidade: `all 0.2s cubic-bezier(0.4, 0, 0.2, 1)` para interações ágeis e suaves.

---

## 6. Padrões de Componentes

### 6.1. Header e Navegação
- **Fixo / Sticky:** Altura aproximada de `72px` no desktop e `64px` no mobile.
- **Fundo:** Branco puro (`#FFFFFF`) com borda inferior sutil (`#E2E8F0`) e leve sombra ao rolar a página.
- **Estrutura:** Logotipo à esquerda, links de navegação com hover verde institucional e botão destacado para o WhatsApp à direita.
- **Menu Mobile:** Gaveta responsiva limpa, com botão hambúrguer acessível por toque e contraste adequado.

### 6.2. Botões (Buttons)

1. **Botão Primário (CTA Verde Institucional):**
   - Fundo: `--color-primary` (`#1B4D2E`)
   - Texto: `--color-text-inverse` (`#FFFFFF`)
   - Hover: Fundo `--color-primary-dark` (`#123520`), elevação de sombra.
   - Aplicação: Ações principais da página clínica, ver serviços e agendamentos.

2. **Botão de WhatsApp (Conversão Máxima):**
   - Fundo: `--color-whatsapp` (`#25D366`)
   - Texto: `--color-text-inverse` (`#FFFFFF`) com ícone oficial do WhatsApp
   - Hover: Fundo `--color-whatsapp-hover` (`#1EBE5D`)
   - Aplicação: Header, Hero, final de cards e botão flutuante.

3. **Botão Secundário / Outline:**
   - Fundo: Transparente
   - Borda: `2px solid var(--color-primary)`
   - Texto: `--color-primary` (`#1B4D2E`)
   - Hover: Fundo `--color-primary-soft` (`#EAF4EE`)

4. **Botão Destaque Coral (Acentos Especiais):**
   - Fundo: `--color-secondary` (`#D93829`)
   - Texto: `--color-text-inverse` (`#FFFFFF`)
   - Hover: Fundo `--color-secondary-hover` (`#B8281A`)
   - Aplicação: Destaques de entrega e avisos pontuais.

5. **Botão Flutuante de WhatsApp (`Floating WhatsApp`):**
   - Posição: Fixo no canto inferior direito (`bottom: 24px; right: 24px; z-index: 1000;`).
   - Formato: Circular (`60px x 60px`), cantos arredondados full, com ícone de conversa e sombra `--shadow-whatsapp`.

### 6.3. Cards (Serviços e Produtos)
- **Fundo:** `--color-surface` (`#FFFFFF`)
- **Borda:** `1px solid var(--color-border)`
- **Raio:** `--radius-lg` (`16px`)
- **Preenchimento:** `24px` (`--space-6`)
- **Efeito Hover:** Translado sutil de `-4px` no eixo Y e sombra `--shadow-lg`, reforçando interatividade.
- **Hierarquia Interna:** Ícone ou imagem temática no topo, badge de categoria, título H3, descrição objetiva e botão de ação para WhatsApp.

### 6.4. Banner de Aviso de Emergência e Horários (`EmergencyNotice`)
- **Finalidade:** Atender obrigatoriamente à regra de nunca induzir o cliente a acreditar em atendimento 24h ou funcionamento aos domingos.
- **Fundo:** `--color-accent-yellow-soft` (`#FEF9E7`) com borda `--color-alert-border` (`#F59E0B`).
- **Texto:** `--color-alert-text` (`#78350F`) com ícone informativo visível.
- **Aviso Expresso:** *"Atenção: A Clínica não oferece atendimento veterinário emergencial 24 horas e não abre aos domingos. Consulte nossos horários oficiais de funcionamento (Seg–Sex: 08:00 às 18:00, Sáb: 08:00 às 13:00)."*

### 6.5. Rodapé Institucional (`Footer`)
- **Fundo:** `--color-primary-dark` (`#123520`)
- **Texto e Links:** `--color-text-inverse` com links em tom suave (`#CBD5E1`) e hover em branco puro.
- **Conteúdo Integrado:** Logotipo, resumo comercial, horários completos (Seg–Sex: 08h às 18h; Sáb: 08h às 13h), endereço em Campina Grande-PB (Rua das Acácias, 245), links para as 5 páginas, WhatsApp ((83) 99999-1234) e Instagram oficial (@bichofeliz.pet).

---

## 7. Folha de Estilos de Tokens CSS Prontos (`tokens.css`)

```css
:root {
  /* Cores Primárias */
  --color-primary: #1B4D2E;
  --color-primary-dark: #123520;
  --color-primary-light: #2D7A49;
  --color-primary-soft: #EAF4EE;

  /* Cores Secundárias e Acentos */
  --color-secondary: #D93829;
  --color-secondary-hover: #B8281A;
  --color-secondary-soft: #FDF2F0;
  --color-accent-yellow: #F6C90E;
  --color-accent-yellow-soft: #FEF9E7;

  /* Redes e Conversão */
  --color-whatsapp: #25D366;
  --color-whatsapp-hover: #1EBE5D;
  --color-instagram: #E1306C;

  /* Neutros e Superfícies */
  --color-bg: #FFFFFF;
  --color-bg-alt: #F8FAFC;
  --color-surface: #FFFFFF;
  --color-border: #E2E8F0;
  --color-border-hover: #CBD5E1;

  /* Tipografia / Textos */
  --color-text-main: #1E293B;
  --color-text-muted: #64748B;
  --color-text-inverse: #FFFFFF;

  /* Alertas e Avisos */
  --color-alert-bg: #FEF9E7;
  --color-alert-border: #F59E0B;
  --color-alert-text: #78350F;

  /* Fontes */
  --font-display: 'Montserrat', system-ui, -apple-system, sans-serif;
  --font-body: 'Inter', system-ui, -apple-system, sans-serif;

  /* Espaçamentos */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-5: 20px;
  --space-6: 24px;
  --space-8: 32px;
  --space-10: 40px;
  --space-12: 48px;
  --space-16: 64px;
  --space-20: 80px;

  /* Raios de Borda */
  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  /* Sombras */
  --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.08), 0 2px 4px -2px rgba(0, 0, 0, 0.05);
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.05);
  --shadow-whatsapp: 0 8px 24px -4px rgba(37, 211, 102, 0.45);

  /* Transição */
  --transition-default: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
}
```
