
# AI Car Marketplace

## Overview

This project is an AI-powered car marketplace application, designed to provide a seamless experience for buying and selling cars. It leverages modern web technologies and AI capabilities to offer features such as car listings, search, user authentication, and potentially AI-driven recommendations or interactions.

## Features

- **Car Listings**: Browse and view details of available cars.
- **Search & Filtering**: Efficiently search for cars based on various criteria.
- **User Authentication**: Secure user login and registration powered by Clerk.
- **Admin Dashboard**: Manage car listings, user accounts, and other administrative tasks.

- **User Dashboard**: 
  - **Profile Management**: View and update user profile information.
  - **Car Listings**: see car listings (e.g., add, edit, delete).
  - **Test Drive Scheduling**: View and manage scheduled test drives.

- **Test Drive Scheduling**: Schedule and manage test drives.
- **AI Integration**: Utilizes Google Generative AI for enhanced functionalities (e.g., car descriptions, chatbot).
- **Responsive Design**: Built with Tailwind CSS for a modern and adaptive user interface.

## Tech Stack

- **Framework**: Next.js 15 (with Turbopack for fast development)
- **UI Library**: React 19
- **Styling**: Tailwind CSS
- **Authentication**: Clerk
- **ORM**: Prisma
- **Database**: PostgreSQL (managed via Supabase)
- **AI**: Google Generative AI
- **Database Migrations**: Prisma Migrate
- **Deployment**: Vercel (assumed, based on Next.js)

## Getting Started

Follow these instructions to set up and run the project locally.

### Prerequisites

- Node.js (v18 or higher)
- npm
- PostgreSQL database (local or remote, e.g., Supabase)

### Installation

1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd car_plaza
   ```

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

