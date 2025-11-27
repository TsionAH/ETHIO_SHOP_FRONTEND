# Ethio Shop Frontend (Updated with Payment Integration)

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
8. [Payment Gateway Integration](#payment-gateway-integration)
9. [Testing with Postman](#testing-with-postman)
10. [Screenshots](#screenshots)
11. [Future Improvements](#future-improvements)
12. [Contact](#contact)

---

## Project Overview

Ethio Shop is a full-stack e-commerce platform where users can browse products, add items to their cart, and complete purchases. This updated version includes **Chapa payment gateway integration** for secure and seamless online payments.

The frontend provides a responsive, user-friendly interface and interacts with backend APIs for products, cart, and payment processing.

---

## Features

- **Homepage:** Featured products, categories, and promotions.
- **User Authentication:** Sign up, login, logout.
- **Product Browsing:** Browse by category, search products.
- **Cart Management:** Add, remove, update items.
- **Checkout:** Integrated with **Chapa payment gateway** for secure payments.
- **Merchant Dashboard:** Merchants manage products, view orders.
- **Responsive Design:** Works on mobile, tablet, and desktop.

---

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript (React.js if used)
- **Payment Integration:** Chapa Payment Gateway
- **API Consumption:** Axios / Fetch
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
├── pages/               # Page components
└── assets/              # Images, icons, and other assets

```

---

## Installation and Setup

1. **Clone the repository**

```bash
git clone <FRONTEND_REPO_LINK>
```

2. **Navigate into the project folder**

```bash
cd ethio-shop-frontend
```

3. **Install dependencies**

```bash
npm install
```

4. **Run development server**

```bash
npm start
```

Access `http://localhost:3000` in your browser.

---

## Usage

- Open [Live Demo](https://ethio-shop-fulstack-3.onrender.com/)
- Navigate through homepage, product pages, and cart.
- Sign up / login to access checkout.
- **Checkout:** Click **Pay Now** → redirects to **Chapa payment gateway** → complete payment securely.

---

## API Integration

Frontend communicates with backend API for:

- Products: `GET /products`
- User Auth: `POST /auth/login`, `POST /auth/signup`
- Cart: `POST /cart`, `GET /cart`
- Checkout & Payment: `POST /checkout` → triggers **Chapa payment**

> Ensure the backend server is live to process payments and update orders.

---

## Payment Gateway Integration

**Chapa Integration Details:**

- Chapa provides secure online payments for Ethiopian users.
- On checkout, the frontend sends the total amount and user details to the backend.
- The backend creates a payment request with Chapa API and returns a payment link.
- Users are redirected to Chapa payment page to complete payment.
- After payment, Chapa redirects back to frontend with payment status.
- Successful payment updates the user order in the system.

**Steps to Test:**

1. Add items to cart.
2. Click **Pay Now** on checkout page.
3. Complete payment using Chapa sandbox/test mode or live credentials.
4. Confirm order status updates in the frontend.

---

## Testing with Postman

- Test backend endpoints with live URL.
- **Example:**

```json
POST /checkout
{
  "userId": "123",
  "cartItems": [...],
  "totalAmount": 500
}
```

- Response contains **Chapa payment link** for testing.

---

## Screenshots

_(Add screenshots of homepage, cart, checkout with Chapa button, and successful payment confirmation.)_

---

## Future Improvements

- Support multiple payment gateways (Paypal, Stripe).
- Email confirmation after successful payment.
- Enhanced UI/UX with animations.
- Order tracking for customers.

---

## Contact

- **Author:** Tsion Alemu Handiso
- **Email:** [Your Email Here]
- **GitHub:** [https://github.com/TsionAH](https://github.com/TsionAH)

---

**Notes for Mentor:**

- The frontend now supports **Chapa payment integration**.
- Backend must be live for payment to work.
- Users can test payments directly using sandbox/live Chapa credentials.
- Fully responsive, easy to navigate, and ready for demonstration.

---
