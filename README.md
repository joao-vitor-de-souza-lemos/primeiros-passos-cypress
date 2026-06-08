# 🌐 Web Testing — OrangeHRM

> Automação de testes E2E para aplicação web utilizando Cypress, com cobertura de fluxos de autenticação e gerenciamento de usuários do sistema [OrangeHRM](https://opensource-demo.orangehrmlive.com).

---

## 📌 Sobre o Projeto

Este repositório contém uma suíte de testes automatizados E2E para o sistema de RH **OrangeHRM**, disponibilizado publicamente como ambiente de demonstração para fins educacionais em Quality Assurance.

O projeto é estruturado seguindo o padrão **Page Object Model (POM)**, separando a lógica de interação com a interface dos casos de teste, garantindo maior organização, manutenibilidade e reusabilidade do código. A biblioteca **Chance.js** é utilizada para geração de dados aleatórios nos testes de atualização de usuário.

---

## 🛠️ Tecnologias Utilizadas

- [Cypress](https://www.cypress.io/) — framework de automação de testes E2E
- [Chance.js](https://chancejs.com/) — geração de dados aleatórios para massa de testes
- JavaScript (CommonJS) — linguagem dos testes e configurações
- Git & GitHub — versionamento e hospedagem do projeto

---

## 📁 Estrutura do Projeto

```
primeiros-passos-cypress/
├── cypress/
│   ├── e2e/
│   │   ├── login.spec.cy.js       # Casos de teste de Login
│   │   └── user.spec.cy.js        # Casos de teste de Usuário
│   ├── fixtures/
│   │   └── users/
│   │       └── userData.json      # Massa de dados dos testes
│   ├── pages/
│   │   ├── loginPage.js           # Page Object da tela de Login
│   │   ├── dashboardPage.js       # Page Object da tela de Dashboard
│   │   ├── menuPage.js            # Page Object do Menu de navegação
│   │   └── myInfoPage.js          # Page Object da tela My Info
│   └── support/
│       ├── commands.js            # Comandos customizados do Cypress
│       └── e2e.js                 # Configuração global dos testes
├── .gitignore
├── cypress.config.js              # Configuração do Cypress
├── package.json                   # Dependências e scripts do projeto
└── README.md
```

---

## ✅ Casos de Teste Implementados

| Módulo    | Caso de Teste                  | Tipo     | Status           |
|-----------|-------------------------------|----------|------------------|
| Login     | Login com credenciais inválidas | Negativo | ✅ Implementado  |
| Login     | Login com credenciais válidas   | Positivo | ✅ Implementado  |
| My Info   | Atualização de dados do usuário | Positivo | ✅ Implementado  |

---

## 🌍 Aplicação Testada

- **Sistema:** OrangeHRM Live Demo
- **URL:** https://opensource-demo.orangehrmlive.com
- **Credenciais de acesso:** disponíveis publicamente na própria página de login do ambiente demo

---

## ⚙️ Pré-requisitos

- [Node.js](https://nodejs.org/) v18+

---

## 🚀 Como Executar

**1. Clone o repositório:**
```bash
git clone https://github.com/joao-vitor-de-souza-lemos/primeiros-passos-cypress.git
cd primeiros-passos-cypress
```

**2. Instale as dependências:**
```bash
npm install
```

**3. Abra o Cypress em modo interativo:**
```bash
npx cypress open
```

**Ou execute os testes em modo headless (terminal):**
```bash
npx cypress run
```

---

## 🗂️ Massa de Dados

Os dados utilizados nos testes estão centralizados em `cypress/fixtures/users/userData.json`, permitindo fácil manutenção sem alterar os arquivos de teste. Dados dinâmicos como nome e sobrenome são gerados aleatoriamente via **Chance.js** em tempo de execução.

---

## 👤 Autor

**João Vitor de Souza Lemos**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-joaolemos2004-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/joaolemos2004)
[![GitHub](https://img.shields.io/badge/GitHub-joao--vitor--de--souza--lemos-black?style=flat&logo=github)](https://github.com/joao-vitor-de-souza-lemos)
