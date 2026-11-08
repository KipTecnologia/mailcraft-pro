# ✉️ MailCraft Pro v2.0

[![Next.js 15](https://img.shields.io/badge/Next.js-15.0_App_Router-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Prisma ORM](https://img.shields.io/badge/Prisma-ORM-2D3748?style=for-the-badge&logo=prisma)](https://prisma.io)
[![Resend](https://img.shields.io/badge/Resend-Email_API-black?style=for-the-badge&logo=resend)](https://resend.com)
[![Stripe](https://img.shields.io/badge/Stripe-Checkout_&_Webhooks-635BFF?style=for-the-badge&logo=stripe)](https://stripe.com)
[![Bilingual i18n](https://img.shields.io/badge/i18n-English_%26_Português-10B981?style=for-the-badge)](https://kiptecnologia.github.io/mailcraft-pro/)
[![By Kip Tecnologia](https://img.shields.io/badge/By-Kip_Tecnologia-059669?style=for-the-badge)](https://github.com/KipTecnologia)
[![Live Demo](https://img.shields.io/badge/Live-Demo_Ready-emerald?style=for-the-badge&logo=googlechrome)](https://kiptecnologia.github.io/mailcraft-pro/)

> **English**: Turnkey **React Email Luxury Transactional Studio & Micro-SaaS Boilerplate**. Built with **Next.js 15 App Router**, **TypeScript**, **Prisma ORM**, **Resend Email API Dispatcher**, **Pre-inlined HTML Compilation**, and **Stripe Subscriptions**.  
> **Português**: Estúdio profissional de **E-mails Transacionais de Luxo com React Email**. Equipado com **Next.js 15**, **Prisma ORM**, **Disparador Real via API Resend**, **HTML Pré-inlinado** e **Stripe**. Engineered by **[Kip Tecnologia](https://github.com/KipTecnologia)**.

---

## ⚡ Live Interactive Demo (Bilingual EN / PT)

Experience the live Light Editorial Studio, real-time preview, and live email dispatcher with 1-click English 🇺🇸 / Portuguese 🇧🇷 switcher:  
👉 **[https://kiptecnologia.github.io/mailcraft-pro/](https://kiptecnologia.github.io/mailcraft-pro/)**

- **🎨 Light Editorial Studio Aesthetic**: Warm stone palette (`#FAF9F6`), delicate borders, and fluid natural full-page desktop scrolling.
- **✉️ Live Resend API Integration**: Test dispatch transactional emails directly to your Gmail/inbox in seconds.
- **📱 Responsive Mobile & Desktop Simulator**: Instant viewport toggle with zero layout shift.
- **📋 Dual Export Engine**: Pre-inlined production HTML and reusable React Email components (`@react-email/components`).

---

## 🏗️ Production Micro-SaaS Architecture

```
mailcraft-pro/
├── prisma/
│   └── schema.prisma                # User, EmailProject, EmailTemplate & EmailDispatchLog
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── email/
│   │   │   │   └── send-test/route.ts   # Resend API email dispatch endpoint
│   │   │   └── stripe/
│   │   │       ├── checkout/route.ts    # Stripe Checkout session creator
│   │   │       └── webhook/route.ts     # Automated plan upgrade webhook
│   │   ├── globals.css                  # Light editorial studio styling
│   │   ├── layout.tsx                   # SEO & Root Layout
│   │   └── page.tsx                     # Interactive transactional email studio
│   ├── lib/
│   │   ├── db.ts                        # Prisma client singleton
│   │   ├── email/
│   │   │   └── sender.ts                # Resend REST client with simulated fallback
│   │   └── stripe.ts                    # Stripe plans & billing config
│   └── types/
├── .env.example                         # Documented environment variables
├── package.json
└── README.md
```

---

## 💰 Built-in Monetization & Business Model

MailCraft Pro includes a turnkey software licensing and recurring revenue structure:

| Plan | Price (Global) | Price (Brazil) | Features |
| :--- | :---: | :---: | :--- |
| **Starter Preview** | $0 | R$ 0 | 3 essential templates, HTML export, responsive preview |
| **Developer Pro** | $19 / mo | R$ 89 / mês | 15+ Luxury Transactional Templates, unlimited test sends, React Email & HTML export |
| **Agency Studio** | $79 once | R$ 349 único | Unlimited client projects, complete TypeScript source code, lifetime updates |

---

## 🚀 Quick Start Guide (English)

### 1. Clone & Install
```bash
git clone https://github.com/KipTecnologia/mailcraft-pro.git
cd mailcraft-pro
npm install
```

### 2. Configure Environment Variables
```bash
cp .env.example .env
```
Add your keys:
- `DATABASE_URL`: Defaults to local SQLite (`file:./dev.db`) for instant local run.
- `RESEND_API_KEY`: From [resend.com](https://resend.com) for live email dispatches.
- `STRIPE_SECRET_KEY`: For monetization checkout.

### 3. Initialize Database & Run
```bash
npx prisma db push
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) to view the studio.

---

## 🇧🇷 Guia de Início Rápido (Português)

### 1. Instalação e Execução
```bash
git clone https://github.com/KipTecnologia/mailcraft-pro.git
cd mailcraft-pro
npm install
cp .env.example .env
npx prisma db push
npm run dev
```

### 2. Envio de E-mails com Resend
Basta criar uma chave de API gratuita no [resend.com](https://resend.com), inserir no arquivo `.env` e disparar e-mails para qualquer endereço através da rota `/api/email/send-test`.

---

## 🏢 About Kip Tecnologia

**MailCraft Pro** is engineered and maintained by **Kip Tecnologia**.

- **Website**: [kiptecnologia.com.br](https://kiptecnologia.com.br)
- **GitHub**: [github.com/KipTecnologia](https://github.com/KipTecnologia)
- **Support**: `contato@kiptecnologia.com.br`

---

## 💎 Commercial Licensing vs. Public Demo

| Feature / Asset | Public Interactive Demo (Free) | Commercial License & Full Boilerplate (Paid) |
| :--- | :---: | :---: |
| **Interactive Light Editorial Studio** | ✅ Free Access | ✅ Included |
| **Bilingual Switcher (EN / PT)** | ✅ Included | ✅ Included |
| **Real-Time Variables & Mobile Simulator** | ✅ Included | ✅ Included |
| **Next.js 15 App Router Full Source** | ❌ (Commercial) | ✅ **100% Unlocked** |
| **Prisma ORM & SQLite/PostgreSQL Database** | ❌ (Commercial) | ✅ **Production Models** |
| **Resend API Real Email Dispatch Endpoint** | ❌ (Commercial) | ✅ **Production Endpoints** |
| **15+ Luxury React Email Templates (@react-email)** | ❌ (Commercial) | ✅ **Pre-inlined HTML & TSX** |
| **Stripe Checkout & Automated Webhooks** | ❌ (Commercial) | ✅ **Turnkey Setup** |
| **100% White-Label Rights (Agency & SaaS Use)** | ❌ (Evaluation only) | ✅ **Full Commercial Rights** |
| **Lifetime Updates & Discord VIP Access** | ❌ (Evaluation only) | ✅ **Included** |

👉 **[Acquire Commercial License & Full Boilerplate on Gumroad](https://rancharia.gumroad.com)**

---

## 📄 License

This repository is governed by the **Kip Tecnologia Commercial & Evaluation License (v2.0)**. The interactive demo and public assets are available for evaluation purposes. Commercial reproduction, distribution, and SaaS operation require a valid Commercial License from Kip Tecnologia. Copyright (c) 2026 Kip Tecnologia.
