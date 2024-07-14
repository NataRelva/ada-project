# Documentação Inicial do Ambiente de Desenvolvimento

## Estrutura do Projeto

```plaintext
packages/
├── contexts/
│   ├── scraping/
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   └── services/
│   │   ├── usecases/
│   │   ├── interfaces/
│   │   │   ├── controllers/
│   │   │   └── gateways/
│   │   ├── infrastructure/
│   │   └── docs/
│   ├── event_management/
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   └── services/
│   │   ├── usecases/
│   │   ├── interfaces/
│   │   │   ├── controllers/
│   │   │   └── gateways/
│   │   ├── infrastructure/
│   │   └── docs/
│   ├── data_processing/
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   └── services/
│   │   ├── usecases/
│   │   ├── interfaces/
│   │   │   ├── controllers/
│   │   │   └── gateways/
│   │   ├── infrastructure/
│   │   └── docs/
│   └── query/
│       ├── domain/
│       │   ├── entities/
│       │   └── services/
│       ├── usecases/
│       ├── interfaces/
│       │   ├── controllers/
│       │   └── gateways/
│       ├── infrastructure/
│       └── docs/
├── shared/
│   ├── domain/
│   └── infrastructure/
├── docs/
├── main.ts
└── serverless.yml

```
