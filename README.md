# 🟢 UpSkill ServiceNow Hub — Trainee Workspace

Este repositório contém o projeto prático desenvolvido no âmbito do módulo de **Programação em JavaScript** da **UpSkill ServiceNow (Turma 2026)**.

O objetivo principal do trabalho consiste na aplicação integrada e consolidação dos conhecimentos adquiridos em aula sobre as fundações de **HTML5** e **CSS3**, simulando um ambiente de desenvolvimento corporativo focado no ecossistema **ServiceNow**.

---

## 🎯 Objetivo & Escopo do Trabalho

O projeto foi desenhado sob o padrão visual e de governança técnica da **Deloitte**, imitando um portal de documentação e cockpit de aprendizagem SaaS (*Software as a Service*). Através desta interface, um consultor em formação (*Trainee*) consegue:
1. **Monitorizar o progresso geral** ao longo do *track* de engenharia core.
2. **Consultar o índice de lições** e navegar através de documentação técnica focada em *Client-Side Scripting*.
3. **Simular boas práticas** e validar regras de negócio num ambiente interativo de testes (*Sandbox*).

---

## ⚙️ Arquitetura Técnica & Melhores Práticas Aplicadas

Para cumprir os requisitos académicos estritos da UpSkill, o projeto foi blindado utilizando técnicas modernas de Engenharia Web Core, sem dependência de bibliotecas externas complexas:

*   **Estrutura Semântica Avançada:** Utilização disciplinada de tags HTML5 puras (`<header>`, `<aside>`, `<main>`, `<footer>`, `<article>`) para garantir acessibilidade e SEO técnico.
*   **Design System Escalável (CSS Variáveis):** Centralização da paleta corporativa (**Verde Deloitte** e tons escuros **ServiceNow Polaris**) através de propriedades `:root`.
*   **Layout Bidimensional Responsivo (CSS Grid):** Divisão macro do ecrã em formato *Master-Detail* (Sidebar de 280px fixa + Workspace fluído `1fr`), além de grelhas preditivas auto-ajustáveis para os cartões de módulos.
*   **Alinhamento Unidimensional Preciso (Flexbox):** Organização horizontal de elementos complexos, tais como o cabeçalho global, botões utilitários de ação e os cartões pequenos de sumário (KPIs).
*   **Separação Estrita de Conceitos:** Todo o design foi centralizado num ficheiro externo unificado (`css/estilo.css`), erradicando a poluição de estilos embutidos (`style=""`).
*   **Segurança e Resiliência Web:** Integração de *HTML Entities* (`&gt;`, `&lt;`) para formatação segura de *breadcrumbs* e renderização estável de fontes e ícones em modo self-hosted/dinâmico.

---

## 🛠️ Funcionalidades de Destaque Desenvolvidas

*   **Navegação Inteligente por Camadas (Workaround CSS):** Implementação de *links fantasma* absolutos combinados com elevação de `z-index`, permitindo que um único cartão físico direcione para dois caminhos lógicos diferentes (Módulo geral vs. Lição ativa atual).
*   **Interruptor de Modo Escuro Simplificado:** Integração de um gatilho reativo via JavaScript nativo inline (`classList.toggle`) associado ao ícone da lua, aplicando uma inversão cromática uniforme na Sidebar e no Workspace sem desformatar o layout.
*   **Dropdown de Perfil Dinâmico:** Menu flutuante interativo configurado por clique através da pseudo-classe `:focus-within` associada ao atributo `tabindex="0"`, eliminando a necessidade de scripts pesados de terceiros.
*   **Matriz Comparativa de Escopos (ES6+):** Grelha técnica responsiva construída em CSS Grid para comparar de forma legível e clara os impactos na memória de `var`, `let` e `const`.

---

## 🐙 Governação de Código & Boas Práticas de Git/GitHub

O ciclo de desenvolvimento deste portal foi gerido sob metodologias ágeis de controlo de versões, aplicando os standards recomendados para repositórios corporativos:

*   **Estratégia de Branching (Feature Branches):** A branch `main` foi blindada e mantida como uma cópia estável de produção. Cada componente do portal (como o Header, a Sidebar ou as páginas de lições) nasceu e foi isolado numa branch de funcionalidade dedicada (ex: `feature/homepage-layout`, `feature/licao1-matriz`).
*   **Mensagens de Commit Semânticas (Conventional Commits):** Para garantir um histórico de código limpo, auditável e legível por qualquer arquiteto da equipa, utilizou-se o padrão internacional de prefixos claros.
*   **Integração Contínua Displiplinada:** Antes de cada fusão (*Merge*), o código foi revisto localmente no Live Server em ambientes simulados de ecrã para anular regressões visuais e conflitos estruturais antes de subir ao GitHub.

---

## 🚀 Como Executar o Projeto Localmente

1. Garanta que tem a extensão **Live Server** instalada no seu VS Code.
2. Clone este repositório para a sua máquina local.
3. Clique com o botão direito do rato no ficheiro `index.html` e selecione **"Open with Live Server"**.
4. Explore a transição fluída entre o Dashboard principal e o ecossistema de lições clicando nos botões ou cartões ativos.

---

## 📚 Referências Visuais & Créditos

O design system e o alinhamento estético deste workspace foram baseados nas diretivas e componentes estruturais do **Google Stitch**, garantindo uma interface polida, moderna e focada em produtividade SaaS.

*   **Projeto de Referência:** [Google Stitch - Dashboard Project](https://stitch.withgoogle.com/projects/16635127389998481073)