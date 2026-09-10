# Projeto CRM
esse projeto tem como objetivo criar um CRM útil para a octobit jr, voltado para melhoria dos processos e aumento de produtividade devido a organização

## Objetivo
criar uma interface que opere no modelo kanban e que todos os membros cormercial tenham acesso, o modelo seria parecido com o que temos hoje no notion

## Linguagens utilizadas
Ecossistema Javascript com react, node e typescript:

**Frontend**

React
Vite
TypeScript
TanStack Query
React Router
Zustand
Tailwind
shadcn/ui
dnd-kit para Kanban

**Backend**

Node
Express
TypeScript
Prisma
Zod
Socket.IO
JWT/session baseado no OAuth

**Banco**

PostgreSQL

## Do que vai ser feito
Para um CRM da Octobit, o núcleo deve ser:

Lead → Oportunidade → Cliente → Projeto

E o Kanban representaria principalmente o pipeline comercial:

Novo Lead
   ↓
Contato realizado
   ↓
Reunião agendada
   ↓
Proposta enviada
   ↓
Negociação
   ↓
Fechado — Ganho
   ↓
Fechado — Perdido

Cada card poderia conter:

Empresa
Contato
Responsável
Valor estimado
Etapa
Data do próximo contato
Origem do lead
Tags
Observações
Atividades

Estrutura de pastas do projeto:
octobit-crm/
│
├── apps/
│   ├── web/          # React + Vite
│ 
│   └── api/          # Node + Express
│
├── packages/
│   ├── database/     # Prisma
│   ├── types/        # tipos compartilhados
│   ├── validation/   # Zod
│   └── config/
│
├── docker-compose.yml
├── package.json
└── README.md