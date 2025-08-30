---
title: "QuickSamachar"
description: "News delivery application from multiple Nepali and Indian news sources."
dateString: November 2024
draft: false
tags: ["AWS","Django", "GitHub Action", "Docker", "Bash", "Scrappy", "Postgres",  "Edge-tts"]
weight: 53
cover:
    image: "/projects/quicksamachar/image.png"
showToc: false

---

<a href="https://apps.apple.com/np/app/quicksamachar/id6450090838" target="_blank" rel="noopener noreferrer" style="color:#32CD32; font-weight:bold; text-decoration:none;"> Get App ↗ </a>

## Intro
[**QuickSamachar**](https://apps.apple.com/sg/app/quicksamachar/id6450090838) is a multilingual news delivery platform built to aggregate real-time content from major Nepali and Indian news sources

Elderly users and specially-abled users face challenges in reading or navigating conventional apps.

This app converts news into audio using Edge TTS and delivers organized articles along with daily horoscopes and trending short videos through a fast, cloud-powered backend, making content accessible to elderly users, specially-abled users, and anyone who prefers listening.



## 🛠 Tech Stack

- **Backend:** Django (Python), Django REST Framework (DRF)
- **Scraping:** Scrapy (for Nepali & Indian news sources)
- **Cloud & Hosting:** AWS EC2 (hosted backend), AWS EC2, S3 (audio & media storage), CloudFront (CDN)
- **Task Automation:** Docker, Celery, GitHub Actions
- **Database:** PostgreSQL (via AWS RDS)
- **Audio Conversion:** Edge TTS (Nepali & English)

---

## ⚙️ How It Works

### Flow

- **News Collection:** Scrapy crawls ~50 news sources, fetching cover images, titles and descriptions in Nepali and English .

- **Horoscope Collection:** Daily Nepali and English horoscopes are scraped and displayed in the app.

- **Trending Videos:** The app scrapes trending Nepali videos and displays them in the “Shorts” section for quick updates.

- **Content Storage:** VNews, horoscope, and video metadata are stored in PostgreSQL for 7 days, then refreshed automatically.

- **Storage & Delivery:** Audio and media files are stored in AWS S3 and served via CloudFront for fast streaming.

### User Features 

- Users can select their preferred language: Nepali, English, or both.

- Elderly users can listen to news instead of reading.

- Specially-abled users, including visually impaired people, can fully access news content via audio.

---

## 🚀 Final Thoughts

QuickSamachar bridges a critical accessibility gap in news delivery for Nepali users, including the elderly and visually impaired.

By combining web scraping, cloud storage, TTS audio, and multilingual support, its AWS + Django + Scrapy + Edge TTS backend ensures scalable, real-time news delivery with a smooth and user-friendly mobile experience on iOS and Android.

---