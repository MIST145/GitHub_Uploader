# GitHub_Uploader

🟩 GitHub Manager Electron

A Ponte Definitiva para um Workflow Git Simples, Intuitivo e Eficiente

<img src="https://upload.wikimedia.org/wikipedia/commons/d/d9/Node.js_logo.svg" width="90"/>GitHub Manager Electron é uma aplicação desktop moderna construída com Electron + React + TypeScript + Tailwind, criada para simplificar o gerenciamento de repositórios, operações Git e integração com a API do GitHub — tudo em uma interface rápida e elegante.


---

🚀 Visão Geral

A aplicação fornece um painel intuitivo que permite:

Visualizar repositórios do GitHub conectados

Executar operações Git essenciais

Gerenciar issues, commits e branches

Autenticar com GitHub OAuth

Navegar em elementos e dados com UI responsiva

Utilizar componentes modernos e reusáveis (shadcn/ui)


A missão: unificar o poder do GitHub + praticidade do desktop + fluidez do NodeJS.


---

🛠️ Tecnologias Principais

Tecnologia	Uso

Electron	Empacotamento desktop e ambiente de execução
React + TypeScript	Camada de UI moderna e tipada
Vite	Build ultrarrápido
TailwindCSS	Estilização eficiente e responsiva
shadcn/ui	Componentes prontos e acessíveis
GitHub REST API	Integração com dados reais
Node.js	Backbone dos scripts e comunicação nativa



---

📁 Estrutura do Projeto

git-hub-dashboard-main/
├── public/
├── src/
│   ├── components/
│   │   ├── ui/...
│   │   └── AppWidgets...
│   ├── hooks/
│   ├── lib/
│   │   ├── github.ts   ← núcleo da API GitHub
│   │   └── utils.ts
│   ├── pages/
│   │   ├── Index.tsx
│   │   └── NotFound.tsx
│   ├── App.tsx
│   └── main.tsx
├── tailwind.config.ts
├── tsconfig.json
└── vite.config.ts


---

🌉 Arquitetura da Aplicação

A aplicação segue uma arquitetura modular orientada a camadas:

1. UI Layer

Construída com React + Tailwind

Usa componentes reutilizáveis (botões, tooltips, inputs, toasts)

Navegação via React Router


2. Hooks Layer

use-mobile → gerenciamento responsivo

use-toast → sistema global de notificações


3. Lib Layer

O coração da integração com o GitHub:

github.ts:

Listar repositórios

Buscar commits

Criar/editar issues

Gerenciar branches

Autenticação OAuth/Token


utils.ts:

Funções auxiliares para formatação, validação, parsing etc.




---

🧩 Principais Funcionalidades

✔ Autenticação GitHub

Token do usuário

Armazenamento seguro

Requisições autenticadas


✔ Visualização de Repositórios

Forks

estrelas

branches

última atualização

commits recentes

tamanho e linguagem dominante


✔ Painel Inteligente

Navegação rápida entre repos

Ações Git essenciais (pull, push, fetch, commit)


✔ UI Dinâmica

Componentes modulares

Dark/Light-ready

Responsividade mobile/desktop



---

📦 Instalação

1️⃣ Instalar dependências

npm install
# ou
bun install

2️⃣ Rodar aplicação em modo dev

npm run dev

3️⃣ Build para produção

npm run build

4️⃣ Empacotar como aplicação desktop

(se aplicável caso exista script Electron configurado)

npm run electron:build


---

🔌 Integração com GitHub

O arquivo src/lib/github.ts contém todas as funções responsáveis pela comunicação:

getUserRepos()

getRepoCommits()

createIssue()

updateIssue()

getBranches()

getRepoDetails()


Cada função retorna dados prontos para renderização na UI.


---

📊 Documentação Extra

Além deste README, foram gerados materiais complementares:

📁 Estrutura completa da aplicação (Excel)
👉 app_structure.xlsx

📄 Documento de arquitetura da aplicação (PDF)
👉 app_architecture.pdf


---

🧪 Testes

Caso deseje implementar testes:

Jest + React Testing Library

Testes unitários dos hooks

Testes das funções da API GitHub



---

🎨 Preview (mock)

┌────────────────────────────────────────┐
│ Repo Name        ⭐120   🍴12          │
│ Branches: main/dev                     │
│ Último commit: 2h atrás                │
├────────────────────────────────────────┤
│ Issues abertas: 8                      │
│ Pull Requests: 3                       │
│ Ações Git: [PULL] [PUSH] [FETCH]       │
└────────────────────────────────────────┘


---

🤝 Contribuições

Contribuições são muito bem-vindas:

1. Fork o projeto


2. Crie uma branch (feature/nova-feature)


3. Faça commit


4. Abra um Pull Request




---

🧑‍💻 Autor

Mist

> “O GOAT da integração Git moderna.”




---

📄 Licença

Este projeto está sob licença MIT.
Use livremente, modifique e distribua
