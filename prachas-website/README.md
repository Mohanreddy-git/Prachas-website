# Prachas Technologies — Website (Static HTML/CSS/JS)

A clean, hand-coded, fully responsive recreation of the Prachas Technologies
website (prachas.com), matching the **real content and page structure** of the
live GoDaddy site. Built with plain HTML5, CSS3 and vanilla JavaScript —
**no build step, no frameworks, no external dependencies.** It runs anywhere.

## Pages (match the live site's menu and slugs)
| File                 | Page         | Live URL                       |
|----------------------|--------------|--------------------------------|
| `index.html`         | Home         | prachas.com/                   |
| `about-us.html`      | About Us     | prachas.com/about-us           |
| `services.html`      | Services     | prachas.com/services           |
| `join-us.html`       | Join Us      | prachas.com/join-us            |
| `contact-us.html`    | Contact Us   | prachas.com/contact-us         |
| `current-jobs.html`  | Current Jobs | prachas.com/current-jobs       |

## Content notes — matched to the live site
- **Home** sections in order: Hero, "Why Prachas? / Affordable Remote Services",
  Our Services, About Prachas (Vision + Values), and a **"My Blog"** section.
- **My Blog is empty on the live site** (a heading with no posts), so this build
  shows a matching "posts coming soon" placeholder rather than invented articles.
  *Blog is not in the navigation menu — same as the live site.*
- **About Us** — outsourced BPO office in Hyderabad, 11+ years serving US
  customers, "see us in person" block with address, phone and hours.
- **Join Us** — "We're Hiring! / Join Our Team" with an Apply Now form
  (Name, Phone, Email, Attach Resume).
- **Contact Us** — "Request a free quote" with a Request For Quote form
  (First Name, Last Name, Business Name, Phone, Email, Country, Required
  Services, Attachment), plus WhatsApp, email (contact@prachas.com) and hours.
- **Current Jobs** — the live page has no listings, so this shows a
  "no current openings" state that points applicants to Join Us.

## Structure
```
prachas-website/
├── index.html  about-us.html  services.html
├── join-us.html  contact-us.html  current-jobs.html
├── css/style.css      # all styling (design system + responsive)
├── js/main.js         # mobile nav, active-link, demo form handling
└── images/            # drop real logo/photos here (see images/README.txt)
```

## How to view
Double-click `index.html` — it opens in any browser. No server needed.

## How to host
Upload the whole folder to any static host: Netlify, Vercel, GitHub Pages,
AWS S3 + CloudFront, or normal web hosting / cPanel. No backend required.

## Notes for the developer
- **Branding:** colors are CSS variables at the top of `css/style.css`
  (`--navy`, `--blue`, `--teal`, `--accent`). Change once to re-theme everything.
- **Logo/images:** placeholders use CSS gradients + inline SVG so the site is
  self-contained. Replace with real assets in `images/` (see `images/README.txt`).
- **Forms** (Join Us, Contact Us) are front-end only — they show a success
  message but don't send anywhere yet. Wire them to email or a service like
  Formspree / Web3Forms, or your backend (set the `<form action=...>`).
- A single-file version of the whole site also exists at
  `../prachas-complete.html` (all pages + CSS + JS in one file).

## Why this instead of GoDaddy's export
GoDaddy's editor doesn't export portable source — its published output is
machine-generated, platform-locked markup that can't run or be edited outside
GoDaddy. This is a clean, standards-based equivalent any developer can read,
edit, and deploy on any host.
