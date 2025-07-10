# NLW Project - Server

## Tecnologias e Bibliotecas Utilizadas

- **Node.js**: Ambiente de execução JavaScript.
- **TypeScript**: Tipagem estática para JavaScript.
- **Fastify**: Framework web rápido e eficiente.
- **@fastify/cors**: Middleware para habilitar CORS.
- **drizzle-orm**: ORM para integração com banco de dados PostgreSQL.
- **drizzle-kit**: Ferramenta para migrações e gerenciamento de banco de dados.
- **postgres**: Cliente PostgreSQL para Node.js.
- **zod**: Validação de esquemas e variáveis de ambiente.
- **fastify-type-provider-zod**: Integração do Zod com Fastify.

## Padrões de Projeto

- **Modularização**: Separação de responsabilidades em arquivos e pastas (ex: rotas, conexão, schema).
- **Validação de ambiente**: Uso do Zod para garantir variáveis de ambiente válidas.
- **Type Provider**: Uso de Zod como type provider no Fastify para validação e serialização.

## Setup e Configuração

1. **Instalação das dependências**
   ```bash
   npm install
   ```

2. **Configuração do ambiente**
   - Crie um arquivo `.env` na raiz do projeto com as variáveis:
     ```env
     PORT=3333
     DATABASE_URL=postgresql://usuario:senha@host:porta/database
     ```

3. **Migrações do banco de dados**
   - Configure e execute as migrações usando o Drizzle Kit:
     ```bash
     npx drizzle-kit migrate
     ```

4. **Seed do banco de dados**
   ```bash
   npm run db:seed
   ```

5. **Rodar o servidor**
   - Ambiente de desenvolvimento:
     ```bash
     npm run dev
     ```
   - Ambiente de produção:
     ```bash
     npm start
     ```

## Endpoints

- `GET /health` - Verifica se o servidor está online.
- `GET /rooms` - Lista as salas cadastradas.

---
