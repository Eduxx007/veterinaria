# Planejamento de implementação — Clínica Veterinária e Pet Shop Bicho Feliz

> **Nota:** Todos os dados comerciais, profissionais e institucionais apresentados neste documento são fictícios e foram estruturados exclusivamente para fins de desenvolvimento, demonstração e estudo.

## 1. Negócio, público e objetivo

**Negócio:**  
Clínica Veterinária e Pet Shop Bicho Feliz, localizada no Centro de Campina Grande - PB. Atua em três segmentos:
- **Clínica veterinária:** consultas veterinárias, cirurgias veterinárias e exames laboratoriais.
- **Estética animal:** banho e tosa.
- **Pet shop:** comercialização de rações, petiscos e acessórios, com suporte a entrega mediante consulta pelo WhatsApp.

**Público-alvo:**  
Tutores de cães e gatos de Campina Grande - PB e região, que procuram atendimento veterinário, serviços de higiene animal ou produtos para seus pets.

**Objetivo do site:**  
Estabelecer uma presença digital profissional, apresentar os serviços e produtos, facilitar a localização da empresa e converter visitantes em contatos pelo WhatsApp.

> **Importante:** O site não deverá transmitir a ideia de atendimento emergencial 24 horas e nem funcionamento aos domingos.

---

## 2. Páginas que serão construídas

Serão desenvolvidas cinco páginas independentes:

| Página | Rota | Finalidade |
|---|---|---|
| Início | `/` (`index.html`) | Apresentação da empresa e direcionamento para os serviços. |
| Clínica Veterinária | `/clinica-veterinaria` | Apresentação dos serviços clínicos e cirúrgicos. |
| Banho e Tosa | `/banho-e-tosa` | Divulgação dos serviços de estética animal. |
| Pet Shop | `/pet-shop` | Apresentação dos produtos e da entrega sob consulta. |
| Contato | `/contato` | Endereço, horários, mapa e canais de comunicação. |

Todas terão navegação compartilhada e acesso facilitado ao WhatsApp.

---

## 3. Componentes reutilizáveis

Os componentes serão desenvolvidos de forma modular e reutilizados em diferentes páginas, reduzindo duplicação e facilitando manutenção:

| Componente | Responsabilidade |
|---|---|
| **Header** | Logotipo, menu e navegação principal. |
| **MobileMenu** | Menu adaptado para dispositivos móveis (hambúrguer/gaveta). |
| **WhatsAppButton** | Botão flutuante e de seção de contato com link direto para o WhatsApp. |
| **HeroSection** | Título, descrição, imagem e CTA de cada página. |
| **SectionTitle** | Padronização dos títulos e subtítulos das seções. |
| **ServiceCard** | Apresentação dos serviços veterinários. |
| **CategoryCard** | Apresentação das categorias de produtos do pet shop. |
| **Gallery** | Exibição de fotografias e ilustrações autorizadas. |
| **BusinessHours** | Horários de funcionamento claros (Seg–Sex: 08h–18h; Sáb: 08h–13h). |
| **EmergencyNotice** | Aviso destacado sobre ausência de atendimento 24h e fechamento aos domingos. |
| **ContactInfo** | Telefone, endereço e link para Instagram oficial. |
| **LocationMap** | Exibição da localização confirmada (mapa embutido / link para navegação). |
| **FAQ** | Perguntas e respostas frequentes. |
| **CTASection** | Seção de chamada para ação antes do rodapé. |
| **Footer** | Informações institucionais, links rápidos, endereço e avisos. |

**Componentes prioritários:** `Header`, `WhatsAppButton`, `BusinessHours`, `EmergencyNotice` e `Footer`.  
Esses elementos deverão manter o mesmo comportamento e consistência visual em todas as páginas.

---

## 4. Regras visuais do design-system.md

As regras visuais foram consolidadas no documento [`design-system.md`](design-system.md):

- **Paleta de Cores Institucional:**
  - **Primária (Verde Floresta):** `#1B4D2E` (títulos, CTAs clínicos principais) e `#123520` (hover e rodapé).
  - **Secundária / Destaque (Vermelho Coral):** `#D93829` (destaque visual, badges de atenção e entrega).
  - **Acento Lúdico (Amarelo Dourado):** `#F6C90E` (elementos de estética e pet shop).
  - **Ação Rápida (Verde WhatsApp):** `#25D366` e `#1EBE5D` (botão flutuante e CTAs de conversão).
  - **Superfície e Neutros:** Branco `#FFFFFF`, Fundo alternado `#F8FAFC`, Borda `#E2E8F0`, Texto grafite `#1E293B` (>10:1 de contraste) e texto atenuado `#64748B`.
  - **Banner de Alerta (Aviso 24h):** Fundo suave `#FEF9E7`, borda âmbar `#F59E0B` e texto marrom `#78350F`.

- **Tipografia:**
  - **Títulos e Destaque:** `'Montserrat'`, sans-serif (pesos 600, 700, 800) — imponente e geométrica.
  - **Corpo e Interface:** `'Inter'`, sans-serif (pesos 400, 500, 600) — alta legibilidade em telas e interfaces móveis.

