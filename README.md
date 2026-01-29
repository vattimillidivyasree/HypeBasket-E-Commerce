# 🛒 HypeBasket – Full Stack E-Commerce Website
<br/>
HypeBasket is a full-stack MERN e-commerce web application designed to deliver a seamless online shopping experience through a modern, fast, and responsive user interface. Built using React.js, Node.js, Express.js, and MongoDB, the platform supports complete e-commerce functionality including product browsing, cart management, and secure checkout.
The application integrates Stripe and Razorpay payment gateways to enable safe and reliable online transactions. HypeBasket is inspired by modern e-commerce platforms in both design and usability and aims to provide a scalable and production-ready shopping solution.
<br/>

## 🌐 VIDEO DEMOLINK ON INTEGRATED TERMINAL:<br/>
https://your-video-link-here
<br/>

## 🚀 Features

<br/>
• Secure user authentication and authorization
<br/>
• Product listing with detailed product views
<br/>
• Shopping cart management (add, remove, update items)
<br/>
• Secure online payments using Stripe and Razorpay
<br/>
• Order placement and order history tracking
<br/>
• Admin panel for product and order management
<br/>
• Responsive and user-friendly shopping interface
<br/>
• Scalable RESTful API backend built with Node.js and Express
<br/>


## 🛠 Tech Stack
<br/>
Frontend: React.js (Vite), JavaScript (JSX), Tailwind CSS
<br/>
Backend: Node.js, Express.js
<br/>
Database: MongoDB (Mongoose)
<br/>
Authentication: JWT-based authentication
<br/>
Payments: Stripe & Razorpay (secure online payments)
<br/>
Media Storage: Cloudinary (image upload & management)
<br/>
Architecture: RESTful APIs
<br/>

## ⚙️ Installation & Setup
```bash
git clone https://github.com/vattimillidivyasree/HypeBasket-full-stack.git
cd HypeBasket-full-stack
```

## 🔐 Environment Variables (Backend)
```bash
JWT_SECRET="HypeBasket"
ADMIN_EMAIL="admin@example.com"
ADMIN_PASSWORD="HypeBasket123"

MONGODB_URI="-------- Paste Your Mongo URI Here --------"

CLOUDINARY_API_KEY="-------- Paste Cloudinary API key --------"
CLOUDINARY_SECRET_KEY="-------- Paste Cloudinary SECRET key --------"
CLOUDINARY_NAME="-------- Paste Cloudinary cloud name --------"

STRIPE_SECRET_KEY="-------- Paste Stripe Secret key --------"

RAZORPAY_KEY_SECRET="-------- Paste Razorpay Secret key --------"
RAZORPAY_KEY_ID="-------- Paste Razorpay key Id --------"
```

## 🔐 Environment Variables (Frontend)
```bash
VITE_BACKEND_URL="http://localhost:4000"
VITE_RAZORPAY_KEY_ID="-------- Paste Razorpay key Id --------"
```

## 🔐 Environment Variables (Admin)
```bash
VITE_BACKEND_URL="http://localhost:4000"
```

## ▶️ Run the Application

```bash
cd backend
npm install
npm run server
```

```bash
cd frontend
npm install
npm run dev
```

```bash
cd admin
npm install
npm run dev
```

## 📋 Prerequisites <br/><br/>

• Node.js (v18 or higher recommended) <br/>
• npm or yarn package manager <br/>
• MongoDB (local or MongoDB Atlas) <br/>
• Stripe account for payments <br/>
• Razorpay account for payments <br/>
• Cloudinary account for media storage <br/>
• Modern web browser (Chrome / Edge / Firefox) <br/>

## 📦 Dependencies <br/><br/>

### 🎨 Frontend <br/>

- `axios` : `^1.7.4` <br/>
- `react` : `^18.3.1` <br/>
- `react-dom` : `^18.3.1` <br/>
- `react-router-dom` : `^6.26.1` <br/>
- `react-toastify` : `^10.0.5` <br/>

### 🎛️ Admin Panel <br/>

- `axios` : `^1.7.4` <br/>
- `react` : `^18.3.1` <br/>
- `react-dom` : `^18.3.1` <br/>
- `react-router-dom` : `^6.26.1` <br/>
- `react-toastify` : `^10.0.5` <br/>

### ⚙️ Backend <br/>

- `bcrypt` : `^5.1.1` <br/>
- `cloudinary` : `^2.4.0` <br/>
- `cors` : `^2.8.5` <br/>
- `dotenv` : `^16.4.5` <br/>
- `express` : `^4.19.2` <br/>
- `jsonwebtoken` : `^9.0.2` <br/>
- `mongoose` : `^8.5.3` <br/>
- `multer` : `^1.4.5-lts.1` <br/>
- `razorpay` : `^2.9.4` <br/>
- `stripe` : `^16.8.0` <br/>
- `validator` : `^13.12.0` <br/>

### 🛠️ Development Tools <br/>

