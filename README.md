# 🍽️ Full Stack Food Delivery Website (PHP Project)

A complete **Food Delivery Website** built with **PHP (Backend)** and **React.js (Frontend)**, integrating **Stripe** for secure online payments.  
This project was developed as part of a full‑stack learning journey to understand the interaction between modern frontend frameworks and traditional backend technologies.

---

## 🚀 Features

### 👨‍💻 User Side
- 🍔 Browse menu and food categories  
- 🛒 Add to cart, edit quantity, and checkout  
- 💳 Online payment with Stripe integration  
- 🔐 User authentication (login/register)  
- 🧾 View order history and order details  
- 📱 Responsive design for mobile & desktop  

### 🧑‍💼 Admin Side
- 📦 Add / edit / delete food items  
- 📋 View orders and update status  
- 📈 Dashboard for overview of sales and activity  

---

## 🛠️ Tech Stack

| Category | Technology |
|-----------|-------------|
| **Frontend** | React.js, Axios, Bootstrap / CSS |
| **Backend** | PHP (Procedural + MySQLi) |
| **Database** | MySQL |
| **Payment** | Stripe API |
| **Hosting** | XAMPP / Apache / Localhost |
| **Version Control** | Git, GitHub |

---

## 📂 Project Structure

```
php-project/
├── backend/
│   ├── config/             # Database connection, constants
│   ├── api/                # PHP scripts for API endpoints
│   ├── uploads/            # Image uploads
│   └── index.php           # Entry point
│
├── frontend/
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Main pages (Home, Cart, etc.)
│   │   ├── App.js
│   │   └── index.js
│   └── public/
│
└── README.md
```

---

## ⚙️ Installation Guide

### 1️⃣ Clone the repository
```bash
git clone https://github.com/tam130103/php-project.git
cd php-project
```

### 2️⃣ Backend (PHP + MySQL)
1. Copy the `backend` folder to your **XAMPP/htdocs** directory  
2. Start **Apache** and **MySQL** from XAMPP Control Panel  
3. Import the database:
   - Open **phpMyAdmin**
   - Create a new database (e.g. `food_delivery`)
   - Import the `.sql` file from the project  
4. Update database credentials in `backend/config/db.php`:
```php
$host = 'localhost';
$user = 'root';
$pass = '';
$dbname = 'food_delivery';
```

---

### 3️⃣ Frontend (React)
```bash
cd frontend
npm install
npm start
```

---

### 4️⃣ Payment Configuration
1. Create a [Stripe](https://stripe.com) account  
2. Copy your **Publishable Key** and **Secret Key**  
3. Add them to `.env` file:
```
REACT_APP_STRIPE_KEY=your_publishable_key
STRIPE_SECRET_KEY=your_secret_key
```

---

## 🌐 Live Demo

🔗 **GitHub Repo:** [https://github.com/tam130103/php-project](https://github.com/tam130103/php-project)  
🔗 **Demo Website:** (Add your Render/Vercel link here)

---

## 🧠 Screenshots

| Homepage | Cart Page | Admin Dashboard |
|-----------|------------|----------------|
| ![Home](https://raw.githubusercontent.com/tam130103/php-project/main/images/home.png) | ![Cart](https://raw.githubusercontent.com/tam130103/php-project/main/images/cart.png) | ![Admin](https://raw.githubusercontent.com/tam130103/php-project/main/images/admin.png) |

---

## 📘 API Overview (PHP Backend)

| Method | Endpoint | Description |
|--------|-----------|-------------|
| `GET` | `/api/foods` | Fetch all food items |
| `POST` | `/api/order` | Place new order |
| `GET` | `/api/orders?user_id={id}` | Get user order history |
| `POST` | `/api/auth/register` | Register new user |
| `POST` | `/api/auth/login` | Login user |
| `POST` | `/api/payment` | Process Stripe payment |

---

## 💡 Future Improvements
- Add coupon system  
- Add food search and filtering  
- Implement order tracking status  
- Improve admin dashboard UI  
- Deploy both backend and frontend to cloud hosting  

---

## 👨‍💻 Author

**Nguyễn Tâm**  
📍 Hanoi, Vietnam  
💼 [GitHub](https://github.com/tam130103) | [Email](mailto:thetam2103@gmail.com)

---

## 📝 License
This project is licensed under the **MIT License** — feel free to use and modify for your own learning or projects.

---

⭐ *If you find this project helpful, please give it a star on GitHub!* ⭐
