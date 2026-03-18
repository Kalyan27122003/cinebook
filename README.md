# 🎬 CineBook — Movie Ticket Booking App

A fully static, single-file movie ticket booking web app inspired by BookMyShow. No backend, no server, no build tools — just open `index.html` in a browser.

---

## 🌐 Live Demo

> https://your-site-name.netlify.app

---

## ✨ Features

- 🔐 User Signup & Login (stored in localStorage)
- 🎬 Movie listing with genre, language, rating & description
- 🕐 Showtimes across 3 screens with date tabs
- 💺 Visual seat map — 10×12 grid (120 seats per screen)
- 💰 3 pricing tiers: Silver / Gold / Premium
- 🎟️ Real-time seat selection with price calculation
- ✅ Booking confirmation modal with summary
- 📋 My Bookings page per user
- 🔒 Anti-double booking via seat lock state
- 📱 Responsive design for mobile & desktop

---

## 🛠️ Tech Stack

| Layer      | Technology                        |
|------------|-----------------------------------|
| Frontend   | HTML5, CSS3, Vanilla JavaScript   |
| Fonts      | Bebas Neue, Rajdhani, Inter       |
| Icons      | Font Awesome 6.5                  |
| Storage    | Browser localStorage              |
| Hosting    | Netlify                           |

---

## 📁 Project Structure

```
cinebook/
└── index.html      # Entire app — HTML + CSS + JS in one file
└── README.md
```

---

## 🚀 Getting Started

### Run Locally

No setup needed. Just open the file:

```bash
# Option 1 — double-click index.html in your file explorer

# Option 2 — use VS Code Live Server extension
# Right-click index.html → "Open with Live Server"
```

### Deploy to Netlify

1. Push this repo to GitHub
2. Go to [netlify.com](https://netlify.com) → **Add new site** → **Import from Git**
3. Select your repo
4. Leave build command and publish directory **blank**
5. Click **Deploy**

Every `git push` auto-redeploys.

---

## 🎭 Movies Included

| Title              | Genre            | Language | Duration |
|--------------------|------------------|----------|----------|
| Kalki 2898 AD      | Sci-Fi / Action  | Telugu   | 181 min  |
| Pushpa 2: The Rule | Action / Drama   | Telugu   | 190 min  |
| Stree 2            | Horror / Comedy  | Hindi    | 145 min  |
| RRR                | Action / Drama   | Telugu   | 182 min  |
| KGF Chapter 3      | Action / Drama   | Kannada  | 175 min  |

---

## 💺 Seat Pricing Tiers

| Category | Rows  | Default Price |
|----------|-------|---------------|
| Silver   | A – C | ₹150          |
| Gold     | D – G | ₹250          |
| Premium  | H – J | ₹400          |

---

## ⚙️ How It Works

Since this is a fully static app with no backend:

- **Auth** — user accounts are saved to `localStorage`. Passwords are hashed client-side before storing.
- **Bookings** — saved to `localStorage`, persist across page refreshes on the same browser.
- **Seat Locks** — booked seats are tracked in `localStorage` per slot, preventing double-booking within the same browser session.
- **Routing** — single-page app with a custom `navigate()` function that shows/hides page sections.

---

## 📸 Pages

| Page       | Description                              |
|------------|------------------------------------------|
| Home       | Movie grid with hero banner and ticker   |
| Login      | Email + password login form              |
| Signup     | Account creation form                    |
| Slots      | Showtimes by date and screen             |
| Seats      | Interactive seat map with price summary  |
| Bookings   | All bookings for the logged-in user      |

---

## 📝 License

MIT — free to use and modify.