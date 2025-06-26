### **NestJS Boilerplate with Auth, Stripe, and Prisma**

```
<p align="center">
  <a href="https://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

<p align="center">
  <b>A modern NestJS boilerplate with Authentication, Stripe, and Prisma ORM</b>
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@nestjs/core" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
  <a href="https://www.npmjs.com/package/@nestjs/core" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="License" /></a>
  <a href="https://www.npmjs.com/package/@nestjs/core" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/core.svg" alt="Downloads" /></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow" /></a>
</p>
```

---

And here’s how you'd start the **Installation** section properly:

````
## 📦 Installation

```
$ yarn install
````

> Copy the `.env.example` file to `.env` and configure your environment variables.

---

## 🔧 Configuration

Environment variables (example):

```env
DATABASE_URL="postgresql://user:password@localhost:5432/mydb"
JWT_SECRET="your_jwt_secret"
STRIPE_SECRET_KEY="sk_test_..."
STRIPE_WEBHOOK_SECRET="whsec_..."
```

---

## 🏃 Running the app

```bash
# development
$ yarn start

# watch mode
$ yarn start:dev

# production
$ yarn start:prod
```

---

## ✅ Test

```bash
# unit tests
$ yarn test

# e2e tests
$ yarn test:e2e

# test coverage
$ yarn test:cov
```

---

## 🗂 Project Structure (Brief)

```
src/
├── auth/               # JWT Auth, strategies, guards
├── user/               # User module
├── stripe/             # Stripe module for payments & webhooks
├── prisma/             # PrismaService and seed logic
├── app.module.ts       # Main app module
├── main.ts             # Entry point
```

---

## 🧱 Prisma

Generate Prisma client after modifying `prisma/schema.prisma`:

```bash
$ npx prisma generate
```

Run migrations:

```bash
$ npx prisma migrate dev --name init
```

---

## 🧾 Stripe Webhooks

To test webhooks locally, use:

```bash
$ stripe listen --forward-to localhost:3000/stripe/webhook
```

---

## 📄 License

Nest is [MIT licensed](LICENSE).

---

## 🏁 Getting Started

Clone the repo:

```bash
git clone https://github.com/your-org/nestjs-boilerplate.git
cd nestjs-boilerplate
yarn install
```

Then set up your `.env`, database, and run:

```bash
yarn start:dev
```

```

---

Let me know if you also want an actual starter GitHub repo layout or `.env.example` content scaffold.
```
