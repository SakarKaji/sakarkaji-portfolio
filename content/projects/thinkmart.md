---
title: "Thinkmart"
description: "Online Grocery Platform for the Australian Market"
dateString: Feburary 2025
draft: false
tags: ["AWS", "RegEx", "MkDocs", "GitHub Action", "Docker", "Bash", "TypeScript", "Node.JS"]
weight: 52
cover:
    image: "/projects/thinkmart/cover.png"

showToc: false

---


<a href="https://www.thinkmart.com.au/" target="_blank" rel="noopener noreferrer" style="color:#32CD32; font-weight:bold; text-decoration:none;">
  View Project ↗
</a>

## Intro
[**Thinkmart**](https://www.thinkmart.com.au/) is a multi-vendor online grocery marketplace in Australia, making Nepali and other ethnic products easy to find while letting vendors manage their products, deals, and deliveries.

It solves the problem of customers struggling to find familiar products in one place and helps small stores sell online without building their own system.

With features like product syncing, secure Stripe payments, daily deals, and admin-approved vendor sign-up, Thinkmart offers an easy and smooth experience for both customers and vendors.

---

## 🛠 Tech Stack

- **Backend:** Django (Python), Django REST Framework (DRF)
- **Cloud Services:** AWS EC2 (hosted backend), S3 (for static/media files), CloudFront (CDN)
- **Deployment:** Docker, GitHub Actions CI/CD
- **Database:** PostgreSQL (via AWS RDS)
- **Task Queue:** Celery (for sending otp)

---

## ⚙️ How It Works

### Vendor Flow

- **Sign Up:** Vendors register using a form, providing store details, location, images, and other necessary information.

- **Approval:** Admin reviews and approves the vendor before their products are listed.

- **Product Management:** Once approved, vendors can add, edit, and manage products, set discounts, and create “Today’s Deals.”

- **EPOS Integration:** Vendors can sync products and inventory with EPOS Now to keep online and in-store catalogs consistent.

### Customer Flow

- **Sign Up & Verification:** Customers register via a form with OTP email verification (handled asynchronously by Celery) or Google Sign-In.

- **Browse Products:** Customers can browse products by category, deals, or offers.

- **Wishlist & Cart:** Customers can add products to their wishlist or cart for later purchase.

- **Place Orders:** Customers checkout securely using Stripe and can order from multiple vendors in one transaction.

- **Order Notifications:** Customers receive emails with details of the products they ordered, including prices and vendor information.

### Key Features / Backend Handling

- **Multi-vendor support:** Each vendor manages their own products, discounts, and delivery rules.

- **OTP verification & email notifications:** Managed asynchronously using Celery.

- **Deals & Offers:** “Today’s Deals” and special offers highlight discounted products.

- **Payment Integration:** Stripe enables secure and seamless customer payments.

- **EPOS Sync:** Bi-directional product and inventory flow between Thinkmart and vendor POS.

- **Order Emails:** Customers get detailed emails for every order they place, showing products and prices.
---

## 🚀 Final Thoughts

[**Thinkmart**](https://www.thinkmart.com.au/) bridges a real market gap: it brings community-specific grocery catalogs (like Nepali
products) into a modern, scalable marketplace while staying inclusive of all vendors. 

With a robust AWS + Django/DRF backbone, async tasking via Celery, Stripe payments, and EPOS Now syncing, the platform balances customer convenience with vendor autonomy—and sets the stage for sustainable growth across Australian suburbs and beyond.

---




