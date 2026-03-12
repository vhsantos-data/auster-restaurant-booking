# 🍽️ Auster — Restaurant Reservation Platform

> A restaurant booking platform designed for the Latin American market, targeting premium dining experiences.

![Status](https://img.shields.io/badge/Status-Academic_Project-blue)
![Stack](https://img.shields.io/badge/Stack-HTML%20|%20CSS%20|%20JS%20|%20PHP%20|%20MySQL-orange)
![Bootstrap](https://img.shields.io/badge/UI-Bootstrap_5-purple)

---

## 📋 About

**Auster** (from *Austerity*) was born from a market gap we identified: there is no strong restaurant reservation platform focused on Latin America. Existing solutions are international with limited coverage in the region, especially for premium dining.

This project was developed as a **Final Year Thesis (TCC)** during a 4-year Integrated Technical High School in Systems Development at FITO (São Paulo, Brazil).

### The Problem
- International booking platforms (OpenTable, Resy) have minimal Latin American presence
- No dedicated solution for premium/fine dining reservations in Brazil
- Restaurants lack integrated tools for managing bookings and customer flow

### Our Solution
A web platform where users can discover premium restaurants, make reservations, and manage their dining experiences — while restaurants get tools to manage bookings and track customer engagement.

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────┐
│                  Frontend                    │
│  HTML5 + CSS3 + JavaScript + Bootstrap 5    │
├─────────────────────────────────────────────┤
│              Backend (PHP)                   │
│  Authentication | Reservation Logic          │
├─────────────────────────────────────────────┤
│            Database (MySQL)                  │
│  Users | Restaurants | Reservations          │
└─────────────────────────────────────────────┘
```

---

## ✨ Features

**For Customers:**
- 🔍 Browse and search restaurants by cuisine, location, and rating
- 📅 Make reservations (date, time, number of guests)
- 📍 Geolocation — find restaurants nearby
- 👤 User registration and authentication
- ❓ FAQ and Help center

**For Restaurants:**
- 🏢 Business portal for restaurant owners
- 📊 Dashboard for managing reservations
- 💎 Auster+ premium subscription plans

---

## 📁 Project Structure

```
auster-restaurant-booking/
├── src/
│   ├── index.html              # Homepage (carousel, features, partners)
│   ├── css/
│   │   ├── home.css            # Main styles
│   │   ├── auth.css            # Login/Signup styles
│   │   ├── Restaurantes.css    # Restaurant listing styles
│   │   ├── FAQs.css            # FAQ page styles
│   │   └── about.css           # About page styles
│   ├── js/
│   │   ├── home.js             # Homepage interactions
│   │   └── reserva.js          # Reservation logic
│   ├── pages/
│   │   ├── Restaurantes.html   # Restaurant catalog
│   │   ├── reserva.html        # Reservation form
│   │   ├── signup.html         # User registration
│   │   ├── FAQs.html           # Frequently asked questions
│   │   └── about.html          # About Auster
│   └── assets/
│       └── img/                # Logos, restaurant images
├── backend/
│   ├── config/
│   │   ├── database.php        # Database connection (env-based)
│   │   └── schema.sql          # Database schema + seed data
│   └── auth/
│       ├── login.php           # User authentication
│       └── register.php        # User registration
├── docs/                       # Documentation & wireframes
├── .env.example                # Environment variables template
├── .gitignore
└── README.md
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, JavaScript |
| UI Framework | Bootstrap 5 |
| Backend | PHP |
| Database | MySQL |
| Features | YouTube API (intro video), Geolocation API, CSS Animations |

---

## 🚀 Getting Started

### Prerequisites
- PHP 7.4+
- MySQL 5.7+
- Web server (Apache/Nginx) or XAMPP/WAMP

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/vhsantos-data/auster-restaurant-booking.git
cd auster-restaurant-booking
```

2. **Configure the database**
```bash
cp .env.example .env
# Edit .env with your database credentials
```

3. **Create the database**
```bash
mysql -u root -p < backend/config/schema.sql
```

4. **Start local server**
```bash
php -S localhost:8000 -t src/
```

5. **Open in browser**
```
http://localhost:8000
```

---

## 📸 Screenshots

> *Screenshots coming soon — homepage, reservation flow, restaurant listing*

---

## 🎯 Market Analysis

| Platform | LatAm Coverage | Premium Focus | Local Restaurants |
|----------|:-:|:-:|:-:|
| OpenTable | ❌ Limited | ✅ | ❌ |
| Resy | ❌ Minimal | ✅ | ❌ |
| TheFork | ⚠️ Partial | ⚠️ | ⚠️ |
| **Auster** | ✅ **Brazil-first** | ✅ | ✅ |

---

## 📈 Future Roadmap

- [ ] React/Next.js frontend migration
- [ ] RESTful API with Node.js or Laravel
- [ ] Real-time availability system
- [ ] Payment integration (Stripe/MercadoPago)
- [ ] Restaurant analytics dashboard
- [ ] Mobile app (React Native)
- [ ] Expansion to Argentina, Colombia, Mexico

---

## 👥 Team

Developed as a Final Year Thesis (TCC) at FITO — Integrated Technical High School in Systems Development.

**Vitor Hugo Santos** — Full-Stack Development & Business Strategy
- [LinkedIn](https://www.linkedin.com/in/vhsantos-data)
- [GitHub](https://github.com/vhsantos-data)

---

## 📄 License

This project is for academic and portfolio purposes.

---

*"The best solutions come from real market gaps, not from copying existing products."*
