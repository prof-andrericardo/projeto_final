# 📑 Módulo 5: **Integração Frontend + Backend do SGSA**

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge Aulas](https://img.shields.io/badge/Aulas-10-blue)
![Badge Frontend](https://img.shields.io/badge/Frontend-Bootstrap-orange)
![Badge Backend](https://img.shields.io/badge/Backend-Node.js-green)
![Badge API](https://img.shields.io/badge/API-REST-blue)

---

## 📖 Sobre o Módulo

Este módulo tem como objetivo **integrar o Frontend do SGSA (construído no Módulo 1)** com a **API RESTful desenvolvida nos Módulos 2, 3 e 4**.  

Ao final, o aluno terá um sistema **dinâmico e interativo**, consumindo dados reais do banco via API, com formulários, tabelas e relatórios atualizados em tempo real.

---

## 🔹 Aulas

### Aula 1 — Introdução à Integração Frontend + Backend

- Revisão do frontend estático.  
- Conceito de consumo de APIs REST.  
- Estruturação inicial para integração.  

### Aula 2 — Fetch API e Requisições Assíncronas

- Uso de **Fetch API** no JavaScript.  
- Requisições GET e POST.  
- Tratamento de respostas e erros.  

### Aula 3 — Listagem Dinâmica (Turmas e Alunos)

- Consumo da rota `/alunos` e `/turmas`.  
- Renderização dinâmica em tabelas.  

### Aula 4 — Formulários Integrados

- Envio de dados via POST (cadastro de alunos/tarefas).  
- Feedback visual no frontend.  

### Aula 5 — Atualização e Exclusão de Registros

- Uso de PUT e DELETE via Fetch API.  
- Atualização automática da interface.  

### Aula 6 — Sessões e Tokens

- Armazenamento do token JWT no frontend.  
- Acesso a rotas protegidas.  
- Logout e controle de sessão.  

### Aula 7 — Relatórios Dinâmicos

- Consumo de endpoints com filtros.  
- Geração de tabelas e exportação CSV.  

### Aula 8 — Gráficos e Visualizações

- Integração com **Chart.js**.  
- Exibição de frequência e ocorrências em gráficos.  

### Aula 9 — Mini-Projeto de Integração

- Turmas, Alunos e Tarefas integrados ao backend.  
- Tela de ocorrências consumindo API.  

### Aula 10 — Revisão e Entrega

- Revisão geral da integração.  
- Checklist de funcionalidade.  
- Publicação do projeto final parcial.  

---

## 📅 Cronograma — Módulo 5 (Integração | 10 aulas)

| Aula | Tema / Foco             | Objetivos de Aprendizagem        | Conteúdos & Componentes       | Prática em Sala                     | Entregáveis              |
| ---- | ----------------------- | -------------------------------- | ----------------------------- | ----------------------------------- | ------------------------ |
| 1    | Introdução              | Revisar frontend e API REST      | Estrutura de integração       | Preparar frontend para consumo API  | Setup inicial            |
| 2    | Fetch API               | Realizar requisições assíncronas | GET/POST, async/await         | Testar requisições em tela simples  | Requisição funcionando   |
| 3    | Listagem dinâmica       | Popular tabelas com dados da API | InnerHTML, loops JS           | Tabela de Alunos/Turmas dinâmica    | Listagens integradas     |
| 4    | Formulários integrados  | Enviar dados para API            | POST, tratamento de erro      | Formulário cadastro aluno/tarefa    | Formulários conectados   |
| 5    | Atualizar/Excluir       | Consumir rotas PUT/DELETE        | Fetch PUT/DELETE              | Editar e excluir registros          | CRUD completo            |
| 6    | Sessões e Tokens        | Utilizar JWT no frontend         | LocalStorage/SessionStorage   | Login, logout, rotas protegidas     | Sessão funcional         |
| 7    | Relatórios dinâmicos    | Exibir relatórios da API         | Filtros, exportação CSV       | Relatório frequência/ocorrências    | Relatórios ativos        |
| 8    | Gráficos                | Visualizar dados em gráficos     | Chart.js, integração JS       | Gráfico de frequência e ocorrências | Gráficos visuais         |
| 9    | Mini-projeto integração | Consolidar CRUD + autenticação   | Frontend + Backend integrados | Sistema parcial SGSA                | Integração validada      |
| 10   | Revisão final           | Ajustar e publicar integração    | Checklist final               | Publicação GitHub Pages + API       | Projeto integrado online |

---

## 📂 Estrutura de pastas (organização sugerida)

```plaintext
sgsa-integration/
  frontend/
    assets/
    pages/
  backend/
    src/
    routes/
  docs/
  README.md
```

------

## ✅ Checklist de QA (usar ao final de cada aula)

**Funcionalidade**

- Frontend consumindo dados da API corretamente.
- CRUD integrado funcionando.
- Sessão JWT implementada.

**Usabilidade**

- Feedback visual em formulários e ações.
- Listagens atualizadas automaticamente.
- Relatórios e gráficos exibindo dados corretos.

**Boas práticas**

- Código JS comentado e organizado.
- Reuso de funções para chamadas API.
- Estrutura clara para futuras expansões.

------

## 📌 Entrega final do Módulo 5

- **Frontend integrado ao Backend** via API REST.
- CRUD completo consumindo dados reais.
- Sessões com JWT funcionando.
- Relatórios dinâmicos e gráficos básicos.
- Publicação no GitHub Pages (frontend) + Backend local/servidor.

------

## 🔗 Próximos Passos

No **Módulo 6**, será desenvolvido o **Projeto Final Guiado**, expandindo todas as funcionalidades e consolidando o SGSA como um sistema funcional.

------

## 🎯 Critérios de Avaliação

Os alunos serão avaliados pelos seguintes critérios:

- Integração completa do frontend com backend.
- CRUD funcional consumindo API real.
- Sessões e autenticação aplicadas corretamente.
- Relatórios e gráficos funcionando.
- Publicação no GitHub Pages e execução do backend.
