# 🌐 Plataforma Freelancer - Open Source

Este é um projeto open source de uma plataforma para freelancers, construído com tecnologias modernas e pronto para colaboração da comunidade dev!

---

## 🚀 Tecnologias

- **Frontend:** Next.js + Tailwind CSS
- **Backend:** Node.js + Express + Prisma
- **Banco de Dados:** PostgreSQL
- **Deploy:** Vercel (frontend) + Render (backend)
- **CI/CD:** GitHub Actions

---

## 💻 Como rodar localmente

### 1. Clonar o repositório

```bash
git clone https://github.com/SidneRezende/freelance-platform.git
cd freelance-platform
```

### 2. Backend

```bash
cd backend
npm install
cp .env.example .env
npx prisma migrate dev --name init
node index.js
```

### 3. Frontend

```bash
cd ../frontend
npm install
cp .env.local.example .env.local
npm run dev
```

---

## 🌐 Deploy

### Backend (Render)

- Crie um novo serviço web no [Render](https://render.com/)
- Configure:
  - **Build command:** `npm install`
  - **Start command:** `node index.js`
  - **Root directory:** `backend`
  - Adicione as variáveis do `.env`

### Frontend (Vercel)

- Importe o projeto no [Vercel](https://vercel.com/)
- Configure a env var:
  - `NEXT_PUBLIC_API_URL` → URL do backend na Render
- Diretório: `frontend`

---

## 🤝 Contribuições

Contribuições são super bem-vindas! Veja a aba de Issues para sugestões e tarefas abertas.  
Use `npm run dev` para rodar o projeto local e explore os arquivos em `frontend` e `backend`.

---

## 📂 Estrutura do Projeto

```
freelance-platform/
├── backend/              # API com Express + Prisma
│   └── ...
├── frontend/             # App com Next.js + Tailwind
│   └── ...
└── .github/workflows/    # CI/CD com GitHub Actions
```

---

## 🛠 Funcionalidades previstas

- [ ] Autenticação com JWT
- [ ] Cadastro de projetos
- [ ] Propostas de freelancers
- [ ] Sistema de avaliações
- [ ] Dashboard de contratantes e freelancers
- [ ] Sistema de pagamento (mock ou real)

---

## 📬 Contato

Quer participar? Crie uma Issue ou mande uma mensagem!  
Vamos construir juntos 💙
