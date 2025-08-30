---
title: "Ayomomo"
description: "A web app bringing authentic Nepali momo to Nepalese and food lovers living across the UK."
dateString: Jun 2025
draft: false
tags: ["AWS", "Django", "Celery", "GitHub Action", "Docker", "Postgres"]
showToc: false
weight: 50
cover:
    image: "/projects/ayomomo/homepage1.png"
---

<a href="https://www.ayomomo.com/" target="_blank" rel="noopener noreferrer" style="color:#32CD32; font-weight:bold; text-decoration:none;">
  View Project ↗
</a>


## Intro

**[Ayomomo](https://www.ayomomo.com/)** is a web platform created for Nepali restaurants in United Kingdom specializing in authentic dumplings (momo). It was initiated by UK based Nepali chef Binod Baral. 

Many Nepalese living UK miss the authentic taste of their comfort food, and Ayomomo solves this by providing genuine momo that taste like home.

The goal of this project is connecting the Nepalese community to their culture as well as introduce Nepali cuisine to international food lovers.

---

## 🛠 Tech Stack

- **Backend:** Django (Python), Django REST Framework (DRF)
- **Cloud Services:** AWS EC2 (hosted backend), S3 (for static/media files), CloudFront (CDN)
- **Deployment:** Docker, GitHub Actions CI/CD
- **Database:** PostgreSQL (via AWS RDS)
- **Task Queue:** Celery + Redis (for background jobs)

---

## ⚙️ How It Works

### Restaurant Flow
- **Sign Up:** Restaurants register using a form, providing details like restaurant name, business phone number, location, and logo.  
- **Approval:** Admin reviews and approves the restaurant.  
- **Menu Management:** Once approved, restaurants can post their menu items and prices.  
- **Order Notifications:** When customers place orders, restaurants receive emails for each food item ordered, ensuring they prepare the correct items.  

### Customer Flow
- **Sign Up & Verification:** Customers register via a form with OTP email verification (handled asynchronously by Celery) or Google Sign-In.  
- **Browse Restaurants:** After account creation, customers can browse and choose nearby restaurants.  
- **Place Orders:** Customers place orders, selecting either delivery (cash on delivery) or pickup.  
- **Multi-Restaurant Orders:** Customers can order from multiple restaurants in a single order. They receive a single consolidated email with all items, while each restaurant receives emails only for their specific items.


### Key Features / Backend Handling
- **Multi-vendor support:** Each restaurant manages its menu and receives orders independently.
- **OTP verification & email notifications:** Managed asynchronously using Celery.
- **Delivery vs pickup:** Flexible ordering options for customers.
- **Order management:** Ensures correct email notifications to restaurants and customers.
---

## 🚀 Final Thoughts

Building [**Ayomomo**](https://www.ayomomo.com/) was a journey where I designed and deployed a production-ready system from backend to cloud.

Along the way, I implemented CI/CD pipelines, asynchronous task management, and scalable architecture.

---

