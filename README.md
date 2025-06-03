# Login - auth
Estrutura de autenticação para o projeto **Login**.
## Atividade em grupo de até 3 integrantes.
- Clonar este repositório.
- Testar a api com **insomnia**.
- Estudar e documentar a estrutura do projeto.
- Detalhar e documentar as bibliotecas utilizadas.
- Documentar descrição do funcionamento utilizando **UML DA(Diagrama de Atividades)**.


# 📚 API de Gerenciamento de Alunos

Este projeto é uma API RESTful desenvolvida em Node.js para gerenciar o cadastro de alunos. Ela permite realizar operações de CRUD (Create, Read, Update, Delete) utilizando MongoDB como banco de dados.

## 📁 Estrutura do Projeto

<pre><code> ``` aula10/
├── controllers/
│ └── alunoController.js
├── models/
│ └── alunoModel.js
├── routes/
│ └── alunoRoutes.js
├── app.js
├── package.json
└── README.md ``` </code></pre>


- `controllers/`: Lógica das funcionalidades (criar, listar, editar, deletar alunos)
- `models/`: Modelos dos dados com Mongoose (definição de como o aluno é salvo)
- `routes/`: Endpoints da API
- `app.js`: Configuração do servidor e middlewares
- `package.json`: Dependências e scripts do projeto

---

## 📦 Bibliotecas Utilizadas

| Biblioteca     | Descrição |
|----------------|-----------|
| **express**    | Framework para criar rotas e middlewares no Node.js |
| **mongoose**   | ODM para MongoDB, facilita interação com banco de dados |
| **body-parser**| Middleware para ler o corpo das requisições HTTP |

---

## 🌐 Rotas da API

| Método | Rota             | Descrição                                 |
|--------|------------------|-------------------------------------------|
| GET    | `/alunos`        | Lista todos os alunos                     |
| GET    | `/alunos/:id`    | Busca um aluno específico por ID          |
| POST   | `/alunos`        | Cria um novo aluno                        |
| PUT    | `/alunos/:id`    | Atualiza os dados de um aluno             |
| DELETE | `/alunos/:id`    | Remove um aluno do banco de dados         |

---

## 🔄 Diagrama de Atividades (UML)

Abaixo está o Diagrama de Atividades que representa o funcionamento da API:

![Diagrama de Atividades - API Alunos](./caminho/para/imagem.png) <!-- Substitua esse caminho após a geração da imagem -->

---

## 🚀 Como executar

```bash
# Instalar dependências
npm install

# Iniciar o servidor
node app.js


