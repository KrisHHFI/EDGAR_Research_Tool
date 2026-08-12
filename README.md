# EDGAR Research Tool

A clean, fast dashboard that gives retail investors direct, filtered access to the SEC's EDGAR filing system — the same public database used by Wall Street professionals.

<img src="EDGAR Project Promo.png" width="1000"/>

<sub><i>Project Screenshot (12/07/2026)</i></sub>

---

## What It Does

The SEC requires every public company to file disclosures — earnings, insider trades, acquisitions, proxy votes, and more — through EDGAR. The problem is the raw site is hard to navigate. This tool solves that by organising the most investment-relevant filing types into a browsable dashboard, with each card linking directly to the live, filtered EDGAR feed for that form type.

Click any card and you land on the latest filings of that type — no account required, no paywall, just raw primary-source data.

You can also save **Favorite Companies** — type any company name and it's stored in your browser's local storage as a one-click tile that opens all of that company's EDGAR filings.

---

## Filing Categories

| Category | What's Included |
|---|---|
| ⚡ High-Signal / Time-Sensitive | 8-K, Form 3, Form 4, Form 5 |
| 🏦 Activist & Institutional | SC 13D, SC 13G, and their amendments |
| 📊 Company Financials | 10-K, 10-Q, and amended versions |
| 💸 Capital Markets & Dilution | S-1, S-3, 424B3, 424B4, Form 144, Form D |
| 🤝 M&A & Proxy | DEF 14A, DEFA14A, DEFM14A, SC TO-T |
| 🌍 Foreign Issuers | 20-F, 6-K |

Each card shows:
- The form name and a plain-English description
- An investor tip explaining why the filing matters
- A colour-coded signal badge: **Bullish**, **Bearish**, **Watch Closely**, or **Due Diligence**

---

## Favorites

At the top of the main content area, the **Favorites** section lets you save company names for instant access:

- Type a company name in the input and press **Enter** or click **Add**
- Each favorite renders as a tile that links directly to `https://www.sec.gov/cgi-bin/browse-edgar?company=<name>&action=getcurrent`
- Click the **×** on any tile to remove it
- Favorites are saved to `localStorage` and persist across sessions

---

## Live App

Hosted on Firebase: **https://sec-dashboard-4c3af.web.app**

---

## Behind the scenes features

### Components page

<img src="Components Page.png" width="1000"/>

---

## Tech Stack

- **React + TypeScript** — component logic and type safety
- **Vite** — instant dev server and fast builds
- **Tailwind CSS v4** — utility classes for all component styling
