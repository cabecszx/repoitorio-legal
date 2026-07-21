# Music Catalog Site

Aplicação web completa para catálogo de músicas com autenticação, busca, paginação e redirecionamento para YouTube.

## Stack

- Front-end: React + Vite
- Back-end: Node.js + Express
- Autenticação: JWT + bcrypt

## Requisitos

- Node.js 18+
- npm

## Como rodar localmente no VS Code

1. Abra o terminal na pasta do projeto.
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Inicie a aplicação em modo de desenvolvimento:
   ```bash
   npm run dev
   ```
4. Abra o front-end em `http://localhost:5173` e o back-end em `http://localhost:3000`.

## Credenciais padrão de administrador

- Usuário: `admin123`
- Senha: `77312476d`

## Funcionalidades

- Catálogo com categorias: Gospel, Sertanejo, Funk, Forró, Rock, MPB, Clássicas, Pop e Hip-Hop.
- Busca em tempo real por título, artista ou categoria.
- Paginação com conjunto de 24 itens por página.
- Registro e login com validação de usuário/e-mail duplicados.
- Redirecionamento para o YouTube ao clicar em um card.

## Publicar no GitHub

1. Crie um repositório vazio no GitHub.
2. No terminal do VS Code, rode:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin <URL_DO_REPO>
   git push -u origin main
   ```

## Observação de escala

Para um catálogo de 100.000 músicas, o modelo ideal é migrar o catálogo para um banco como PostgreSQL/Supabase ou MongoDB e aplicar paginação/virtualização no front-end.
