# Projeto Carros Pedro

Plataforma de vendas de carros com backend em NestJS, banco PostgreSQL, ORM Prisma, autenticação via JWT e controle de acesso por perfis (roles).

## Como rodar

1. Acesse a pasta `backend/`
2. Crie um arquivo `.env` com:
```
DATABASE_URL="postgresql://postgres:postgres@localhost:5432/carros"
JWT_SECRET="segredo-supersecreto"
```
3. Rode os comandos:
```bash
npm install
npx prisma migrate dev --name init
npm run start:dev
```

## Estrutura
- Módulos: `usuarios`, `lojas`, `carros`, `pedidos`, `comissoes`, `vendedores`
- Autenticação com JWT
- Roles: `ADMIN`, `VENDEDOR`, `CLIENTE`