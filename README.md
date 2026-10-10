# ⚡ Fluxxbank — Banking in Motion

A modern digital bank web application with a live customer-facing site and a full admin console, built with pure HTML/CSS/JS and powered by Supabase.

![Fluxxbank](og-cover.png)

## 🌐 Live Site
**[fluxxbank.netlify.app](https://fluxxbank.netlify.app)** — deployed on Netlify

## ✨ Features

### Customer Site
- Stunning landing page with animated hero, live market ticker & trust badges
- Interactive banking dashboard demo (send payments, watch charts update in real time)
- **Printable transaction receipts** (print or save as PDF)
- Auto-crossfading customer review backgrounds
- "Fluxxbank in Pictures" showcase gallery (cards, HQ, vault — 10 visuals)
- FAQ accordion, newsletter signup, 5-star rating badges
- **Real accounts** — sign up with email + password (stored in Supabase Auth + database)

### Admin Console (`/admin.html`)
- Login: `admin` / `fluxx2026` (demo)
- Live customer table — freeze / delete accounts (writes to the real database)
- Transaction monitor with fraud flagging
- Loan & card application approvals (approve/reject)
- Security audit log, activity feed, deposits chart

## 🛠️ Tech Stack
| Layer | Technology |
|---|---|
| Hosting | Netlify |
| Database & Auth | Supabase (PostgreSQL + Row Level Security) |
| Frontend | Vanilla HTML / CSS / JavaScript |
| Share previews | Open Graph + Twitter Cards |

## 🗂️ Project Structure
```
index.html      → Customer-facing bank website
admin.html      → Admin back-end console
og-cover.png    → Social share image (Open Graph)
favicon.png     → Browser tab icon
review 1-4.png  → Customer review background photos
show 1-3.png    → Fluxxbank card graphics (Visa / Credit / Metal)
show 4-10.png   → Showcase gallery photos (HQ, vault, ATMs…)
```

## 🗄️ Database Schema (Supabase)
- `profiles` — customer accounts (auto-created on signup via trigger)
- `transactions` — payment history
- `approvals` — pending loan/card applications
- `subscribers` — newsletter signups
- All tables protected with Row Level Security policies

## 🚀 Deploy Your Own
1. Fork/clone this repo
2. Create a free [Supabase](https://supabase.com) project
3. Run `fluxxbank-schema.sql` in the SQL Editor
4. Add your Project URL + publishable key in `index.html` and `admin.html` (top of script)
5. Deploy to Netlify (drag the folder or connect the repo)

## ⚠️ Disclaimer
Fluxxbank is a demo/educational project. It is not a licensed financial institution — no real money is involved.

---
© 2026 Fluxxbank · Built with ⚡ and caffeine
