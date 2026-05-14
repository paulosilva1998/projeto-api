# 🚀 Projeto API - Gestão de Usuários

Este projeto é uma API RESTful desenvolvida em **Node.js** para a gestão de usuários, utilizando uma **Arquitetura em Camadas (MSC)** para garantir um código limpo, escalável e de fácil manutenção.

## 📋 Sobre o Projeto
A aplicação permite o gerenciamento completo (CRUD) de usuários em um banco de dados MySQL, aplicando regras de negócio como validação de e-mail e prevenção de duplicidade.

## 🏗️ Arquitetura MSC
O projeto segue o padrão de separação de responsabilidades:
- **Model**: Responsável pela interação direta com o banco de dados MySQL.
- **Service**: Onde residem as regras de negócio e validações.
- **Controller**: Gerencia as requisições HTTP e envia as respostas ao cliente.

## 🛠️ Tecnologias Utilizadas
*   **Node.js** & **Express**
*   **MySQL** (Driver `mysql2/promise`)
*   **Dotenv** (Gerenciamento de variáveis de ambiente)
*   **Cors** & **Helmet** (Segurança)
*   **Nodemon** (Ambiente de desenvolvimento)

## 📂 Estrutura de Pastas
```text
src/
 ├── config/      # Conexão com o banco de dados
 ├── controllers/ # Camada de controle (HTTP)
 ├── database/    # Scripts SQL (DDL e DML)
 ├── middlewares/ # Tratamento de erros e interceptores
 ├── models/      # Camada de dados (Queries SQL)
 ├── routes/      # Definição das rotas da API
 ├── services/    # Regras de negócio e validações
 ├── utils/       # Funções auxiliares (Regex, etc.)
 └── app.js       # Configuração da aplicação Express