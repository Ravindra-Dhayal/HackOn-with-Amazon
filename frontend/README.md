# HackOn with Amazon Frontend

This frontend powers the Amazon-style shopping experience for the HackOn project. It includes the storefront, cart flow, payment selection, budget planner, and embedded analytics dashboard.

## What this app does

- Renders the product catalog and shopping cart
- Calculates cart totals and proceeds to checkout
- Recommends a payment method based on backend ML prediction
- Supports budget setup and monitoring for user spending limits
- Displays an embedded Power BI dashboard for insights

## Architecture

The frontend is a React + Vite application with route-based screens:

- `/` — product shop page
- `/cart` — cart and total summary
- `/pay` — payment method selection and checkout
- `/dashboard` — embedded analytics dashboard
- `/Budget` — personal budget planner

## Tech stack

- React
- Vite
- React Router
- Tailwind CSS
- Axios for API calls
- Power BI embed client

## Local setup

```bash
cd frontend
npm install
npm run dev
```

## Key project files

- [src/App.jsx](src/App.jsx) — route configuration
- [src/pages/shop/shop.jsx](src/pages/shop/shop.jsx) — product listing
- [src/pages/cart/cart.jsx](src/pages/cart/cart.jsx) — cart and subtotal logic
- [src/components/Payment.jsx](src/components/Payment.jsx) — payment recommendation and checkout flow
- [src/pages/Budget/budget.jsx](src/pages/Budget/budget.jsx) — budget tracking UI
- [src/pages/dashboard/dashboard.jsx](src/pages/dashboard/dashboard.jsx) — Power BI dashboard embed

## Problem solved

The application addresses the gap between shopping and financial awareness. Instead of making a payment decision blindly, users get a more informed checkout flow backed by historical payment success patterns, offers, and budget controls.
