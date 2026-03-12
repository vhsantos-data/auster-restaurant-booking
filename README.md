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

## 🔄 Development Methodology

The project followed **Scrum** with 2-week sprints and 4 MVPs:

| Phase | Timeline | Deliverable |
|-------|----------|-------------|
| MVP 1 | June → August | Basic prototype — restaurant search and listing |
| MVP 2 | August → September | Reservation system and menu visualization |
| MVP 3 | September → October | Responsive dashboard with analytics |
| MVP 4 | October → November | Final product with all integrations |

Each sprint delivered a tangible increment reviewed and improved based on user testing feedback.

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

## 📸 Screenshots & Demo

The platform includes 9+ distinct screens:

| # | Screen | Description |
|---|--------|-------------|
| 01 | Restaurant Cards | Browse restaurants with ratings, addresses, and quick-reserve buttons |
| 02 | Login / Sign Up | User authentication with email and social login options |
| 03 | Reservation System | Select guests, date, time, with popular time slot suggestions |
| 04 | Restaurant Details | Photos, menu, hours, location map, reviews |
| 05 | Categories | Filter by cuisine: Japanese, Italian, Desserts, Seafood, etc. |
| 06 | Restaurant Listing | Partner restaurants with logos (Outback, Coco Bambu, Fogo de Chao, etc.) |
| 07 | Auster+ Login | Separate portal for restaurant owners |
| 08 | Orders Table | Reservation management with customer data |
| 09 | Dashboard | Weekly/Monthly analytics with charts and KPIs |

The full TCC presentation is available in [`docs/TCC-Presentation.pdf`](docs/TCC-Presentation.pdf), including:
- Problem analysis with wait-time data (avg. 45 min per table)
- Before/after UI comparison
- 4 MVP evolution timeline with Scrum methodology
- Market analysis vs TheFork and OpenTable
- Technical, financial, and market viability analysis
- Site flow diagram
- Market & feasibility analysis

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
- [ ] AI-powered restaurant recommendations
- [ ] Restaurant analytics dashboard enhancements
- [ ] Mobile app (React Native)
- [ ] Expansion to Argentina, Colombia, Mexico

---

## 📋 Development Methodology

The project followed **Scrum** with 2-week sprints and 4 MVPs:

| Phase | Focus | Deliverable |
|-------|-------|------------|
| MVP 1 (Jun) | Core prototype | Restaurant search & listing |
| MVP 2 (Aug) | Booking flow | Table reservation & menu viewing |
| MVP 3 (Sep) | Business tools | Responsive dashboard for restaurants |
| MVP 4 (Nov) | Final product | Full integration & optimizations |

---

## 💰 Business Model

**Auster+** subscription plans for restaurants:

| Plan | Price | Features |
|------|-------|----------|
| Basic | Free | 2 users, 2GB storage, dashboard |
| Pro | R$499/mo | 10 users, 10GB, priority layout, help center |
| Enterprise | R$999/mo | 30 users, 15GB, custom layout, all features |

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
