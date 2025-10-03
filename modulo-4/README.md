# 📑 Módulo 4: **API RESTful do SGSA**

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge Aulas](https://img.shields.io/badge/Aulas-16-blue)
![Badge Node.js](https://img.shields.io/badge/Node.js-20.x-brightgreen)
![Badge Express](https://img.shields.io/badge/Express.js-4.x-lightgrey)
![Badge MySQL](https://img.shields.io/badge/MySQL-8.0-blue)

---

## 📖 Sobre o Módulo

Este módulo tem como objetivo construir a **API RESTful do SGSA (Sistema de Gerenciamento de Sala de Aula)** utilizando **Node.js, Express e MySQL**.  

Ao final, o aluno terá desenvolvido uma **API completa e documentada**, com autenticação básica, CRUDs conectados ao banco de dados, boas práticas de versionamento, testes e documentação via **Swagger**.

---

## 🔹 Aulas

### Aula 1 — Métodos HTTP e Boas Práticas

- Revisão dos métodos HTTP (GET, POST, PUT, DELETE).  
- Convenções REST.  
- Estrutura de endpoints para o SGSA.  

### Aula 2 — Endpoints Básicos

- Criação de rotas organizadas no Express.  
- Rotas de teste para health-check.  

### Aula 3 — Middlewares Essenciais

- Uso de `express.json()`.  
- Tratamento de erros e logs.  

### Aula 4 — CRUD Conectado ao MySQL

- Implementação de CRUD de **Alunos**.  
- Uso de `mysql2` e queries parametrizadas.  

### Aula 5 — CRUD de Turmas

- Endpoints de Turmas.  
- Relacionamento Aluno ↔ Turma.  

### Aula 6 — CRUD de Professores

- Endpoints de Professores.  
- Relacionamento Professor ↔ Turma.  

### Aula 7 — Testes de API com Insomnia/Postman

- Estrutura de collection de testes.  
- Testes de CRUDs implementados.  

### Aula 8 — Autenticação Simples

- Rota de login (usuário/senha).  
- Sessão básica com token JWT.  

### Aula 9 — Rotas Protegidas

- Middleware de autenticação.  
- Proteção de rotas sensíveis.  

### Aula 10 — Relacionamentos na API

- Endpoint de listagem Alunos por Turma.  
- Endpoint de listagem Aulas por Turma.  

### Aula 11 — Paginação e Filtros

- Paginação em rotas de listagem.  
- Parâmetros de busca e ordenação.  

### Aula 12 — Upload e Download de Arquivos

- Implementação com `multer`.  
- Upload de arquivos vinculados a tarefas.  
- Download simples de relatórios.  

### Aula 13 — Documentação com Swagger

- Instalação e configuração do Swagger.  
- Definição de endpoints com exemplos.  

### Aula 14 — Testes Automatizados

- Introdução ao Jest/Mocha.  
- Testes unitários simples de rotas.  

### Aula 15 — Mini-Projeto API SGSA

- Implementação de rotas completas:  
  - Alunos, Turmas, Professores, Aulas, Ocorrências, Tarefas.  
- Testes de integração.  

### Aula 16 — Revisão e Ajustes

- Revisão da API final.  
- Checklist de boas práticas.  
- Preparação para consumo no frontend.  

---

## 📅 Cronograma — Módulo 4 (API RESTful | 16 aulas)

| Aula | Tema / Foco           | Objetivos de Aprendizagem             | Conteúdos & Componentes              | Prática em Sala                       | Entregáveis          |
| ---- | --------------------- | ------------------------------------- | ------------------------------------ | ------------------------------------- | -------------------- |
| 1    | Métodos HTTP          | Compreender convenções REST           | GET, POST, PUT, DELETE, status codes | Criar rotas de exemplo                | Rotas REST básicas   |
| 2    | Endpoints básicos     | Criar endpoints organizados           | Express Router, health-check         | `/status` e `/hello`                  | Rotas teste          |
| 3    | Middlewares           | Aplicar middlewares essenciais        | express.json, error handler          | Middleware global                     | Middleware aplicado  |
| 4    | CRUD Alunos           | Criar CRUD completo em MySQL          | mysql2, queries preparadas           | Rotas de Alunos                       | CRUD Alunos          |
| 5    | CRUD Turmas           | CRUD com relacionamentos              | FK Aluno-Turma                       | Rotas de Turmas                       | CRUD Turmas          |
| 6    | CRUD Professores      | CRUD Professores + vínculo com Turmas | Tabelas relacionadas                 | Rotas de Professores                  | CRUD Professores     |
| 7    | Testes de API         | Validar endpoints                     | Insomnia/Postman                     | Collection de testes                  | Arquivo .json export |
| 8    | Autenticação          | Criar login simples com JWT           | bcrypt, jwt-simple                   | Rota `/login`                         | Login funcional      |
| 9    | Rotas protegidas      | Proteger endpoints com middleware     | Token JWT, authorization header      | Proteção em CRUD Turmas               | Rotas seguras        |
| 10   | Relacionamentos       | Implementar endpoints relacionados    | JOINs no MySQL                       | Alunos por Turma                      | Rotas relacionadas   |
| 11   | Paginação e filtros   | Melhorar consultas                    | LIMIT, OFFSET, parâmetros query      | Listagem com paginação                | Rotas com filtros    |
| 12   | Upload/Download       | Gerenciar arquivos                    | multer, res.download                 | Upload de tarefa + download relatório | Upload/download ok   |
| 13   | Documentação Swagger  | Documentar API                        | Swagger UI, OpenAPI 3                | Documentar Alunos/Turmas              | Swagger rodando      |
| 14   | Testes automatizados  | Criar testes de rotas                 | Jest/Mocha                           | Testes unitários CRUD Alunos          | Testes passando      |
| 15   | Mini-projeto API SGSA | Consolidar rotas SGSA                 | CRUDs + autenticação                 | Integração de todos os módulos        | API consolidada      |
| 16   | Revisão final         | Refinar API para entrega              | Ajustes finais, boas práticas        | Testes cruzados                       | API finalizada       |

---

## 📂 Estrutura de pastas (organização sugerida)

```plaintext
sgsa-api/
  src/
    config/db.js
    controllers/
    models/
    routes/
    middlewares/
    docs/ (swagger.yaml)
    tests/
  uploads/
  app.js
  package.json
  README.md
```

------

## ✅ Checklist de QA (usar ao final de cada aula)

**Funcionalidade**

- CRUDs funcionando com MySQL.
- Autenticação por JWT operando.
- Upload e download de arquivos funcionando.

**Boas práticas**

- Uso de status codes corretos.
- Middlewares aplicados (erros, logs, autenticação).
- Documentação atualizada no Swagger.

**Testes**

- Testes manuais (Insomnia/Postman).
- Testes automatizados básicos passando.

**Integração**

- API pronta para consumo pelo frontend.
- Endpoints consistentes e versionados (`/api/v1`).

------

## 📌 Entrega final do Módulo 4

- **API RESTful completa** do SGSA.
- CRUDs funcionando (Alunos, Turmas, Professores, Tarefas, Ocorrências, Aulas).
- Autenticação JWT implementada.
- Upload/download de arquivos funcionando.
- Documentação Swagger publicada.
- Testes básicos executados com Jest/Postman.

------

## 🔗 Próximos Passos

No **Módulo 5**, será feita a **Integração Frontend + Backend**, consumindo a API REST criada aqui para gerar telas dinâmicas e interativas do SGSA.

------

## 🎯 Critérios de Avaliação

Os alunos serão avaliados pelos seguintes critérios:

- CRUDs completos funcionando no MySQL.
- Autenticação implementada corretamente.
- Upload/download de arquivos operacionais.
- Documentação Swagger atualizada.
- API testada com Insomnia/Postman e Jest.
