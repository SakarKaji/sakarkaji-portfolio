---
title: "Ayomomo"
description: "A web app bringing authentic Nepali momo to food lovers all across the UK."
dateString: Jun 2025
draft: false
tags: ["AWS", "Django", "Celery", "GitHub Action", "Docker"]
showToc: false
weight: 50
cover:
    image: "/projects/ayomomo/homepage1.png"
---
## Intro

[**Ayomomo**](https://www.ayomomo.com/) is a web-based platform built for a modern Nepali restaurant that specializes in authentic dumplings (momos). The project aims to bring traditional cuisine into the digital space with a fast, scalable, and cleanly designed web presence. It showcases brand identity while also laying the foundation for future features like online ordering, reservations, and customer profiles.

---

## 🛠 Tech Stack

- **Backend:** Django (Python), Django REST Framework
- **Frontend:** HTML, Tailwind CSS (with Django templates)
- **Task Queue:** Celery + Redis (for background jobs)
- **Deployment:** Docker, GitHub Actions CI/CD
- **Cloud Services:** AWS EC2 (hosted backend), S3 (for static/media files), CloudFront (CDN)
- **Database:** PostgreSQL (via AWS RDS)
- **Authentication:** Django Auth with session management

---

## ⚙️ How It Works

- **Home Page:** Clean and responsive layout that introduces the brand and food concept
- **Authentication:** Users can sign up and log in securely using Django's built-in auth system
- **FAQ & About Us:** Static pages rendered via Django templates to inform users
- **Scalability:** Cloud-native setup using AWS EC2 and S3; Dockerized backend with automatic CI/CD via GitHub Actions
- **Performance:** CloudFront used as a CDN to deliver static assets globally with low latency
- **Background Processing:** Celery handles asynchronous tasks (e.g., image optimization, email jobs)

---

## 🚀 Final Thoughts

Ayomomo was a full-stack project that helped me bring together modern web development skills—from backend architecture to cloud deployment. I gained hands-on experience with DevOps (CI/CD), asynchronous task management, and scalable application design.

This project reflects my ability to:
- Build and deploy a production-ready backend system
- Architect cloud-based, scalable infrastructure
- Combine clean design with performance-first development practices

Next steps could include:
- Implementing a real-time order management system
- Integrating Stripe or Khalti for online payments
- Building a mobile-first frontend using React or Next.js

---
