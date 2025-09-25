🎯 AI Career Coach Advisor

An AI-powered career guidance platform built with Next.js, TailwindCSS, Prisma, Gemini AI, and Shadcn UI.
This application helps users with interview preparation, career insights, resume & cover letter generation, and more — combining AI with structured user flows.

🚀 Features

🔐 User authentication and onboarding

📊 Weekly AI-generated career insights via Gemini AI & scheduled jobs (Inngest)

🎤 Mock Interview Mode

Generate domain-specific interview questions using AI

Track performance metrics and results

📄 Resume Builder

Build resume in Markdown

Export / download as PDF

📝 Cover Letter Generator using AI

📂 User dashboard to view & manage insights, interviews, resumes, etc.

🛠 Tech Stack

Frontend / Fullstack: Next.js (App Router)

UI & Styling: TailwindCSS, Shadcn UI

Database / ORM: Prisma + PostgreSQL

AI / NLP: Google Gemini API

Background / Serverless Jobs: Inngest (cron + async tasks)

Auth / Session: Clerk

Deployment (recommended): Vercel

📁 Project Structure
/app
 ├── (auth)/         # Login, Signup UI & pages
 ├── (dashboard)/    # User dashboard / core pages
 ├── api/            # API route handlers
 ├── components/     # Reusable UI components
 ├── hooks/          # Custom React hooks
 ├── lib/            # Configs: Prisma, AI, Inngest setup
 ├── prisma/         # Prisma schema / migrations
 └── public/         # Static assets

Other files:
- next.config.mjs
- tailwind.config.mjs
- middleware.js
- .env file (see Setup section)
- TypeScript / ESLint configs

⚙️ Setup & Installation

1️⃣ Clone the repository

git clone https://github.com/KakarlaRakeshNaidu/AI-Career-coach-Advisor.git
cd AI-Career-coach-Advisor


2️⃣ Install dependencies

npm install
# or yarn / pnpm


3️⃣ Configure environment variables
Create a .env file in the root directory. Example:

DATABASE_URL=your_postgres_database_url
NEXTAUTH_SECRET=your_nextauth_secret
GEMINI_API_KEY=your_gemini_api_key

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
CLERK_SECRET_KEY=your_clerk_secret
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding


➡️ Replace placeholders with your actual credentials.

4️⃣ Run the development server

npm run dev


Now open http://localhost:3000
 in your browser 🚀

📈 Future Enhancements

🎙 Voice-based mock interviews

📊 AI-driven progress tracking & personalized career roadmap

🌐 Multi-language / localization support

📱 Dedicated mobile app (React Native or Next.js mobile UI)

🔐 Further enhancements to auth & security

📜 License

MIT License © 2025
Feel free to use, modify, and contribute!
