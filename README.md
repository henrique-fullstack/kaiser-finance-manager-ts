<h1 align="center">Kaiser Finance Manager (TypeScript Edition)</h1>

## 📖 About the project (Sobre o Projeto)

This project is a CLI personal finance management application built with **TypeScript**, **Node.js**, and **SQLite**. Designed as a backend engineering portfolio project, it applies a modular architecture inspired by **Nest.js**, utilizing strict typing, Generic Repository patterns (`<T>`), segregated service layers, data integrity, and user authentication.

Este projeto é uma aplicação CLI para gerenciamento de finanças pessoais construída com **TypeScript**, **Node.js** e **SQLite**. Desenvolvido como projeto de portfólio para engenharia de software backend, aplica uma arquitetura modular inspirada no **Nest.js**, utilizando tipagem estrita, padrão Generic Repository (`<T>`), camadas de serviços isoladas, integridade de dados e autenticação de usuários.

---

## 🚀 Features (Funcionalidades)

### English
* **User Authentication:** Secure registration and login flow using SQLite persistence.
* **Category Management:** Full CRUD operations for custom transaction categories (Incomes/Expenses).
* **Transaction Management:** Complete financial logging tied specifically to each user account.
* **Financial Summaries:** Real-time general and monthly financial summary calculations.
* **Formatted CLI Interface:** Terminal output structured with clean tables and visual feedback (`src/cli/formatters`).
* **Automated Database Setup:** Automatic schema initialization on first startup.

### Português
* **Autenticação de Usuários:** Fluxo seguro de registro e login com persistência no SQLite.
* **Gerenciamento de Categorias:** Operações CRUD completas para categorias de transação personalizadas (Receitas/Despesas).
* **Gerenciamento de Transações:** Registro financeiro completo associado individualmente a cada conta de usuário.
* **Resumos Financeiros:** Cálculos em tempo real de saldo geral e relatórios mensais.
* **Interface CLI Formatada:** Saída no terminal estruturada com tabelas limpas e feedbacks visuais (`src/cli/formatters`).
* **Inicialização Automática:** Criação automática de tabelas e do banco de dados no primeiro uso.

---

## 🏗️ Architecture & Best Practices (Arquitetura e Boas Práticas)

* **Modular Domain Architecture:** Business domains isolated into dedicated modules (`src/modules/`), following Nest.js design patterns.
* **Generic Repository Pattern:** Decoupled data access layer leveraging TypeScript Generics (`src/database/base.repository.ts`).
* **CLI Layer Separation:** Command handlers and terminal formatters completely decoupled from core business logic (`src/cli/`).
* **Strict TypeScript & Clean Code:** Strict type checking (`strict: true`) and clean naming conventions across all entities and services.
* **Automated Testing:** Unit and integration test suite using `Vitest` / `Jest` (`tests/`).

```text
kaiser-finance-manager/
├── src/
│   ├── cli/                        # CLI Interface (Commands & Formatters)
│   ├── modules/                    # Business Domains (Transactions, Categories, Users)
│   ├── database/                   # SQLite Connection & Generic Base Repository <T>
│   └── main.ts                     # CLI Application Entry Point
├── tests/                          # Unit and Integration Tests
├── package.json
└── tsconfig.json
```

---

## 🛠️ Technologies (Tecnologias)

<div align="left">
  <img src="https://skillicons.dev/icons?i=ts" height="60" alt="typescript logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=nodejs" height="60" alt="nodejs logo" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sqlite/sqlite-original.svg" height="60" alt="sqlite logo" />
</div>

---

## ⚙️ How to run (Como Rodar)

### English
1. **Clone the repository:**
   ```bash
   git clone https://github.com/henrique-fullstack/Kaiser-finance-manager.git
   ```
2. **Navigate to the folder:**
   ```bash
   cd Kaiser-finance-manager
   ```
3. **Install dependencies:**
   ```bash
   npm install
   ```
4. **Run the application (Development mode):**
   ```bash
   npm run dev
   ```
5. **Build and run for production:**
   ```bash
   npm run build
   npm start
   ```
> **Note:** The system will automatically create the SQLite database file (`kaiser_finance_manager.db`) on its first execution.

### Português
1. **Clone o repositório:**
   ```bash
   git clone https://github.com/henrique-fullstack/Kaiser-finance-manager.git
   ```
2. **Navegue até a pasta:**
   ```bash
   cd Kaiser-finance-manager
   ```
3. **Instale as dependências:**
   ```bash
   npm install
   ```
4. **Rode a aplicação (Modo de desenvolvimento):**
   ```bash
   npm run dev
   ```
5. **Compile e rode em produção:**
   ```bash
   npm run build
   npm start
   ```
> **Nota:** O sistema criará automaticamente o arquivo de banco de dados SQLite (`kaiser_finance_manager.db`) na primeira execução.