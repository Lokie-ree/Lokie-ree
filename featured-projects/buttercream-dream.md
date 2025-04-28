# E-Commerce Development Journey

## Project Overview

**Goal**:
To build a fully functional e-commerce website with a dynamic shopping cart, a streamlined checkout process, using Stripe, and CMS for easy product management.

**Tech Stack**

- **Frontend**: Next.js, React
- **Backend**: Node.js, API Routes
- **Libraries**: DaisyUi, Tailwind CSS
- **Payment Gateway**: Stripe
- **CMS**: Sanity
- **Hosting**: Vercel

---

## Table of Contents

- [E-Commerce Development Journey](#e-commerce-development-journey)
  - [Project Overview](#project-overview)
  - [Table of Contents](#table-of-contents)
  - [Development Journey](#development-journey)
    - [Phase 1: Initial Setup and Planning](#phase-1-initial-setup-and-planning)
    - [Phase 2: Main Pages and Reusuable Components](#phase-2-main-pages-and-reusuable-components)
      - [Navbar](#navbar)
      - [Shop Page](#shop-page)
      - [Product Detail Page](#product-detail-page)
      - [Cart Page](#cart-page)
      - [Checkout Page](#checkout-page)
      - [About Page](#about-page)
    - [Phase 3: Sanity Integration and Product Fetching](#phase-3-sanity-integration-and-product-fetching)
    - [Phase 4: Stripe Integration and Testing](#phase-4-stripe-integration-and-testing)
    - [Phase 5: Final Testing and Live Deployment](#phase-5-final-testing-and-live-deployment)
  - [Key Features](#key-features)
  - [Future Enhancements](#future-enhancements)
  - [Installation and Setup](#installation-and-setup)
  - [**Prerequisites**](#prerequisites)
  - [**1. Clone the Repository**](#1-clone-the-repository)
  - [License](#license)

---

## Development Journey

### Phase 1: Initial Setup and Planning

The project was initialized using **Next.js**, with hosting provided by **Vercel** for seamless deployment. The aim was to create a scalable e-commerce platform that allowed the client to manage product information independently through **Sanity Studio**.

### Phase 2: Main Pages and Reusuable Components

#### Navbar

- On mobile devices, the navbar includes a responsive overlay menu, providing easy navigation in a compact, user-friendly format.
- Cart icon that dynamically tracks the subtotal and number of items in the cart
- Clicking the cart icon opens a side cart menu, allowing users to view and manage items in their cart without leaving the current page.

#### Shop Page

- Displays products in a visually appealing grid, with each card linking to its individual product page for further exploration.

#### Product Detail Page

- Shows detailed information about a single product, including title, description, price, stock, and an option to add the product to the cart

#### Cart Page

- Lists all items added to the cart, allowing users to modify quantities or remove products before proceeding to checkout
- Cart side menu is built into the cart icon in the Navbar

#### Checkout Page

- Handles the payment process using Stripe Checkout and provides a summary of the user’s order before completing the purchase.
- Users are then routed to a success page with order details or a cancel page if they choose to cancel their purchase

#### About Page

- Includes an owner profile card, a call to action with contact and custom order Google forms, a photo gallery carousel, and a collapsible FAQ section.

### Phase 3: Sanity Integration and Product Fetching

- Sanity is used as the CMS, allowing the client to manage products (title, description, price, image, stock) through a simple dashboard.
- Products are structured with fields like title, price, and images, enabling easy updates via the CMS.
- Product data is fetched from Sanity using GROQ queries, allowing the site to display up-to-date product information dynamically.
- Changes in Sanity are reflected immediately on the site, ensuring seamless content updates without developer input.

### Phase 4: Stripe Integration and Testing

- Stripe is integrated to handle secure payments. Users can complete purchases through Stripe Checkout, which processes credit card payments.
- Custom API routes are used to create and retrieve checkout sessions, enabling smooth transaction flow between the site and Stripe.

### Phase 5: Final Testing and Live Deployment

- Conducted thorough testing of the checkout process, cart functionality, and responsive design to ensure everything worked smoothly across devices.
- The site was deployed on Vercel, providing a scalable and fast production environment with seamless integration for updates.

---

## Key Features

- Sanity Integration for Product Management
- Dynamic Product Pages
- Product Variants and Quantity Handling
- Cart Functionality with Context API
- Responsive and Mobile-Optimized Design
- Stripe Integration for Payment Processing
- Cart Summary and Order Summary
- Side Cart Menu
- Overlay Mobile Menu
- Confetti Animation on Successful Purchase

## Future Enhancements

- User Authentication and Account Management
- Wishlist or Favorites
- Product Recommendations
- Product Reviews and Ratings
- Enhanced Search and Filters
- Social Sharing Features

## Installation and Setup

## **Prerequisites**

Before starting, ensure you have the following software installed on your machine:

- **Node.js**: Version 14.x or higher
- **npm** (Node Package Manager): Installed with Node.js
- **Git**: To clone the repository
- **Sanity CLI**: To interact with the CMS
- **Stripe Account**: For payment processing

---

## **1. Clone the Repository**

First, clone the project repository to your local machine:

```bash
git clone https://github.com/your-username/ecommerce-app.git
cd ecommerce-app

```

## License

MIT License

Copyright ©️ 2024 Randall LaPoint, Jr.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.