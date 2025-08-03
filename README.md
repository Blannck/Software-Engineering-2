This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

# Project Setup Guide

Follow these steps to set up your environment for development:

---

## 1. Install Dependencies

### ✅ Download Node.js  
Go to [NodeJS.org](https://nodejs.org) and install the latest stable version.

---

## 2. Create Accounts

### 🔷 Prisma  
Create an account on [Prisma](https://www.prisma.io/).

### 🟢 MongoDB  
1. Sign up at [MongoDB.com](https://www.mongodb.com/).
2. Create a new **Project**.
3. Assign your **username** and **password** for the database.

### 🔐 Create an account on [Clerk.com](https://clerk.com)  
1. Create a new application  
2. Locate your **Publishable Key** and **Secret Key**

---

## 3. Configure Environment Variables

### 🛠 Create a `.env` file in your project root and add:

- ``DATABASE_URL="mongodb+srv://username:password@cluster0.dbgobil.mongodb.net/db_name?retryWrites=true&w=majority"``


Replace:
- `username` with the MongoDB username you set
- `password` with the MongoDB password you set
- `db_name` with your database name

---

 - ``NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_publishable_key``
 - ``CLERK_SECRET_KEY=your_secret_key``

Replace:
- `your_publishable_key` with your Publishable Key
- `your_secret_key` with your Secret Key


---

## 5. Install Project Dependencies

```bash
npm install next react react-dom

npm install @clerk/nextjs

npm install mongodb

npx prisma generate

npx prisma db push

⚠️ If prompted for an update, run:

npm i --save-dev prisma@latest 
npm i @prisma/client@latest

Run the development server:

npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
