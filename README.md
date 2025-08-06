# 🚗 AI Car Marketplace

An AI-powered web application that provides a seamless platform to **buy and sell cars**. Leveraging modern web technologies and AI integration, it offers intuitive features like car listings, advanced search, user dashboards, and smart AI interactions.

---

## 📌 Overview

AI Car Marketplace is built with a modern full-stack architecture using **Next.js**, **Tailwind CSS**, **Prisma**, and **Google Generative AI**. It provides both buyers and sellers with a responsive, secure, and smart car marketplace experience.

---

## ✨ Features

- **🔍 Car Listings** – Browse and view available cars with rich detail.
- **⚙️ Search & Filtering** – Quickly find cars by brand, model, price, and more.
- **🔐 Authentication** – Secure sign-in & sign-up using [Clerk](https://clerk.dev).
- **👤 User Dashboard**
  - Manage profile
  - Add/Edit/Delete car listings
  - Schedule test drives
- **📊 Admin Dashboard** – Manage users, listings, and platform data.
- **📅 Test Drive Scheduling** – Book and manage test drives seamlessly.
- **🤖 AI Integration**
  - Auto-generate car descriptions
  - Integrated AI chatbot
- **📱 Responsive Design** – Optimized for all devices using Tailwind CSS.

---

## 🛠 Tech Stack

| Category          | Technology               |
|------------------|---------------------------|
| **Framework**     | [Next.js 15](https://nextjs.org) (Turbopack) |
| **Frontend**      | [React 19](https://reactjs.org) |
| **Styling**       | [Tailwind CSS](https://tailwindcss.com) |
| **Authentication**| [Clerk](https://clerk.dev) |
| **Database**      | [PostgreSQL](https://www.postgresql.org) via [Supabase](https://supabase.com) |
| **ORM**           | [Prisma](https://www.prisma.io) |
| **AI**            | [Google Generative AI](https://ai.google/discover/generative-ai/) |
| **Deployment**    | [Vercel](https://vercel.com) |
| **Migrations**    | Prisma Migrate            |

---

## 🚀 Getting Started

### ✅ Prerequisites

- Node.js v18 or higher
- npm
- PostgreSQL database (e.g., [Supabase](https://supabase.com))

---

### 📦 Installation

```bash
# Clone the repo
git clone <your-repository-url>
cd car_plaza

# Install dependencies
npm install --legacy-peer-deps

2. Install dependencies:
   ```bash
   npm install --legacy-peer-deps
   ```

### Environment Variables

Create a `.env` file in the root of the project and add the following environment variables:

DATABASE_URL=
DIRECT_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=

ARCJET_KEY=


NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

### Database Migrations

Apply Prisma migrations to set up your database schema:

```bash
npx prisma migrate dev --name init
```

### Running the Development Server

Start the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Project Structure

    car_plaza/
    ├── prisma/
    ├── public/
    ├── app/
    ├── components/
    ├── lib/
    ├── styles/
    ├── .env
    ├── .env.test
    ├── .gitignore
    ├── next.config.js
    ├── package.json
    ├── postcss.config.js
    ├── tailwind.config.js
    └── tsconfig.json
