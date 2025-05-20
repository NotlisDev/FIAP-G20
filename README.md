# TechChallenge FIAP - Sistema de Gerenciamento de Conteúdo Educacional

## Descrição

Sistema de gerenciamento de conteúdo educacional desenvolvido como parte do TechChallenge da FIAP. O projeto consiste em uma aplicação full-stack que permite o gerenciamento de usuários, posts e conteúdo educacional.

## Tecnologias Utilizadas

### Backend
* Node.js
* Express
* TypeScript
* MongoDB
* JWT para autenticação
* Bcrypt para hash de senhas

### Frontend
* React
* TypeScript
* Material-UI
* Axios
* React Router

### Infraestrutura
* Docker
* Docker Compose
* MongoDB

## Funcionalidades

### Autenticação e Autorização
* Login de usuários (admin, professor, aluno)
* Registro de novos usuários
* Controle de acesso baseado em papéis (RBAC)
* Validação de campos obrigatórios por papel

### Gerenciamento de Usuários
* Criação e edição de usuários
* Definição de papéis (admin, professor, aluno)
* Campo de disciplina obrigatório para professores
* Validação de campos por tipo de usuário

### Gerenciamento de Conteúdo
* Criação e edição de posts
* Visualização de posts
* Filtragem e ordenação de conteúdo
* Interface responsiva

## Estrutura do Projeto

```
techchallenge/
├── api/                    # Backend
│   ├── src/
│   │   ├── config/        # Configurações
│   │   ├── controllers/   # Controladores
│   │   ├── models/        # Modelos
│   │   ├── routes/        # Rotas
│   │   └── app.ts         # Aplicação principal
│   └── package.json
│
├── frontend/               # Frontend
│   ├── src/
│   │   ├── components/    # Componentes React
│   │   ├── services/      # Serviços (API)
│   │   └── App.tsx        # Aplicação principal
│   └── package.json
│
├── app/blog-dos-professores/
│   ├── app/               # Tela inicial com lista de posts
│   ├── components/        # Componentes de telas
│   ├── hooks/             # Hooks para autenticação e tema
│   ├── types/             # Interfaces para componentes
│   └── configurações      # Babel, TypeScript, etc.
│
├── docker-compose.yml      # Configuração Docker
└── README.md
```

## Requisitos do Sistema
* Docker
* Docker Compose
* Node.js (versão 14 ou superior)
* npm ou yarn

## Instalação e Execução

### Backend e Frontend principal

1. Clone o repositório:
```
git clone https://github.com/joandeitos/fiap-techchallenge.git
cd fiap-techchallenge
```

2. Inicie os containers:
```
docker-compose up -d
```

3. Acesse a aplicação:
   * Frontend: http://localhost:8080
   * Backend: http://localhost:4000/api-docs/

### App Blog dos Professores

1. Navegue até a pasta do app:
```
cd app/blog-dos-professores/
```

2. Instale as dependências e inicie:
```
npm install
npm start
```

## Usuários Iniciais

### Administrador
* Email: admin@system.com
* Senha: 123456

## Contribuição
1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Contato
* GitHub: [joandeitos](https://github.com/joandeitos)
* GitHub: [NotlisDev](https://github.com/NotlisDev)
