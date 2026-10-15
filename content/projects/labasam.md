---
title: "Labasam"
description: "A ride sharing app"
dateString: Dec 2025
draft: false
tags: ["AWS", "Django", "Celery", "GitHub Action", "Docker", "Postgres"]
showToc: false
weight: 49
cover:
    image: "/projects/labasam/labasam_homepage1.jpeg"
---
<style>
  .store-link {
    color: #32CD32;
    font-weight: bold;
    text-decoration: none;
    display: inline-block;     /* stays on one line */
    margin-right: 25px;        /* spacing */
    border-bottom: 2px solid transparent;  /* small underline */
    padding-bottom: 2px;
  }
  .store-link:hover {
    border-bottom: 2px solid #32CD32;      /* underline only text */
  }
</style>
<!-- 
<a class="store-link">Play Store (Passenger) ↗</a>
<a class="store-link" href="https://play.google.com/store/apps/details?id=com.labasam.rider&hl=en" target="_blank" rel="noopener noreferrer">Play Store (Driver) ↗</a>
<a class="store-link" href="https://apps.apple.com/np/app/labasam/id6677030592" target="_blank" rel="noopener noreferrer">App Store (Passenger) ↗</a>
<a class="store-link" href="#">App Store (Driver) ↗</a> -->


<a class="store-link" href="https://play.google.com/store/apps/details?id=com.labasam.rider&hl=en" target="_blank" rel="noopener noreferrer">Play Store ↗</a>
<a class="store-link" href="https://apps.apple.com/np/app/labasam/id6677030592" target="_blank" rel="noopener noreferrer">App Store  ↗</a>

## Intro
**LaBasam** is a Nepal-based ride-sharing app available on iOS and Android, built to make daily travel faster, easier, and safer for passengers and drivers.

Nepal’s transport system often suffers from unreliable rides, inconsistent pricing, and limited safety measures during travel.

LaBasam solves these issues with real-time tracking and a powerful SOS feature that instantly alerts the admin with geo-hash location and sends emergency SMS updates to saved contacts, ensuring quick and reliable support.

---

## 🛠 Tech Stack

- **Backend:** Django (Python), Django REST Framework (DRF), Node
- **Cloud Services:** AWS EC2 (hosted backend), S3 (for static/media files), CloudFront (CDN)
- **Deployment:** Docker, Gitlab Action CI/CD
- **Database:** PostgreSQL (via AWS RDS)
- **Task Queue:** Celery + Redis (for background jobs)
- **SMS Service:** Akash SMS (used for OTP verification and sending SOS alerts)

---

## ⚙️ How It Works

### Passenger Flow
- **Sign Up & Verification:** Passengers register using their first, middle, and last name, phone number, and email. OTP verification is required for login.  
- **Booking Rides:** Passengers can book **Quick Rides**, **City-to-City rides**, or **Parcel delivery**.  
- **Pink Mode:** Female passengers can enable Pink Mode to see only female drivers.  
- **Rating & Review:** After each ride, passengers can rate and review their drivers.  

### Driver Flow
- **Sign Up & Verification:** Drivers register similarly, then provide driver details (license, expiry, photo) and vehicle details (type, brand, model, billbook, insurance, seating capacity).  
- **Approval:** Admin reviews all driver and vehicle documents. Only verified drivers can accept rides.  

### Admin & Staff Flow
- **Roles:** Admin manages everything and can create staff with specific roles. Staff can handle tasks such as **driver/vehicle management** or **SOS alerts**.  
- **Operations Management:** Ensures smooth ride assignments, safety monitoring, and verification processes.  

### Key Features / Backend Handling

- **SOS System:** Alerts admin instantly with geo-hash location and notifies emergency contacts via SMS with Google Maps link.  
- **Points & Rewards:** Passengers and drivers earn points per ride; 5-star drivers get bonus points; points can be used for giveaways.  
- **Single-Role Enforcement:** Prevents logging in as both passenger and driver on the same device.  
- **Automatic Logout:** Detects device and logs out the other session during OTP verification.  
- **Points Integrity:** Ensures points are earned fairly and cannot be manipulated.  
- **Real-time Tracking & Notifications:** Tracks rides and sends updates to passengers, drivers, and admin in real-time.

---

## 🚀 Final Thoughts

Developing **Labasam** allowed me to build a full-featured ride-sharing platform with real-time tracking, secure OTP authentication, and advanced safety mechanisms like SOS alerts. It was a valuable experience in integrating backend verification, user experience design, and scalable features for both passengers and drivers.

---

