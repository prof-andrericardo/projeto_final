# 📚 SGSA – Sistema de Gerenciamento de Sala de Aula

![Badge Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Badge License](https://img.shields.io/badge/License-MIT-green)
![Badge Node](https://img.shields.io/badge/Node.js-20.x-brightgreen)
![Badge MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![Badge Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-purple)

---

## 📖 Sobre o Projeto

Este repositório contém o **projeto final integrador** do curso Técnico em Informática.  
O **SGSA (Sistema de Gerenciamento de Sala de Aula)** foi idealizado como uma aplicação **Fullstack** para apoiar o trabalho de **professores, secretaria e coordenação**.  

### 🎯 Objetivos principais
- ✅ Registrar aulas, conteúdos e frequência.  
- ✅ Cadastrar tarefas e ocorrências em sala de aula.  
- ✅ Gerar relatórios básicos de turmas e alunos.  

---

## 🛠️ Tecnologias Utilizadas

**Frontend**  
- HTML5  
- CSS3  
- Bootstrap 5.3  
- JavaScript (ES6+)  

**Backend**  
- Node.js (Express.js)  
- API RESTful  

**Banco de Dados**  
- MySQL 8.0  

**Ferramentas de Apoio**  
- GitHub / GitHub Pages  
- VSCode  
- Insomnia (testes de API)  

---

## 📂 Estrutura Inicial de Pastas

```plaintext
projeto_final/
│── frontend/         # Interface do usuário (HTML, CSS, JS, Bootstrap)
│── backend/          # Servidor Node.js + API REST
│── database/         # Scripts SQL (criação e carga inicial)
│── docs/             # Documentação do projeto
│── README.md         # Documentação principal
````

---

## 🚀 Como Executar o Projeto

### 🔹 Pré-requisitos

* Node.js (versão 18 ou superior)
* MySQL 8.0 instalado e configurado

### 🔹 Passos iniciais

```bash
# Clone este repositório
git clone https://github.com/prof-andrericardo/projeto_final.git

# Acesse a pasta do projeto
cd projeto_final

# Instale as dependências do backend
cd backend
npm install

# Crie o banco de dados (script em /database)
mysql -u root -p < database/schema.sql

# Inicie o servidor
npm start
```

---

## 📊 Funcionalidades (MVP)

* Login simples (professor, secretaria, coordenação).
* Cadastro de turmas, alunos e professores.
* Registro de aulas e chamadas (presença/falta).
* Cadastro de tarefas e ocorrências.
* Relatórios básicos por turma/aluno.

---

## 👥 Autores

* **Professor André Ricardo da Silva** – Orientador
* **Turma 3ºC Técnico em Informática – Colégio Victorino**

---

## 📜 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
