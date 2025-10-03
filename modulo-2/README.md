# 📑 Módulo 2: **Backend SGSA com Node.js e Express**

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge Aulas](https://img.shields.io/badge/Aulas-8-blue)
![Badge Node.js](https://img.shields.io/badge/Node.js-20.x-brightgreen)
![Badge Express](https://img.shields.io/badge/Express.js-4.x-lightgrey)

---

## 📖 Sobre o Módulo

Este módulo tem como objetivo introduzir o **Backend do SGSA (Sistema de Gerenciamento de Sala de Aula)** utilizando **Node.js** e o framework **Express.js**.  

Ao final, o aluno terá construído uma **API inicial** com rotas básicas, manipulação de dados locais em JSON e estrutura organizada em **MVC**, preparando o terreno para a integração com o **MySQL no Módulo 3**.

---

## 🔹 Aulas

### Aula 1 — Introdução ao Node.js e NPM

- Conceitos de Node.js (runtime JS no servidor).  
- Uso do **NPM** para gerenciamento de pacotes.  
- Primeiro script com Node.js.  

### Aula 2 — Criando um Servidor com HTTP Nativo

- Módulo **http** do Node.js.  
- Resposta simples (Hello World).  
- Diferenças entre servidor nativo e Express.  

### Aula 3 — Introdução ao Express.js

- Instalação do **Express**.  
- Criação de rotas básicas (GET/POST).  
- Servindo respostas em JSON.  

### Aula 4 — Estrutura MVC no Projeto

- Organização do código em **Models, Views e Controllers**.  
- Separação de responsabilidades.  
- Implementação de rotas controladas.  

### Aula 5 — Manipulação de Dados com JSON

- CRUD simples utilizando arquivo `.json` como base de dados.  
- Leitura e escrita de arquivos no Node.js (`fs`).  
- Estrutura de endpoints para cadastro/listagem.  

### Aula 6 — Middlewares no Express

- Conceito de **middlewares**.  
- Aplicação prática: logger, parser de JSON, tratamento de erros.  

### Aula 7 — Upload e Manipulação de Arquivos

- Upload de arquivos com **multer**.  
- Salvando dados e referências no backend.  
- Preparação para uso futuro no SGSA (tarefas/relatórios).  

### Aula 8 — Mini-Projeto Backend

- Criação de uma API fake para o SGSA com rotas de:  
  - Login (simples, sem criptografia).  
  - Alunos e Turmas (CRUD básico em JSON).  
- Estrutura pronta para evoluir no **Módulo 3 (MySQL)**.  

---

## 📅 Cronograma — Módulo 2 (Backend SGSA | 8 aulas)

| Aula | Foco / Tema          | Objetivos de Aprendizagem              | Conteúdos & Componentes               | Prática em Sala                                 | Entregáveis               |
| ---- | -------------------- | -------------------------------------- | ------------------------------------- | ----------------------------------------------- | ------------------------- |
| 1    | Node.js + NPM        | Entender Node.js e usar pacotes NPM    | Runtime JS, NPM init, scripts         | Criar projeto inicial com `npm init`            | Estrutura Node.js básica  |
| 2    | Servidor HTTP nativo | Criar servidor básico em Node          | Módulo http, request/response         | Servidor Hello World                            | `server.js` simples       |
| 3    | Express.js básico    | Criar rotas GET/POST                   | Express, JSON, status codes           | API com rotas iniciais                          | `app.js` com rotas        |
| 4    | Estrutura MVC        | Organizar projeto em camadas           | Controllers, Models, Routes           | Reestruturar API para MVC                       | Estrutura MVC funcional   |
| 5    | CRUD com JSON local  | Manipular dados persistidos em arquivo | Módulo fs, JSON.parse/stringify       | CRUD de alunos/turmas em arquivo JSON           | `alunos.json`, rotas CRUD |
| 6    | Middlewares          | Aplicar camadas de tratamento          | Logger, JSON parser, error handler    | Middleware de log e tratamento de erro          | Middleware funcionando    |
| 7    | Upload de arquivos   | Gerenciar upload no backend            | Multer, validações básicas            | Upload de arquivos teste (tarefas)              | Rota de upload            |
| 8    | Mini-projeto backend | Consolidar aprendizados em API inicial | CRUD + login fake + rotas organizadas | Implementar API do SGSA (login, alunos, turmas) | API inicial SGSA          |

---

## 📂 Estrutura de pastas (organização sugerida)

```plaintext
sgsa-backend/
  src/
    controllers/
    models/
    routes/
    middlewares/
  data/
    alunos.json
    turmas.json
  uploads/
  app.js
  package.json
  README.md
```

------

## ✅ Checklist de QA (usar ao final de cada aula)

**Estrutura e Organização**

- Projeto organizado em MVC.
- Pastas e arquivos nomeados de forma consistente.

**Funcionalidade**

- Rotas GET/POST funcionando.
- CRUD básico operando em JSON.
- Upload de arquivos aceito.

**Boas práticas**

- Uso de `status codes` corretos.
- Middlewares aplicados para logs e erros.
- Código comentado de forma clara.

**Preparação para Integração**

- Dados prontos para migrar para MySQL no próximo módulo.
- Rotas estruturadas pensando em consumo pelo frontend.

------

## 📌 Entrega final do Módulo 2

- **API inicial em Node.js + Express** com CRUD básico e login fake.
- Estrutura organizada em **MVC**.
- Dados persistidos em arquivos JSON.
- Upload de arquivos funcionando.
- Documentação simples das rotas (em README ou Insomnia export).

------

## 🔗 Próximos Passos

No **Módulo 3**, será feita a **integração com MySQL**, substituindo o armazenamento em JSON por um banco de dados relacional e expandindo o CRUD do SGSA.

------

## 🎯 Critérios de Avaliação

Os alunos serão avaliados pelos seguintes critérios:

- Estrutura correta do projeto (MVC).
- Rotas funcionando com CRUD básico.
- Middlewares aplicados corretamente.
- API publicada/local testada com Insomnia.
- Documentação mínima das rotas.