# 🐾 VetCare — Hospital Veterinário e Centro Diagnóstico

Uma aplicação web front-end completa e moderna desenvolvida para o **Hospital Veterinário VetCare**. O projeto foi construído focando em usabilidade, navegação fluida, acessibilidade, performance e fidelidade visual às diretrizes de marca fornecidas.

---

## 📌 Visão Geral e Objetivo do Projeto

O projeto **VetCare** consiste no desenvolvimento de uma landing page institucional interativa para apresentação de serviços médicos e diagnósticos veterinários. A interface foi projetada para cobrir 100% da viewport (tela cheia), permitindo que tutores de animais encontrem rapidamente informações essenciais sobre o corpo clínico, especialidades oferecidas, preparo para exames e canais de atendimento direto via WhatsApp.

### 🎯 Principais Objetivos Alcançados:
- **Acessibilidade e Semântica:** Uso rigoroso de elementos HTML5 para garantir leitura clara e suporte a leitores de tela.
- **Experiência de Navegação:** Transição suave entre seções com tratamento de rolagem e links de âncora personalizados.
- **Arquitetura Escalável:** Aplicação de padrões de código limpo e separação modular de arquivos CSS.

---

## 🖼️ Seções da Aplicação

A página foi organizada em seções integradas e acessíveis pelo menu de navegação lateral:

1. **Início (`#home`):** Apresentação principal (Hero) com frase de impacto, descrição do centro diagnóstico e botão de agendamento rápido via WhatsApp.
2. **Quem Somos (`#sobre`):** Apresentação do hospital, histórico de atuação, estrutura moderna e pilares de atendimento humanizado.
3. **Corpo Clínico (`#equipe`):** *Cards* informativos apresentando os médicos veterinários responsáveis (Dra. Camila Nogueira e Dr. Rafael Santos), CRMVs e áreas de atuação.
4. **Infraestrutura (`#infraestrutura`):** Destaques para o Centro Cirúrgico, Laboratório Próprio e Sala de Internação.
5. **Especialidades (`#servicos`):** Apresentação detalhada dos serviços de Odontologia, Oftalmologia, Ortopedia e Cardiologia em formato de grid.
6. **Dúvidas Frequentes (`#faq`):** Sistema acordeão nativo (`<details>` e `<summary>`) esclarecendo dúvidas sobre jejum para exames, atendimento de emergência 24h e agendamentos.
7. **Rodapé Fixo (`footer`):** Informações de endereço, horário de atendimento e contatos institucionais acessíveis em todas as telas.

---

## 🛠️ Tecnologias e Conceitos Aplicados

### 🟢 HTML5 Semântico & Acessibilidade
- Uso exclusivo das tags `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<details>`, `<summary>` e `<footer>`.
- Atributos `alt` detalhados em todas as imagens para garantir acessibilidade visual.

### 🎨 CSS3 Moderno & Design System
- **Metodologia BEM (Block Element Modifier):** Padrão de escrita limpo e independente de especificidade para seletores (ex: `.card`, `.card__header`, `.card__button--accent`).
- **Variáveis Globais (`variable.css`):**
  - **Paleta de Cores:**
    - Primary Color: `#1E3A8A` (Azul Escuro institucional)
    - Secondary Color: `#0284C7` (Azul Médio)
    - Light Background: `#F8FAFC` / Surface: `#FFFFFF`
    - Accent / Highlight: `#10B981` (Verde para destaque e CTA)
    - Text Main: `#1E293B` / Text Secondary: `#64748B`
  - **Tipografia:** Fonte externa **Poppins** (pesos 400, 500, 600, 700) importada do Google Fonts.
  - **Efeitos e Microinterações:** Sombras sutis (`box-shadow`) e transições em estados de `:hover` nos *cards* e botões.

### 📐 Unidades Relativas & Responsividade
- **Zero uso de pixels fixos** em dimensões estruturais e textos, adotando estritamente `rem`, `%`, `vh` e `vw`.
- Uso restrito de `px` somente para bordas decorativas de 1px ou 2px.

---

🚀 Como executar
Clone este repositório:

git clone https://github.com/julia-beatris/VetCare.git

Abra o arquivo index.html no navegador.

## 📂 Organização da Arquitetura de Arquivos

O projeto adota uma estrutura modularizada de arquivos CSS para manter a organização, reutilização de estilos e facilidade de manutenção:

```text
├── CSS/
│   ├── reset.css         # Normalização e remoção de margens/estilos padrão dos navegadores
│   ├── responsive.css    # Regras e ajustes de responsividade para diferentes tamanhos de tela
│   ├── style.css         # Estilização dos componentes, seções e layout da aplicação
│   └── variable.css      # Definição das variáveis globais (cores, fontes, espaçamentos)
├── index.html            # Estrutura HTML semântica principal da aplicação
└── README.md             # Documentação completa do projeto