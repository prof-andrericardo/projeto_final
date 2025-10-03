# 📑 Módulo 6: **Projeto Final Guiado – SGSA**

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge Aulas](https://img.shields.io/badge/Aulas-12-blue)
![Badge Projeto](https://img.shields.io/badge/Projeto-SGSA-blueviolet)
![Badge Integração](https://img.shields.io/badge/Fullstack-Completo-green)

---

## 📖 Sobre o Módulo

Este módulo tem como objetivo consolidar todo o aprendizado dos módulos anteriores por meio do **desenvolvimento guiado do SGSA (Sistema de Gerenciamento de Sala de Aula)**.  

Ao final, o aluno terá construído uma versão funcional e integrada do sistema, com frontend responsivo, backend estruturado, banco de dados conectado e API REST consumida em tempo real.  

---

## 🔹 Aulas

### Aula 1 — Revisão de Estrutura do Projeto

- Revisão da arquitetura geral (frontend + backend + banco).  
- Organização das pastas do projeto final.  
- Checklist inicial.  

### Aula 2 — Login e Autenticação

- Fluxo de login conectado à API.  
- Sessão JWT armazenada no frontend.  
- Redirecionamento pós-login.  

### Aula 3 — Dashboard Dinâmico

- Cards com KPIs reais (turmas, alunos, ocorrências).  
- Consumo de endpoints e atualização automática.  

### Aula 4 — Gestão de Turmas

- CRUD completo de turmas integrado ao MySQL.  
- Listagem dinâmica e formulário com validação.  

### Aula 5 — Gestão de Alunos

- CRUD completo de alunos vinculado às turmas.  
- Ficha de aluno com dados e ocorrências.  

### Aula 6 — Registro de Aulas e Chamada

- CRUD de aulas integrado ao backend.  
- Tela de chamada com marcação de presença/falta.  

### Aula 7 — Ocorrências

- Cadastro e listagem de ocorrências por aluno.  
- Relatórios básicos de ocorrências.  

### Aula 8 — Tarefas

- Cadastro e listagem de tarefas.  
- Upload de anexos com backend.  

### Aula 9 — Relatórios Consolidados

- Relatórios de frequência e ocorrências por turma/aluno.  
- Exportação para CSV e impressão com CSS.  

### Aula 10 — Gráficos e Visualizações

- Integração com **Chart.js**.  
- Gráficos de frequência e ocorrências no dashboard.  

### Aula 11 — Revisão Geral do Sistema

- Testes cruzados (frontend + backend).  
- Correções e ajustes de bugs.  

### Aula 12 — Entrega e Publicação

- Publicação do frontend no GitHub Pages.  
- Execução do backend + banco em servidor local/VM.  
- Apresentação do sistema final.  

---

## 📅 Cronograma — Módulo 6 (Projeto Final Guiado | 12 aulas)

| Aula | Tema / Foco          | Objetivos de Aprendizagem         | Conteúdos & Componentes            | Prática em Sala                      | Entregáveis            |
| ---- | -------------------- | --------------------------------- | ---------------------------------- | ------------------------------------ | ---------------------- |
| 1    | Estrutura do projeto | Revisar arquitetura completa      | Frontend + Backend + Banco         | Organizar pastas e dependências      | Projeto configurado    |
| 2    | Login e Autenticação | Implementar autenticação JWT      | Fluxo login, sessão JWT            | Login integrado ao backend           | Login funcional        |
| 3    | Dashboard Dinâmico   | Exibir KPIs reais                 | Fetch KPIs, atualização automática | Dashboard com dados                  | Dashboard real         |
| 4    | Turmas               | Gerenciar turmas                  | CRUD Turmas, validação             | Tela de turmas conectada ao banco    | CRUD Turmas            |
| 5    | Alunos               | Gerenciar alunos                  | CRUD Alunos, vínculo Turma         | Tela de alunos integrada             | CRUD Alunos            |
| 6    | Aulas e Chamada      | Registrar aulas e presença        | CRUD Aulas, chamada dinâmica       | Tela de chamada funcionando          | Registro de presença   |
| 7    | Ocorrências          | Cadastrar ocorrências             | CRUD Ocorrências, filtros          | Tela de ocorrências conectada        | CRUD Ocorrências       |
| 8    | Tarefas              | Gerenciar tarefas com upload      | CRUD Tarefas, multer               | Cadastro e upload funcionando        | CRUD Tarefas           |
| 9    | Relatórios           | Consolidar relatórios             | Filtros, CSV, impressão CSS        | Relatórios de frequência/ocorrências | Relatórios exportáveis |
| 10   | Gráficos             | Exibir gráficos no dashboard      | Chart.js, integração API           | Gráficos de frequência e ocorrências | Dashboard visual       |
| 11   | Revisão Geral        | Ajustar bugs e revisar integração | Testes finais                      | Correções no SGSA                    | SGSA revisado          |
| 12   | Entrega Final        | Publicar sistema completo         | GitHub Pages + servidor backend    | Apresentação do sistema              | SGSA publicado         |

---

## 📂 Estrutura de pastas (organização sugerida)

```plaintext
sgsa-projeto-final/
  frontend/
    assets/
    pages/
  backend/
    src/
      config/
      controllers/
      models/
      routes/
      middlewares/
    uploads/
  database/
    schema.sql
    seeds.sql
  docs/
  README.md
```

------

## ✅ Checklist de QA (usar ao final de cada aula)

**Funcionalidade**

- CRUDs funcionando em todas as entidades.
- Relatórios e gráficos exibindo dados reais.
- Login com autenticação JWT ativo.

**Usabilidade**

- Interface responsiva e intuitiva.
- Feedback visual em formulários e ações.
- Exportação de relatórios funcionando.

**Boas práticas**

- Código organizado (MVC no backend, componentes no frontend).
- Scripts SQL versionados.
- Documentação mínima no README.

**Integração**

- Frontend consumindo API em todas as telas.
- Backend conectado ao MySQL.
- Publicação validada (frontend + backend).

------

## 📌 Entrega final do Módulo 6

- **Sistema SGSA funcional e integrado**.
- CRUDs completos (Alunos, Turmas, Professores, Aulas, Tarefas, Ocorrências).
- Relatórios dinâmicos e exportáveis.
- Gráficos interativos no dashboard.
- Publicação do frontend no GitHub Pages e backend em ambiente local/servidor.

------

## 🔗 Próximos Passos

Encerrando o ciclo, este módulo representa a **conclusão do projeto integrador**.
 O próximo passo será a **documentação final** (relatórios, manuais de uso, guias técnicos) para consolidar a entrega acadêmica/profissional do SGSA.

------

## 🎯 Critérios de Avaliação

Os alunos serão avaliados pelos seguintes critérios:

- Implementação completa do SGSA (frontend + backend + banco).
- Autenticação JWT funcionando corretamente.
- Relatórios e gráficos dinâmicos entregues.
- Publicação validada e apresentação final.
- Qualidade geral da interface e do código.
