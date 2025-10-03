# 📑 Módulo 3: **Banco de Dados SGSA com MySQL**

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge Aulas](https://img.shields.io/badge/Aulas-8-blue)
![Badge MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![Badge Node.js](https://img.shields.io/badge/Node.js-20.x-brightgreen)

---

## 📖 Sobre o Módulo

Este módulo tem como objetivo introduzir o **Banco de Dados do SGSA (Sistema de Gerenciamento de Sala de Aula)** utilizando o **MySQL 8.0**.  

Ao final, o aluno terá aprendido a criar e manipular tabelas no MySQL, realizar consultas básicas e avançadas, trabalhar com relacionamentos e integrar o banco ao backend desenvolvido no **Módulo 2 (Node.js + Express)**.

---

## 🔹 Aulas

### Aula 1 — Introdução ao MySQL e DDL

- Conceitos de banco de dados relacional.  
- Criação de banco e tabelas com **DDL** (`CREATE`, `ALTER`, `DROP`).  
- Estrutura inicial para alunos, turmas e professores.  

### Aula 2 — Manipulação de Dados (DML)

- Inserção de registros com `INSERT`.  
- Atualização de registros com `UPDATE`.  
- Exclusão lógica/física com `DELETE`.  

### Aula 3 — Consultas Básicas (DQL)

- Uso de `SELECT`.  
- Filtros com `WHERE`, operadores lógicos e de comparação.  
- Ordenação com `ORDER BY` e limites com `LIMIT`.  

### Aula 4 — Relacionamentos e JOINs

- Criação de **chaves primárias e estrangeiras**.  
- Tipos de relacionamentos (1:1, 1:N, N:N).  
- Consultas com `INNER JOIN`, `LEFT JOIN` e `RIGHT JOIN`.  

### Aula 5 — Conexão MySQL com Node.js

- Instalação do **mysql2**.  
- Conexão ao banco pelo backend.  
- Testes de conexão com rotas simples.  

### Aula 6 — CRUD com Node.js + MySQL

- Implementação de CRUD completo no banco.  
- Rotas para alunos e turmas consumindo dados reais.  
- Tratamento de erros e exceções de banco.  

### Aula 7 — Validações e Integridade

- Restrições (`NOT NULL`, `UNIQUE`, `CHECK`).  
- Tratamento de chaves estrangeiras e cascatas.  
- Boas práticas para integridade referencial.  

### Aula 8 — Mini-Projeto: Integração Completa

- Backend do SGSA conectado ao MySQL.  
- CRUD real para alunos, turmas e professores.  
- Testes com Insomnia/Postman.  

---

## 📅 Cronograma — Módulo 3 (MySQL | 8 aulas)

| Aula | Foco / Tema       | Objetivos de Aprendizagem              | Conteúdos & Componentes                | Prática em Sala                           | Entregáveis               |
| ---- | ----------------- | -------------------------------------- | -------------------------------------- | ----------------------------------------- | ------------------------- |
| 1    | DDL               | Criar banco e tabelas                  | CREATE, ALTER, DROP                    | Criar BD SGSA com tabelas iniciais        | `schema.sql` inicial      |
| 2    | DML               | Manipular dados básicos                | INSERT, UPDATE, DELETE                 | Inserir, atualizar e excluir alunos       | `dados_iniciais.sql`      |
| 3    | DQL               | Consultar e filtrar dados              | SELECT, WHERE, ORDER BY, LIMIT         | Listagem filtrada de alunos/turmas        | Consultas SQL             |
| 4    | JOINs             | Relacionar tabelas                     | PK, FK, INNER JOIN, LEFT/RIGHT JOIN    | Relatórios de alunos por turma            | Consultas SQL com JOIN    |
| 5    | Conexão Node.js   | Integrar backend ao banco              | mysql2, conexão pool                   | Criar rota de teste `/db-status`          | Conexão ativa funcionando |
| 6    | CRUD Node + MySQL | Persistir dados reais                  | Express + MySQL (INSERT/SELECT/UPDATE) | CRUD completo de alunos/turmas            | API CRUD funcional        |
| 7    | Validações        | Garantir integridade e consistência    | Restrições, validações, cascatas       | Inserções com regras aplicadas            | Tabelas ajustadas         |
| 8    | Integração final  | Consolidar aprendizado em mini-projeto | API + BD + testes                      | CRUD de alunos/professores/turmas testado | API conectada ao MySQL    |

---

## 📂 Estrutura de pastas (organização sugerida)

```plaintext
sgsa-database/
  scripts/
    schema.sql
    dados_iniciais.sql
  migrations/
  tests/
sgsa-backend/
  src/
    config/db.js
    controllers/
    models/
    routes/
```

------

## ✅ Checklist de QA (usar ao final de cada aula)

**Banco de Dados**

- Tabelas criadas corretamente com PK e FK.
- Dados inseridos/atualizados/excluídos corretamente.
- JOINs retornando resultados esperados.

**Backend**

- Conexão com MySQL funcionando.
- Rotas do CRUD persistindo dados reais.
- Tratamento de erros implementado.

**Boas práticas**

- Scripts SQL organizados em `/scripts`.
- Código Node.js desacoplado (config/db.js).
- Nomes consistentes para tabelas e colunas.

------

## 📌 Entrega final do Módulo 3

- **Banco de Dados MySQL** criado e documentado (`schema.sql`).
- **CRUD real** funcionando no backend com persistência em MySQL.
- Scripts de migração e inserção inicial organizados.
- Testes de CRUD realizados via Insomnia/Postman.

------

## 🔗 Próximos Passos

No **Módulo 4**, será criada a **API RESTful completa**, conectada ao MySQL e com rotas estruturadas para atender ao frontend do SGSA.

------

## 🎯 Critérios de Avaliação

Os alunos serão avaliados pelos seguintes critérios:

- Banco de dados criado corretamente (tabelas, relacionamentos, integridade).
- CRUD persistindo dados reais no MySQL.
- Integração entre backend e banco funcionando.
- Scripts SQL organizados e reutilizáveis.
- API testada e validada no Insomnia.
