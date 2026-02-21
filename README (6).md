# 🍕 Zomato Analytics — Pro Executive Dashboard

<div align="center">

![Zomato Analytics](https://img.shields.io/badge/🔴_Zomato-Analytics_Dashboard-E23744?style=for-the-badge&logoColor=white)
[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-View_Now-success?style=for-the-badge)](https://YOUR-USERNAME.github.io/zomato-dashboard/)
[![Built With](https://img.shields.io/badge/Built_With-HTML_CSS_JS-orange?style=for-the-badge)]()
[![Charts](https://img.shields.io/badge/Charts-Chart.js_4.4.1-blue?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)]()

**A fully interactive, production-grade food delivery analytics dashboard**
Built with pure HTML · CSS · JavaScript — no frameworks, no backend required

[🔴 View Live Demo](https://YOUR-USERNAME.github.io/zomato-dashboard/) · [📋 Report Bug](https://github.com/YOUR-USERNAME/zomato-dashboard/issues)

</div>

---

## 📌 Table of Contents

1. [About the Project](#-about-the-project)
2. [Dashboard Pages](#-dashboard-pages)
3. [Features Overview](#-features-overview)
4. [Tech Stack](#-tech-stack)
5. [Data Sources](#-data-sources)
6. [Key Metrics](#-key-metrics)
7. [Power BI Mapping](#-power-bi-mapping)
8. [Project Structure](#-project-structure)
9. [How to Run Locally](#-how-to-run-locally)
10. [How to Deploy on GitHub Pages](#-how-to-deploy-on-github-pages)
11. [Dashboard Architecture](#-dashboard-architecture)
12. [Analyst Profile](#-analyst-profile)
13. [License](#-license)

---

## 📖 About the Project

This project is a **single-file executive analytics dashboard** built to simulate a real Power BI report for a food delivery business (Zomato). It was created as part of a data analyst portfolio to demonstrate:

- Data wrangling and analysis from raw CSV files
- Dashboard design and UX thinking
- JavaScript-based chart building (Chart.js)
- Power BI feature replication in a browser
- Real-world business KPI storytelling

The entire dashboard — all 7 pages, 15 charts, animations, filters, drill-through panels, and the analyst profile — lives in **one single HTML file (183 KB)**. No server, no database, no framework needed.

> **"This dashboard is my proof of work — showing I can take raw data, find insights, and present them in a way business stakeholders can act on."**  
> — G. Saisagar, Data Analyst

---

## 📄 Dashboard Pages

The dashboard has **7 fully interactive pages**, each accessed via the left sidebar:

### 1. 🏠 Executive Overview
The command center — everything at a glance

- **Hero Banner** — Zomato-branded welcome section with animated scooter SVG, floating food emojis (🍕🍔🍜), and 5 headline stats (Revenue, Orders, Success Rate, Avg Delivery, Cities)
- **4 KPI Cards** — Total Revenue (₹1.60L), Total Orders (300), Delivery Rate (82%), Avg Delivery Time (32.3 min) — each with trend arrow badge, sparkline mini-chart, and hover tooltip
- **Revenue & Order Trend Chart** — Weekly line/bar/area chart with toggle buttons (Line / Bar / Area)
- **Order Status Donut Chart** — Delivered (246) vs Cancelled (54) visual split with large numbers
- **City Revenue Bar Chart** — Hyderabad vs Bangalore vs Chennai vs Mumbai comparison with radar toggle
- **City Market Cards (4 cards)** — Clickable cards with food emojis 🌶️🌿🐟🌊 that open drill-through panels, revenue bars, and city stats
- **Q1 Goal Tracker** — 5 animated progress bars comparing actual vs targets (Revenue, Delivery Rate, Orders, Delivery Time, AOV)
- **Live Activity Feed** — Real-time order events timeline with color-coded badges

---

### 2. 📦 Orders
Deep dive into all order transactions

- **4 KPI Cards** — Orders (300), Avg Order Value (₹534), Discounts Given (₹13.7K), Delivery Fees Collected (₹5.8K)
- **Payment Mode Split Bar Chart** — Wallet 83 · UPI 73 · Card 73 · COD 71
- **Orders by City Bar Chart** — Hyderabad (113) leads, Mumbai (57) is lowest
- **Full Order Transactions Table** — 20 rows with Order ID, Date, City, Restaurant, Value, Status pill (Delivered/Cancelled), Payment Mode, Delivery Time. Fully sortable by every column, searchable, with CSV Export button

---

### 3. 🍽 Food & Restaurants
Menu performance and restaurant analytics

- **4 KPI Cards** — Active Restaurants (10), Avg Rating (4.3★), #1 Restaurant (Biryani House 62 orders), Cuisines Offered (6)
- **Top Dishes Gallery** — 4 real food photo cards (Biryani, BBQ Chicken, Tandoori, Margherita) with hover zoom effect, trending fire badges, order count, and animated progress bars
- **Restaurant Photo Cards** — Top 4 restaurants with food images and star rating overlays
- **Cuisine Order Share** — Polar area chart: Indian (62) > Barbecue (52) > North Indian (52) > Italian (48) > South Indian (44) > Fast Food (42)
- **Restaurant Directory Table** — All 10 restaurants sorted by orders with revenue and rating bar

---

### 4. 🛵 Delivery Operations
Partner performance and logistics analysis

- **4 KPI Cards** — Active Partners (7), Avg Rating (4.1★), Avg Delivery Time (32.3 min), Total Deliveries (246)
- **Delivery Partner Leaderboard** — Ranked list with avatar, name, city, deliveries, avg time, animated performance bar, and star rating. All rows clickable for drill-through
- **Delivery Time Distribution Histogram** — 6 buckets: <25min to >37min showing delivery spread
- **Partner Performance Radar Chart** — Multi-series radar comparing top 4 partners on 5 dimensions (Rating, Deliveries, Speed, Coverage, Consistency)
- **City-wise Cancellation Stacked Bar** — Cancelled vs Delivered per city side by side

---

### 5. 👥 Customers
Customer demographics and spending behavior

- **4 KPI Cards** — Total Customers (10), Avg Age (26.5), Gender Split (50/50), Orders Per Customer (30)
- **Gender Distribution** — Two animated circular progress rings (50% Male / 50% Female) + weekly multi-line trend chart
- **Age Distribution Bar Chart** — Bar for each age 22–31 years
- **Customer Directory Table** — Full list: Name, City, Age, Gender (colored pill), Orders, Total Spend

---

### 6. 📊 Deep Analytics
Advanced data science layer

- **Order Volume Heatmap** — 8 hours × 7 days CSS grid with dynamic color intensity. Each cell shows order count with color from light pink → deep red
- **Customer Satisfaction Gauge** — Half-donut gauge showing 4.2/5.0 with breakdown: 89% Satisfied / 8% Neutral / 3% Unhappy + weekly satisfaction trend line
- **Order Value Distribution Histogram** — 5 price brackets (₹0–200 to ₹801+) showing how orders distribute across values
- **Revenue Waterfall Chart** — Gross Revenue (₹160,114) → minus Discounts (₹13,730) → plus Delivery Fees (₹5,810) → Net Revenue (₹152,194)

---

### 7. 👤 Analyst Profile — G. Saisagar
Built-in data analyst portfolio page

- **Profile Hero Banner** — Real photo, name, title badge, online status indicator, CGPA ring (8.04/10)
- **Contact Info** — Clickable email, phone, LinkedIn links
- **4 Action Buttons** — Hire Me (opens email), LinkedIn (external link), Download Resume (downloads .txt), Print/PDF (browser print)
- **Technical Skills Grid** — 12 hoverable skill chips with colored dot indicators
- **Skill Proficiency Animated Bars** — Animate from 0% on page open: Python 85%, SQL 88%, Power BI 80%, ML 72%, Excel 90%, Communication 85%
- **Experience Timeline** — Data Science Intern @ Intraintech + CSI Club Design Coordinator
- **3 Project Cards** — Each with emoji visual, tag badge, description, and metric grid
- **Education Card** — VIT AP University B.Tech CSBS 2021–2025 with badges
- **Quick Stats Grid** — 3 Projects · CGPA 8.04 · 88% ML Accuracy · 6+ Tools
- **Profile Summary** — Open to Work status, availability, location tags

---

## ✨ Features Overview

### Navigation & Layout

| Feature | How It Works |
|---|---|
| 7-Page Sidebar | Fixed 68px sidebar expands to 215px on hover, revealing page labels with icons |
| Page Transitions | `@keyframes fadeUp` — 0.35s ease with opacity + translateY on every switch |
| Topbar | Fixed header: logo, page title, LIVE dot, global search, filter button, bell, theme toggle, clock |
| Responsive | CSS Grid breakpoints at 960px — 4-column KPIs collapse to 2-column |

### Panels & Interactions

| Feature | How It Works |
|---|---|
| Filter Slicer Panel | 285px right panel slides in. Chip toggles for City / Status / Payment / Cuisine / Date. Range slider for Min Order Value |
| Drill-Through Panel | 420px right panel with food image, 4 KPI cards, mini Chart.js line chart, recent activity list |
| KPI Hover Tooltips | Floating positioned tooltip div shows contextual data (best city, SLA status, breakdown) |
| Notification Bell | Dropdown panel with 5 alerts: cancellation spike, revenue target, top restaurant, partner rating, city ranking |
| Global Search | Single input queries all three tables (orders, restaurants, customers) simultaneously on keypress |

### Charts (15 Total)

| Chart | Type | Page |
|---|---|---|
| Revenue & Order Trend | Line / Bar / Area (switchable) | Overview |
| Order Status | Doughnut | Overview |
| City Revenue | Bar / Radar (switchable) | Overview |
| Payment Mode | Bar | Orders |
| Orders by City | Bar | Orders |
| Cuisine Share | Polar Area | Food |
| Delivery Time Distribution | Bar (histogram bins) | Delivery |
| Partner Performance Radar | Multi-series Radar | Delivery |
| City Cancellation | Stacked Bar | Delivery |
| Gender Trend | Multi-line | Customers |
| Age Distribution | Bar | Customers |
| Order Value Histogram | Bar | Deep Analytics |
| Revenue Waterfall | Bar (+/-) | Deep Analytics |
| Satisfaction Gauge | Half-Doughnut overlay | Deep Analytics |
| Satisfaction Trend | Line | Deep Analytics |

### Animations & Theme

| Feature | Detail |
|---|---|
| Dark / Light Theme | CSS variable swap on body class. All Chart.js grid/label colors update dynamically |
| Animated KPI Counters | Count up from 0 using `requestAnimationFrame` with ease-out quartic easing curve |
| KPI Sparklines | 7-bar mini arrays on each card, last bar full opacity |
| Bookmark Page Animations | `pulseIn` scale keyframe on every page switch |
| Chart Type Toggle | Mutates existing Chart.js instance type — no re-creation overhead |
| Card Hover Lift | 4px translateY + box-shadow on all cards via CSS transition |
| Skill Bar Animation | Profile bars animate 0% → target with staggered 100ms delays |
| Food Image Hover Zoom | `transform: scale(1.07)` on image inside overflow:hidden wrapper |

### Data Table Features

| Feature | Detail |
|---|---|
| Sortable Columns | Click any `<th>` — toggles asc/desc, handles string and numeric, shows ▲/▼ indicator |
| Live Search Filter | Hides non-matching `<tr>` elements on every keystroke |
| CSV Export | Generates CSV blob from JavaScript array, triggers browser file download |
| Drill Mini Charts | Each drill-through renders a fresh Chart.js line for that entity |
| Order Heatmap | 56-cell grid (8 hours × 7 days) with `rgba(226,55,68, dynamic-alpha)` coloring |

---

## 🛠 Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| HTML5 | — | Page structure, semantic layout |
| CSS3 | — | Custom properties, Grid, Flexbox, animations, transitions |
| Vanilla JavaScript | ES6+ | All interactivity — no jQuery, no React, no Vue |
| Chart.js | 4.4.1 via CDN | All 15 chart visualizations |
| Google Fonts | — | Nunito (display/headings) + Inter (body text) |
| Unsplash | Free image CDN | Food photography for restaurant and dish cards |
| Base64 Image | Embedded | Analyst photo embedded directly — works offline |

> Zero dependencies to install. Chart.js loads from CDN. Just open index.html.

---

## 📁 Data Sources

The dashboard uses 4 CSV files from a synthetic food delivery dataset covering January 2026:

### Orders.csv — 300 rows
| Column | Type | Sample |
|---|---|---|
| Order_ID | String | O1001, O1002 |
| Order_Date | Date | 12 Jan 2026 |
| Customer_ID | String | C201–C210 |
| Restaurant_ID | String | R101–R110 |
| Delivery_Partner_ID | String | D501–D507 |
| City | String | Hyderabad / Bangalore / Chennai / Mumbai |
| Order_Value | Float | ₹196 – ₹990 |
| Discount | Float | ₹0 – ₹150 |
| Delivery_Fee | Float | ₹0 – ₹50 |
| Payment_Mode | String | UPI / Wallet / Card / COD |
| Order_Status | String | Delivered / Cancelled |
| Delivery_Time_Min | Integer | 19–45 min (0 if cancelled) |

### Restaurants.csv — 10 rows
Biryani House · Pizza Hub · Burger Point · Dosa Corner · Tandoori Flames · WrapZone · Pasta Palace · Sushi World · BBQ Nation · Spice Garden

### Customers.csv — 10 rows
10 customers (C201–C210) aged 22–31, equal gender split, spread across 4 cities

### Delivery_Partners.csv — 7 rows
Vijay · Ajay · Ramesh · Manoj · Sunil · Suresh · Imran — ratings 3.8 to 4.4

---

## 📈 Key Metrics (January 2026)

```
Total Revenue         ₹1,60,114
Total Orders          300
Delivered             246  (82.0%)
Cancelled             54   (18.0%)
Avg Delivery Time     32.3 minutes
Avg Order Value       ₹534
Total Discounts       ₹13,730
Total Delivery Fees   ₹5,810
Net Revenue           ₹1,52,194

Cities                4 (Hyderabad, Bangalore, Chennai, Mumbai)
Restaurants           10
Delivery Partners     7
Customers             10

Top City              Hyderabad — 113 orders, ₹59,440
Top Restaurant        Biryani House — 62 orders, ₹31,405
Best Partner Rating   Imran, Mumbai — 4.4 stars
Fastest Partner       Manoj, Chennai — 30.7 min avg
Top Payment Mode      Wallet — 83 transactions
Best Delivery City    Chennai — only 7 cancellations (10.6%)
```

### Revenue by City

| City | Orders | Revenue | Avg Value | Cancelled |
|---|---|---|---|---|
| Hyderabad | 113 | ₹59,440 | ₹526 | 20 (17.7%) |
| Chennai | 66 | ₹36,223 | ₹549 | 7 (10.6%) |
| Bangalore | 64 | ₹34,133 | ₹533 | 14 (21.9%) |
| Mumbai | 57 | ₹30,318 | ₹532 | 13 (22.8%) |

---

## 🔁 Power BI Mapping

| Power BI Feature | This Dashboard | Location |
|---|---|---|
| Page Navigation Buttons | Sidebar nav buttons with icons and labels | Left sidebar |
| Slicer Panel (Bookmarks) | Filter panel with chip selectors | Top filter button |
| Drill-through Pages | Sliding right panel per entity | City / restaurant / partner click |
| Report Page Tooltips | Hover tooltip floating panel | KPI card hover |
| Bookmark Animations | Chart type toggle + page transitions | Line/Bar/Area buttons |
| Theme JSON Dark/Light | CSS variable class swap | Moon/sun toggle |
| KPI Visual | KPI cards with trend badge and sparkline | All pages, top row |
| Line Chart | Chart.js line with fill | Overview trend |
| Bar Chart | Chart.js bar rounded corners | Multiple pages |
| Donut Chart | Chart.js doughnut | Overview status |
| Polar Area | Chart.js polar | Food — cuisine share |
| Radar Chart | Multi-series radar | Delivery — partner radar |
| Gauge / KPI Ring | Half-doughnut + centered text overlay | Deep Analytics |
| Matrix Table | Sortable HTML table with search | Orders, Food, Customers |
| Heatmap | Custom CSS grid + JS color interpolation | Deep Analytics |
| Waterfall Chart | Bar chart with positive and negative values | Deep Analytics |
| Sparkline | 7-bar mini array in KPI footer | All KPI cards |
| Goal / Progress Bar | Animated CSS progress with % label | Overview goal tracker |
| Notifications | Bell dropdown with categorized alerts | Topbar |
| Export Data | CSV blob download | Orders page button |

---

## 📁 Project Structure

```
zomato-dashboard/
│
├── index.html                  ← ENTIRE DASHBOARD — single file, 183 KB
│                                 HTML + CSS (40+ components) + JS (25+ functions)
│                                 + Chart.js configs + base64 photo embedded
│
├── README.md                   ← Full documentation (this file)
│
└── data/                       ← Source CSV files for reference
    ├── Orders.csv              300 order records
    ├── Restaurants.csv         10 restaurant records
    ├── Customers.csv           10 customer records
    └── Delivery_Partners.csv   7 delivery partner records
```

> The CSV data has been pre-processed and embedded as JavaScript arrays inside index.html. The CSV files are included for transparency and reproducibility.

---

## 💻 How to Run Locally

### Option 1 — Double Click (Easiest)
```
1. Download or clone the repo
2. Open the folder
3. Double-click index.html
4. Opens in browser instantly — done
```

### Option 2 — VS Code Live Server
```
1. Open folder in VS Code
2. Install "Live Server" extension (by Ritwick Dey)
3. Right-click index.html → "Open with Live Server"
4. Opens at: http://127.0.0.1:5500/
```

### Option 3 — Python Local Server
```bash
cd zomato-dashboard
python -m http.server 8000
# Open browser: http://localhost:8000
```

### Option 4 — Git Clone
```bash
git clone https://github.com/YOUR-USERNAME/zomato-dashboard.git
cd zomato-dashboard
open index.html       # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

No npm install. No pip install. No .env files. No build step required.

---

## 🚀 How to Deploy on GitHub Pages

### Step 1 — Create GitHub Account
Visit https://github.com/signup and create a free account.

### Step 2 — Create New Repository
1. Click + icon (top-right) → New repository
2. Repository name: `zomato-dashboard`
3. Description: `Zomato Analytics Executive Dashboard — Data Analyst Portfolio`
4. Set visibility to: Public (required for free GitHub Pages)
5. Check: Add a README file
6. Click: Create repository

### Step 3 — Upload Your Files
1. Inside the repo, click Add file → Upload files
2. Drag and drop:
   - `index.html` (rename from Zomato_Pro_Dashboard_Final.html)
   - `README.md`
   - `data/` folder with all 4 CSV files (optional but professional)
3. Commit message: `:rocket: Launch Zomato Analytics Dashboard`
4. Click: Commit changes

> IMPORTANT: The HTML file MUST be named `index.html` exactly.

### Step 4 — Enable GitHub Pages
1. Go to your repository
2. Click the Settings tab
3. Click Pages in the left sidebar
4. Under Source, select: Deploy from a branch
5. Under Branch, select: main and / (root)
6. Click: Save

### Step 5 — Access Your Live URL
Wait 2–5 minutes. Refresh the Pages settings. You will see:

```
Your site is live at:
https://YOUR-USERNAME.github.io/zomato-dashboard/
```

### Step 6 — Share Your Dashboard Link
- Add to your GitHub profile → Edit profile → Website field
- Pin the repository → Customize your pins → select zomato-dashboard
- Add to your LinkedIn profile → Featured section
- Add to your resume under Projects with the live URL

---

## 🏗 Dashboard Architecture

### CSS Design System
```
Layer 1: :root variables      Color tokens, spacing, shadow, transition
Layer 2: .lt class            Light theme — swaps all tokens
Layer 3: Layout               .sb (sidebar), .tb (topbar), .main, .footer
Layer 4: Panels               .fp (filter), .drp (drill), .notif-panel
Layer 5: Components           .kpi, .card, .food-card, .rest-card, .city-card
Layer 6: Tables               table, thead, tbody, .pill, .rbar
Layer 7: Profile              .profile-hero, .ph-banner, .proj-card, .timeline
Layer 8: Utilities            .badge, .tb2, .chips, .chip, .sw-btn
Layer 9: Animations           @keyframes fadeUp, pulse, bm
Layer 10: Media queries       960px breakpoint
```

### JavaScript Data Layer
```javascript
ORDERS[]          — 20 sample rows (structure matches full 300)
RESTAURANTS[]     — 10 restaurants with name, city, cuisine, rating, revenue, image
PARTNERS[]        — 7 delivery partners with stats and colors
CUSTOMERS[]       — 10 customers with demographics
DISHES[]          — 4 top dishes with images and trending flags
```

### JavaScript Function Map
```javascript
INIT (called on DOMContentLoaded)
  buildSparks()       — KPI sparkline mini-charts
  initCharts()        — All 15 Chart.js instances
  buildTables()       — Populate 3 sortable tables
  buildFoodCards()    — Food gallery + restaurant cards
  buildHeatmap()      — 56-cell order heatmap
  animateCounters()   — requestAnimationFrame counter animations

NAVIGATION
  goPage(p)           — Switch page, animate, update title

PANELS
  toggleFilter()      — Open/close filter slicer
  toggleNotif()       — Toggle notification dropdown
  closeDrp()          — Close drill-through panel

DRILL-THROUGH
  drillCity()         — Open panel with city/restaurant data
  openDrill(r)        — Open panel from restaurant object
  drillPartner()      — Open panel from partner row

THEME
  toggleTheme()       — Swap .lt class + update all chart colors

CHART CONTROLS
  switchTrend()       — Mutate trend chart type (line/bar/area)
  switchCity()        — Mutate city chart type (bar/radar)
  switchTrendType()   — Topbar toggle button handler

TABLES
  sortTable()         — Sort any table by column, asc/desc
  filterTable()       — Live row filter on keypress
  handleSearch()      — Global search across all tables

DATA EXPORT
  exportCSV()         — Generate CSV blob + download

TOOLTIPS
  tip()               — Show positioned tooltip on hover
  hidetip()           — Hide tooltip on mouseleave

PROFILE
  downloadResume()    — Generate resume text file + download
  printProfile()      — window.print() trigger
  animateSkillBars()  — Staggered skill bar fill animation

UTILITY
  tick()              — Live clock update every 1 second
```

---

## 👤 Analyst Profile

| Field | Details |
|---|---|
| Name | G. Saisagar |
| Role | Data Analyst |
| Education | B.Tech Computer Science & Business Systems, VIT AP University (2021–2025), CGPA 8.04/10 |
| Location | Bengaluru, India |
| Email | saisagar200123@gmail.com |
| Phone | +91 9100606922 |
| LinkedIn | linkedin.com/in/sai-sagar-6824a2238 |
| Status | Open to full-time opportunities |

### Technical Skills
Python · SQL · Power BI · Excel · R · Weka · Machine Learning · EDA · Dashboards · Data Cleaning · KPI Reporting · Business Analysis

### Projects
| Project | Technology | Key Achievement |
|---|---|---|
| Sign Language Recognition | Python, ML, Classification | Improved accuracy 70% → 88% |
| Women Safety Device | IoT, GPS, GSM modules | Reduced emergency response time |
| Loan Credit Score ML | Python, Scikit-learn, FinTech | Reduced false positives, full documentation |

### Experience
- Data Science Intern — Intraintech (Remote, 2023): ML workflows, Python automation, stakeholder reporting
- Design Team Coordinator — CSI Club, VIT AP University: Led team, created event creatives, improved campus visibility

---

## 📊 Dashboard Stats

| Metric | Value |
|---|---|
| File size | 183 KB |
| Lines of code | ~1,650 |
| Pages | 7 |
| Charts | 15 |
| JavaScript functions | 25+ |
| CSS components | 40+ |
| CSS animations | 6 |
| Data records embedded | 300 orders, 10 restaurants, 10 customers, 7 partners |
| External dependencies | 1 (Chart.js 4.4.1 via CDN) |
| Backend required | None |
| Framework required | None |
| Install commands needed | None |

---

## 🙏 Acknowledgements

- [Chart.js](https://www.chartjs.org/) — Open-source JavaScript charting
- [Unsplash](https://unsplash.com/) — Free food photography
- [Google Fonts](https://fonts.google.com/) — Nunito and Inter typefaces
- Zomato — Brand design inspiration (this is an educational portfolio project only, not affiliated with Zomato)

---

## 📄 License

MIT License — free to use, modify, and distribute with attribution.

```
Copyright (c) 2026 G. Saisagar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files to use, copy, modify,
merge, publish, distribute, sublicense, and/or sell copies of the Software.
```

---

<div align="center">

**Built with love by G. Saisagar — Data Analyst**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/sai-sagar-6824a2238)
[![Email](https://img.shields.io/badge/Email-Hire_Me-E23744?style=flat-square&logo=gmail)](mailto:saisagar200123@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Live_Dashboard-success?style=flat-square)](https://YOUR-USERNAME.github.io/zomato-dashboard/)

*If this project helped you, please give it a ⭐ star!*

</div>
