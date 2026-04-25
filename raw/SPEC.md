# IAM Clothing Brand — Project Spec

## What Is It?
Christian streetwear brand. Premium, bold, faith-based apparel.

**Live URL:** https://xxdjhugoxx.github.io/IAM/
**GitHub:** https://github.com/xxdjhugoxx/IAM
**Status:** Live on GitHub Pages

---

## Brand Identity

- **Name:** IAM (all caps, varsity block style)
- **Tagline:** "Faith In Every Thread"
- **Scripture:** John 14:6

### Logo Style
- Varsity block letters "IAM"
- Maroon inner (#6B1C2A)
- Cream outer border (#F5F0E8)
- Thick, bold, collegiate feel

### Color Palette
- Primary: Maroon #6B1C2A
- Secondary: Cream #F5F0E8
- Background: Black #0A0A0A
- Text: White/Cream

### Typography
- Headings: Bebas Neue
- Body: Inter

---

## Pages

| Page | File | Purpose |
|------|------|---------|
| Landing | `index.html` | Brand statement, scripture, no products |
| Shop | `shop.html` | Product catalog + cart + checkout |
| Client Portal | `client-portal.html` | Track orders by email |
| Admin Portal | `admin.html` | Scan & ship, manage orders |

---

## Products

| Name | Price | Category |
|------|-------|----------|
| Essential Tee | $48 | tops |
| Oversize Hoodie | $118 | outerwear |
| Camp Cap | $38 | accessories |
| Praying Hands Tee | $45 | tops |
| Cross Hoodie | $98 | outerwear |
| Scripture Tee | $50 | tops |

---

## Architecture

### Frontend
- Static HTML/CSS/JS (Netlify-ready)
- GitHub Pages enabled (`gh-pages` branch)

### Backend
- Express API at `api/server.js`
- Runs on port 3001
- **Needs 24/7 server deployment**

### Database
- Supabase schema at `supabase/schema.sql`
- **Needs Supabase connection**

---

## Admin Credentials

- **Email:** admin@iam.com
- **Password:** admin123

---

## Workflow

1. Client → shop.html → places order
2. Order → API → saved to database
3. Admin → admin.html → sees pending orders
4. Admin → "Scan & Ship" → enters tracking ID
5. System → emails client with tracking
6. Client → client-portal.html → tracks order

---

## TODO

- [ ] Deploy backend API on server (24/7)
- [ ] Connect to Supabase database
- [ ] Configure SMTP for email notifications
- [ ] Add real product images
- [ ] Stripe/payment integration
- [ ] Custom domain (iam.com)

---

*Last updated: 2026-04-25*
