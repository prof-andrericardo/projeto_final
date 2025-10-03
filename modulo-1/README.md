# 📑 Módulo 1: **Frontend SGSA com Mobile-First e Bootstrap**

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge Aulas](https://img.shields.io/badge/Aulas-12-blue)
![Badge Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-purple)

---

## 📖 Sobre o Módulo

Este módulo tem como objetivo desenvolver o **Frontend do SGSA (Sistema de Gerenciamento de Sala de Aula)** utilizando conceitos de **mobile-first, Bootstrap e acessibilidade digital**.  

Ao final, o aluno terá construído um **protótipo navegável** do sistema, cobrindo as telas de **Login, Dashboard, Turmas, Alunos, Aulas, Chamada, Tarefas, Ocorrências, Relatórios e Perfil**, já pronto para integração futura com backend e banco de dados.

---

## 🔹 Aulas

### Aula 1 — Mobile-First + Escopo UX do SGSA

- Introdução ao conceito de **mobile-first**.  
- Criação do **sitemap** e **wireframes** das telas principais.  
- Definição do escopo visual do SGSA.  

### Aula 2 — Setup do Projeto + Design System

- Estrutura inicial de pastas e arquivos.  
- Integração do **Bootstrap via CDN**.  
- Definição de **tokens de design**: cores, tipografia, espaçamentos.  

### Aula 3 — Grid e Layout Base

- Uso do **sistema de grid do Bootstrap**.  
- Criação do layout principal com **header fixo** e **menu offcanvas**.  
- Aplicação de containers e breakpoints.  

### Aula 4 — Navegação e Acessibilidade

- Criação da **navbar responsiva**.  
- Uso de **breadcrumbs** e landmarks ARIA.  
- Aplicação de boas práticas de **Acessibilidade Digital (A11y)**.  

### Aula 5 — Formulários (Login e Cadastro)

- Construção de **formulários responsivos**.  
- Feedback visual (validação) com Bootstrap.  
- Telas: **Login** e **Cadastro de Tarefas** (UI).  

### Aula 6 — Tabelas e Listagens (Turmas/Alunos)

- Criação de **tabelas responsivas** com Bootstrap.  
- Paginação e filtros simples (offcanvas).  
- Páginas: **Turmas** e **Alunos**.  

### Aula 7 — Cards e Dashboard

- Uso de **cards** para resumos visuais (KPIs).  
- Implementação de **badges, tooltips e toasts**.  
- Construção do **Dashboard inicial** do SGSA.  

### Aula 8 — Modais e Fluxos Críticos

- Uso de **modais** para confirmações e formulários rápidos.  
- Aplicação de **offcanvas avançado** para filtros.  
- Telas: **Tarefas** e **Ocorrências** com modais.  

### Aula 9 — Páginas de Aulas e Chamada

- Criação da página de **Aulas** com lista e detalhes.  
- Tela de **Chamada de presença** (P/F/A) com inputs acessíveis.  
- Fluxo completo: Aula → Chamada.  

### Aula 10 — Relatórios (Frequência e Ocorrências)

- Construção de relatórios com tabelas filtráveis.  
- Botões de exportação (CSV fake) e impressão com CSS.  
- Telas: **Relatório de Frequência** e **Relatório de Ocorrências**.  

### Aula 11 — Performance e Qualidade

- Refinos de UX: ícones (Bootstrap Icons), imagens responsivas.  
- Teste de qualidade com **Lighthouse** (auditoria local).  
- Organização de código e componentização.  

### Aula 12 — Congelamento do Frontend (UI Final)

- Revisão geral de **responsividade e acessibilidade**.  
- Ajustes finais de layout e consistência.  
- Publicação do **Frontend SGSA v1** (GitHub Pages).  

---

## 📅 Cronograma — Módulo 1 (Frontend SGSA | 12 aulas)

| Aula | Foco / Tela              | Objetivos de Aprendizagem                                | Conteúdos & Componentes                      | Prática em Sala                               | Entregáveis                              |
| ---- | ------------------------ | -------------------------------------------------------- | -------------------------------------------- | --------------------------------------------- | ---------------------------------------- |
| 1    | Visão geral + UX         | Definir escopo, mapa de navegação e padrões mobile-first | Mobile-first, semântica, sitemap, wireframes | Wireframes das telas principais (papel/figma) | **Sitemap** + **Wireframes**             |
| 2    | Setup + Design System    | Padronizar tokens de UI                                  | Bootstrap via CDN, variáveis CSS             | Criar `index.html` + `styles.css` (tokens)    | **Base HTML** + **styles.css**           |
| 3    | Grid & Layout            | Estruturar layout mestre responsivo                      | Containers, grid, breakpoints                | Layout com **header** + **offcanvas**         | **Template base**                        |
| 4    | Navegação & A11y         | Implementar navegação acessível                          | Navbar, breadcrumbs, landmarks ARIA          | Navbar fixa + breadcrumbs                     | **Navegação funcional** + checklist A11y |
| 5    | Formulários: Login       | Construir formulários consistentes                       | Forms, validação, feedback visual            | **Login** + **Cadastro Tarefas (UI)**         | **login.html** + **tarefas.html**        |
| 6    | Tabelas: Turmas/Alunos   | Criar listagens legíveis e responsivas                   | Tables responsivas, filtros (offcanvas)      | **Turmas** + **Alunos**                       | **turmas.html** + **alunos.html**        |
| 7    | Cards & Dashboard        | Sintetizar KPIs e empty states                           | Cards, badges, tooltips, toasts              | Criar **Dashboard** com 4 indicadores         | **dashboard.html**                       |
| 8    | Modais & Fluxos Críticos | Confirmar ações sensíveis                                | Modals, offcanvas avançado                   | **Tarefas** e **Ocorrências** com modais      | **modals** aplicados                     |
| 9    | Aulas & Chamada          | Preparar diários e chamada                               | Lists, inputs acessíveis, navegação teclado  | **aulas.html** + **chamada.html** (P/F/A)     | Fluxo Aula → Chamada                     |
| 10   | Relatórios (2 telas)     | Exibir dados com filtros e impressão                     | Tables, filtros, export CSV, `@media print`  | **Relatórios Frequência + Ocorrências**       | **relatorios-*.html**                    |
| 11   | Performance & Qualidade  | Refinar UX, peso e organização                           | Bootstrap Icons, imagens, Lighthouse         | Revisão CSS/HTML e otimizações                | **Refino UI** + notas auditoria          |
| 12   | Congelamento de UI       | Preparar handoff para backend                            | Revisão A11y, consistência, responsividade   | Testes cruzados de telas/fluxos               | **Frontend v1 publicado** (GitHub Pages) |

---

## 📂 Estrutura de pastas (organização sugerida)

```plaintext
sgsa-frontend/
  assets/
    css/ (styles.css, overrides.css)
    img/
    icons/
  components/ (header.html, sidebar.html, modals.html, footer.html)
  pages/
    dashboard.html
    login.html
    turmas.html
    alunos.html
    aulas.html
    chamada.html
    tarefas.html
    ocorrencias.html
    relatorios-frequencia.html
    relatorios-ocorrencias.html
    perfil.html
  index.html  (redirige para login/dashboard)
  README.md
```

------

## ✅ Checklist de QA (usar ao final de cada aula)

**Responsividade**

- Layout íntegro em `sm`, `md`, `lg`, `xl` (sem overflow horizontal).
- Navbar/offcanvas funcionam em telas pequenas.

**Acessibilidade**

- Hierarquia de títulos coerente (`h1` → `h2` → `h3`).
- Labels associados a inputs; foco visível; navegação por teclado.
- Elementos interativos com `aria-label`/`aria-controls` quando necessário.

**Consistência visual**

- Tokens de cor e tipografia aplicados (nada fora do padrão).
- Espaçamentos com utilitários Bootstrap (evitar CSS ad-hoc excessivo).

**Boas práticas**

- Componentes reutilizáveis em `components/` (header, sidebar, modals).
- Comentários úteis nos arquivos; nomes de classes previsíveis.
- Preparado para API: IDs/classes onde haverá injeção de dados.

**Qualidade**

- Peso razoável (sem libs desnecessárias); imagens otimizadas.
- `@media print` nos relatórios; botão “Exportar CSV” como placeholder.

------

## 📌 Entrega final do Módulo 1

- **Frontend navegável** cobrindo: Login, Dashboard, Turmas, Alunos, Aulas, Chamada, Tarefas, Ocorrências, Relatórios (2 telas) e Perfil (UI).
- **Publicação:** link do GitHub Pages (ou equivalente).
- **README.md** com:
  - Descrição do projeto (SGSA – Frontend v1)
  - Estrutura de pastas
  - Padrões de UI/UX (tokens, componentes)
  - Telas prontas e pendências
  - Como executar localmente / como publicar

------

## 🔗 Próximos Passos

No **Módulo 2**, será desenvolvido o **Backend em Node.js**, criando a **API REST** que fornecerá os dados para o frontend construído neste módulo.

------

## 🎯 Critérios de Avaliação

Os alunos serão avaliados pelos seguintes critérios:

- Responsividade em múltiplos dispositivos.
- Acessibilidade mínima (labels, foco visível, navegação por teclado).
- Padrão de design consistente (tokens, componentes).
- Publicação correta no GitHub Pages.