- **Espaçamento e Dimensões:**
  - Grid baseado em múltiplos de 4px / 8px (4, 8, 12, 16, 24, 32, 48, 64px).
  - Container máximo de 1200px com margens responsivas de 16px (mobile) a 32px (desktop).
  - Raios de borda: 10px (botões), 16px (cards), 9999px (pills e botão flutuante WhatsApp).

---

## 5. Aplicação das regras ao novo site

A aplicação é centralizada através do arquivo de variáveis e componentes CSS, garantindo coerência visual absoluta entre as 5 páginas:

| Elemento | Aplicação no site |
|---|---|
| **Cores** | Variáveis CSS em `:root` (`--color-primary`, `--color-secondary`, etc.), garantindo contraste WCAG AA em todos os textos e fundos. |
| **Tipografia** | Carregamento otimizado via Google Fonts; H1 a H4 padronizados com `'Montserrat'` e parágrafos com `'Inter'`. |
| **Espaçamento** | Seções com espaçamento vertical padronizado (48px mobile / 80px desktop) para respiro e hierarquia limpa. |
| **Botões** | 3 variantes bem definidas: Primário Verde (`.btn-primary`), WhatsApp Oficial (`.btn-whatsapp`) e Outline (`.btn-outline`). |
| **Cards** | Cards de serviços clínicos e produtos com fundo branco, borda sutil, cantos arredondados (16px) e elevação suave ao hover. |
| **Imagens** | Proporções e tratamentos consistentes, logotipo e ilustrações com texto alternativo acessível. |
| **Responsividade** | Layout Mobile-First, com menu hambúrguer interativo para telas menores que 768px. |
| **Avisos Obrigatórios** | Componente `EmergencyNotice` em destaque amarelo/âmbar informando horários e ausência de atendimento 24h. |

---

## 6. Plano de implementação

A implementação será dividida em sete etapas:

1. **Etapa 1 — Preparação do projeto**
   - Organizar a estrutura de pastas (`css/`, `js/`, `assets/`, etc.).
   - Configurar o ambiente de desenvolvimento.
   - Definir as rotas das cinco páginas.
   - Verificar o briefing, mapa do site e conteúdo oficial fictício.

2. **Etapa 2 — Design system**
   - Consultar o `design-system.md`.
   - Configurar variáveis CSS (cores, tipografia, espaçamentos).
   - Estabelecer padrões de botões, cards e tipografia.

3. **Etapa 3 — Componentes compartilhados**
   - Desenvolver `Header` e `MobileMenu`.
   - Desenvolver `Footer`.
   - Criar botão flutuante de `WhatsApp`.
   - Criar avisos de funcionamento e emergência (`EmergencyNotice`).
   - Criar cards e seções reutilizáveis.

4. **Etapa 4 — Desenvolvimento das páginas**
   - Ordem de implementação:
     1. Início (`index.html`)
     2. Clínica Veterinária (`clinica-veterinaria.html`)
     3. Pet Shop (`pet-shop.html`)
     4. Contato (`contato.html`)
     5. Banho e Tosa (`banho-e-tosa.html`)

5. **Etapa 5 — Integrações e mídias**
   - Configurar links do WhatsApp fictício (`(83) 99999-1234` / `https://wa.me/5583999991234`).
   - Configurar link do Instagram fictício (`@bichofeliz.pet` / `https://www.instagram.com/bichofeliz.pet/`).
   - Inserir mapa com a localização confirmada (Rua das Acácias, 245, Centro, Campina Grande - PB).
   - Inserir mídias e ilustrações com alt tags descritivas.

6. **Etapa 6 — Responsividade e acessibilidade**
   - Testar em celulares, tablets e computadores.
   - Verificar contraste de cores e legibilidade.
   - Garantir navegação por teclado e semântica HTML5.
   - Adicionar textos alternativos (`alt`) descritivos a todas as imagens.

7. **Etapa 7 — Testes e validação final**
   - Verificar todas as rotas e links internos/externos.
   - Conferir informações comerciais (horários 08h–18h, endereço, ausência de 24h).
   - Verificar desempenho e carregamento rápido.
   - Revisar SEO básico (meta tags, open graph, títulos).

---

## Critérios para considerar o projeto concluído

- [ ] Cinco páginas funcionando (`/`, `/clinica-veterinaria`, `/banho-e-tosa`, `/pet-shop`, `/contato`).
- [ ] Navegação consistente entre todas as páginas.
- [ ] Componentes reutilizáveis implementados e padronizados.
- [ ] Design system aplicado corretamente através de CSS padronizado.
- [ ] Layout totalmente responsivo (mobile-first).
- [ ] WhatsApp funcionando e acessível em todas as telas (`(83) 99999-1234`).
- [ ] Instagram configurado corretamente (`@bichofeliz.pet`).
- [ ] Endereço e horários de funcionamento precisos (Campina Grande - PB, Seg–Sex 08h–18h, Sáb 08h–13h).
- [ ] Aviso visível sobre fechamento aos domingos e ausência de atendimento 24h.
- [ ] Nenhuma informação da marca/empresa anterior presente nos arquivos.
- [ ] Testes de usabilidade e responsividade realizados.
