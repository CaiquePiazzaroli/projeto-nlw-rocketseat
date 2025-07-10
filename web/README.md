# NLW Project - Web

Este projeto é uma aplicação web desenvolvida com React, Vite e TypeScript, utilizando bibliotecas modernas para UI, roteamento e gerenciamento de estado.

## Principais Bibliotecas
- **React**: Biblioteca principal para construção da interface.
- **Vite**: Ferramenta de build e desenvolvimento rápido.
- **TypeScript**: Tipagem estática para JavaScript.
- **React Router DOM**: Gerenciamento de rotas.
- **@tanstack/react-query**: Gerenciamento de dados assíncronos e cache.
- **TailwindCSS**: Estilização utilitária.
- **@radix-ui/react-slot**: Composição de componentes UI.
- **class-variance-authority, clsx, tailwind-merge**: Utilitários para manipulação de classes CSS.
- **lucide-react**: Ícones SVG.

## Padrões de Projeto
- **Componentização**: Componentes reutilizáveis em `src/components`.
- **Hooks e Providers**: Uso de `QueryClientProvider` para contexto global de dados.
- **Aliases**: Importações simplificadas usando `@` para `src`.
- **Estilização utilitária**: TailwindCSS e helpers para classes dinâmicas.

## Setup e Configuração
1. **Pré-requisitos**: Node.js >= 18
2. **Instalação das dependências**:
   ```sh
   npm install
   ```
3. **Rodar em modo desenvolvimento**:
   ```sh
   npm run dev
   ```
4. **Build para produção**:
   ```sh
   npm run build
   ```
5. **Preview do build**:
   ```sh
   npm run preview
   ```

## Estrutura de Pastas
- `src/`: Código-fonte principal
  - `components/`: Componentes reutilizáveis
  - `lib/`: Utilitários
  - `pages/`: Páginas da aplicação
  - `app.tsx`: Configuração de rotas e providers

## Observações
- O projeto utiliza o padrão de importação por alias (`@/`) para facilitar o gerenciamento de caminhos.
- As configurações do TypeScript e Vite já estão otimizadas para desenvolvimento moderno.

---

Para dúvidas ou sugestões, consulte a documentação das bibliotecas utilizadas ou abra uma issue.
