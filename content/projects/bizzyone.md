---
title: "Bizzyone"
description: "Bizzyone – A Connected Platform for Real Estate Buyers, Sellers & Agents"
dateString: May 2025
draft: false
tags: ["AWS", "Flask", "Celery", "GitHub Action", "Docker", "Postgres"]
weight: 51
cover:
    image: "/projects/bizzyone/home.png"

showToc: false

---

<a href="https://www.bizzyone.com/" target="_blank" rel="noopener noreferrer" style="color:#32CD32; font-weight:bold; text-decoration:none;">
  View Project ↗
</a>


## Intro

[**Bizzyone**](https://www.bizzyone.com/) is an online marketplace for commercial real estate which provides a platform where buyers, sellers, agents, and admins interact seamlessly.

In Nepal, real estate pricing is highly inconsistent, with sellers often quoting random rates and brokers charging excessive commissions and this lack of transparency creates confusion, mistrust, and unfair deals for both buyers and sellers. 

Bizzyone solves this by providing a transparent, standardized, and centralized platform for real estate transactions.

---

## 🛠 Tech Stack

- **Backend:** Flask (Python), Flask-RESTful APIs  
- **Database:** PostgreSQL (hosted on DigitalOcean)  
- **Cloud Services:** DigitalOcean Droplets (servers), Spaces (bucket storage)  
- **Task Queue:** Celery + Redis (for background jobs like email notifications, OTPs)  
- **Deployment:** Docker, GitHub Actions CI/CD  
- **Authentication:** Email/OTP (Celery), Google Sign-In, Apple Sign-In  

---

## ⚙️ How It Works

### Seller Flow
- **Sellers sign up** via form, Google, or Apple login.  
- **Create listings** (for rent, urgent sale, or standard sale) with property details: photos, floor plans, maps, and financials.  
- **Agent Support:** Sellers can also assign listings to agents, including broker/agent details.  
- **Admin Moderation:** Listings are reviewed by admins and faulty ones can be rejected.  

### Buyer Flow
- **Buyers register** through form, Google, or Apple login.  
- **Search listings** with advanced filters (category, price, property type).  
- **Post requirements** such as “Looking to buy retail space” or “Need industrial warehouse.”  
- **Contact sellers/agents** directly through the platform.  

### Subscription Model
- **Basic:** 3 listings per week, standard support.  
- **Standard:** 10 listings per week, includes featured listings.  
- **Premium:** Unlimited listings + advanced advertising & marketing tools.  

### Admin & Manager Flow
- **Admins manage users, listings, and subscriptions.**  
- **Moderation system** ensures only high-quality, fraud-free listings.  
- **Analytics & oversight** to track platform activity and performance.  

---

## 🚀 Final Thoughts
[**Bizzyone**](https://www.bizzyone.com/) is the live output of this project—an operational, subscription-based **real estate marketplace for Nepal**.  

Through this project, I strengthened my expertise in multi-role systems and  scalable backend services   