

### 📄 **README.md**

````markdown
# 🌸 Flower Store App (Multi-Merchant E-Commerce)

A modern e-commerce backend for flower stores built with **NestJS**, **Prisma**, and **MySQL**.  
Supports multiple merchants, customers, product management, and secure ordering.

---

## 🧭 Overview

The Flower Store App is an online platform where:
- 🌼 **Customers** can browse and buy flowers.  
- 🛍️ **Merchants** can sell flowers and manage their inventory.  
- ⚙️ **Admins** can manage users, merchants, and analytics.

This backend uses **NestJS** for modular architecture, **Prisma ORM** for database modeling, and **MySQL** for data storage.

---

## 🧰 Tech Stack

| Layer | Technology |
|-------|-------------|
| **Backend** | [NestJS](https://nestjs.com/) |
| **Database** | [MySQL](https://www.mysql.com/) |
| **ORM** | [Prisma](https://www.prisma.io/) |
| **Authentication** | JWT + bcrypt |
| **Documentation** | Swagger (OpenAPI) |
| **Language** | TypeScript |

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/emangomaa/flower-store-app.git
cd flower-store-app
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Create a `.env` File in Project Root

Create a file named `.env` in the **same folder as** `package.json`, and add:

```env
DATABASE_URL="mysql://root:your_password@localhost:3306/flower_store"
JWT_SECRET="your_jwt_secret_key"
```

> ⚠️ Replace `your_password` and `your_jwt_secret_key` with your actual credentials.

---

## 🗄️ Database Setup (MySQL + Prisma)

### Initialize Prisma

```bash
npx prisma init
```

### Apply Schema & Create Tables

```bash
npx prisma migrate dev --name init_flower_store
```

### Generate Prisma Client

```bash
npx prisma generate
```

### Optional: Open Prisma Studio

```bash
npx prisma studio
```

(Launches a web UI to browse and edit your database.)

---

## 🚀 Running the Application

### Development

```bash
npm run start:dev
```

### Production

```bash
npm run build
npm run start:prod
```

The API will run at:
➡️ **[http://localhost:3000](http://localhost:3000)**

---

## 🧠 Features

### 👥 Users

* Register / Login
* Manage addresses and profiles
* Place and track orders
* Review purchased products

### 🛒 Merchants

* Register as merchants
* Add / Edit / Delete flower products
* Manage stock, prices, and orders

### 🧾 Admins

* Approve merchants
* Manage categories
* View analytics and reports

---

## 🧩 Example Folder Structure

```
src/
 ├── auth/
 ├── users/
 ├── merchants/
 ├── products/
 ├── orders/
 ├── payments/
 ├── reviews/
 ├── prisma/
 ├── main.ts
 └── app.module.ts
```

---

## 🧾 API Documentation

Swagger auto-generated docs available at:
👉 **[http://localhost:3000/api/docs](http://localhost:3000/api/docs)**

---

## 🧪 Testing

Run all tests:

```bash
npm run test
```

End-to-end tests:

```bash
npm run test:e2e
```

---

## 🧑‍💻 Contribution

1. Fork the repo
2. Create a feature branch:

   ```bash
   git checkout -b feature/my-feature
   ```
3. Commit changes:

   ```bash
   git commit -m "Add my feature"
   ```
4. Push and create a pull request 🚀

---

## 🛡️ License

This project is licensed under the **MIT License**.

---

## 💐 Author

**Your Name**
💻 GitHub: [@emangomaa](https://github.com/emangomaa)
📧 Email: [emangomaa149@gmail.com](mailto:emangomaa149@gmail.com)