- `vite` : `^7.3.1` <br/>
- `tailwindcss` : `^3.4.10` <br/>
- `postcss` : `^8.4.41` <br/>
- `autoprefixer` : `^10.4.20` <br/>
- `eslint` : `^8.57.0` <br/>
- `eslint-plugin-react` : `^7.35.0` <br/>
- `eslint-plugin-react-hooks` : `^4.6.2` <br/>
- `eslint-plugin-react-refresh` : `^0.4.9` <br/>
- `@vitejs/plugin-react` : `^4.3.1` <br/>
- `@types/react` : `^18.3.3` <br/>
- `@types/react-dom` : `^18.3.0` <br/>
- `nodemon` : `^3.1.4` <br/>

## 🔄 Application Flow <br/><br/>

1. User Registration & Login <br/>
Users can register and log in securely using JWT-based authentication <br/><br/>

2. Product Browsing <br/>
Users browse products by categories, view product details, prices, and images <br/><br/>

3. Cart Management <br/>
Users can add products to cart, update quantities, or remove items before checkout <br/><br/>

4. Order Placement & Payment <br/>
Users place orders using secure payment gateways like Stripe and Razorpay <br/><br/>

5. Order Confirmation <br/>
After successful payment, users receive order confirmation and order details <br/><br/>

6. Admin Product Management <br/>
Admins can add, update, and delete products using the admin dashboard <br/><br/>

7. Order Management <br/>
Admins manage user orders, update order status, and track payments <br/><br/>


## 🔌 API Endpoints <br/><br/>

###  Authentication <br/>
Authentication is handled using JWT (JSON Web Tokens). <br/>
Admin authentication is managed separately for secure access. <br/><br/>

###  Products <br/>
- GET `/api/product/list` – Get all products <br/>
- GET `/api/product/single/:id` – Get product details <br/>
- POST `/api/product/add` – Add a new product (Admin) <br/>
- PUT `/api/product/update/:id` – Update product details (Admin) <br/>
- DELETE `/api/product/remove/:id` – Delete a product (Admin) <br/><br/>

###  Cart <br/>
- POST `/api/cart/add` – Add product to cart <br/>
- POST `/api/cart/remove` – Remove product from cart <br/>
- GET `/api/cart/get` – Get user cart items <br/><br/>

###  Orders <br/>
- POST `/api/order/place` – Place an order <br/>
- GET `/api/order/userorders` – Get user order history <br/>
- GET `/api/order/list` – Get all orders (Admin) <br/>
- PUT `/api/order/status` – Update order status (Admin) <br/><br/>

###  Payments <br/>
- POST `/api/payment/stripe` – Stripe payment processing <br/>
- POST `/api/payment/razorpay` – Razorpay payment processing <br/><br/>


## 🧪 Testing <br/><br/>

- Test user authentication (login & logout) <br/>
- Verify product listing and product detail pages <br/>
- Test cart functionality (add, update, remove items) <br/>
- Test Stripe and Razorpay payments using test keys <br/>
- Verify order placement and order history <br/>
- Test admin functionalities (add/update/delete products) <br/>
- Check protected routes for admin access <br/>
- Validate API responses using Postman <br/>

## 🛠️ Troubleshooting <br/><br/>

### Server Issues <br/>
- Ensure `MONGODB_URI` is correctly set in the backend `.env` file <br/>
- Check if the backend server port is already in use <br/>
- Restart the server after updating environment variables <br/><br/>

### Authentication Issues <br/>
- Verify `JWT_SECRET` is properly configured <br/>
- Ensure admin email and password are correct in `.env` <br/>
- Clear browser cookies or local storage if login issues persist <br/><br/>

### Payment Issues <br/>
- Use Stripe and Razorpay test keys for development <br/>
- Verify payment keys are correctly added to `.env` files <br/>
- Check payment callback and webhook configurations <br/><br/>

### Image Upload Issues <br/>
- Verify Cloudinary API credentials in `.env` <br/>
- Ensure supported image formats are being uploaded <br/><br/>

### Frontend / Admin Issues <br/>
- Run `npm install` before starting frontend or admin servers <br/>
- Ensure backend server is running before accessing frontend or admin panel <br/>
- Check API base URL in frontend and admin `.env` files <br/>


## 📈 Future Enhancements <br/><br/>

• Wishlist functionality for users <br/>
• Product reviews and ratings <br/>
• Order tracking with real-time status updates <br/>
• Discount coupons and promotional offers <br/>
• Advanced admin analytics and sales reports <br/>
• Multi-vendor marketplace support <br/>
• Improved performance and scalability <br/>

## 📄  License <br/><br/>
This project is licensed under the MIT License. <br/><br/>

## 🤝 Contributing <br/><br/>

Contributions are currently not accepted for this project. <br/>
This repository is maintained as a completed full-stack project for learning and portfolio purposes. <br/>

## 🙏 Acknowledgements <br/><br/>

- Clerk for authentication and user management <br/>
- Stripe for secure payment processing <br/>
- MongoDB for database services <br/>
- Cloudinary for media storage <br/>
- React & Node.js open-source community <br/>


# React + Vite <br/><br/>

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.<br/>

Currently, two official plugins are available:<br/>

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh<br/>
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh<br/>
