# Ethio Shop Frontend

**Project Name:** Ethio Shop  
**Live Demo:** [Ethio Shop Frontend](https://ethio-shop-fulstack-3.onrender.com/)  
**Author:** Tsion Alemu Handiso  
**Date:** November 27, 2025

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Project Structure](#project-structure)
5. [Installation and Setup](#installation-and-setup)
6. [Usage](#usage)
7. [API Integration](#api-integration)
8. [Testing with Postman](#testing-with-postman)
9. [Screenshots](#screenshots)
10. [Future Improvements](#future-improvements)
11. [Contact](#contact)

---

## Project Overview

Ethio Shop is a full-stack e-commerce platform where users can browse products, add items to their cart, and complete purchases. This repository contains the **frontend** part of the project, which is fully integrated with the backend APIs hosted on Render.

The frontend is built with modern web technologies to provide a clean, responsive, and user-friendly interface.

---

## Features

- **Homepage:** Displays featured products, categories, and promotions.
- **User Authentication:** Sign up, login, and logout functionality.
- **Product Browsing:** Browse products by category with search functionality.
- **Cart Management:** Add, remove, and update items in the shopping cart.
- **Merchant Dashboard:** Merchants can manage products, view orders, and update inventory.
- **Checkout:** Simple and intuitive checkout process with “Pay Now” button.
- **Responsive Design:** Works seamlessly on mobile, tablet, and desktop devices.

---

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Frameworks/Libraries:** React.js (if used)
- **API Consumption:** Axios or Fetch for HTTP requests to backend
- **Deployment:** Render

---

## Project Structure

```

ethio-shop-frontend/
│
├── index.html           # Main HTML file
├── css/                 # Stylesheets
│   └── styles.css
├── js/                  # JavaScript files
│   └── main.js
├── components/          # Reusable UI components
├── pages/               # Individual page components
└── assets/              # Images, icons, and other assets

```

---

## Installation and Setup

If someone wants to run the frontend locally:

1. **Clone the repository**

```bash
git clone [<FRONTEND_REPO_LINK>](https://github.com/TsionAH/ETHIO_SHOP_FRONTEND)
```

2. **Navigate into the project folder**

```bash
cd ethio-shop
```

3. **Install dependencies** (if using npm)

```bash
npm install
```

4. **Run the development server**

```bash
npm start
```

The project should now be running on `http://localhost:3000`.

---

## Usage

- Open the [Live Demo](https://ethio-shop-fulstack-3.onrender.com/) in any modern browser.
- Use the navigation bar to access different pages.
- Sign up or login to access personalized features.
- Browse products and add items to the cart.
- Go to the checkout page and click the **Pay Now** button to simulate purchases.

---

## API Integration

This frontend communicates with the backend via API endpoints. Ensure the backend is live to fully test all functionalities.

**Example endpoints (from backend):**

- `GET /products` → Fetch all products
- `POST /auth/login` → User login
- `POST /auth/signup` → User registration
- `POST /cart` → Add item to cart
- `GET /cart` → Fetch user cart items

> Note: Replace the backend URL in your frontend API calls with the live Render link if testing live.

---

## Testing with Postman

1. Open [Postman](https://www.postman.com/).
2. Use the live backend URL [(provided separately)](https://backend-capstone1-9.onrender.com/ ) to test endpoints.
3. Make requests like GET, POST, PUT, DELETE to verify frontend-backend integration.
4. Examples:

   - **Login:** `POST /auth/login` with JSON `{ "email": "user@example.com", "password": "password" }`
   - **Fetch Products:** `GET /products`

---

## Screenshots

_(Add screenshots of the homepage, cart, product page, merchant dashboard, checkout page here for better clarity)_

---

## Future Improvements

- Add **payment gateway integration** (Stripe, PayPal, etc.)
- Enhance **UI/UX** with animations and better responsiveness
- Add **user reviews and ratings** for products
- Implement **order tracking** for customers
- Optimize performance for mobile devices

---

## Contact

- **Author:** Tsion Alemu Handiso
- **GitHub:** [https://github.com/TsionAH](https://github.com/TsionAH)

---

**Notes for Mentor:**

- Frontend is fully functional and deployed on Render.
- Backend API link should be connected for testing full features.
- All pages are responsive and can be tested on Postman and browser directly.

---
