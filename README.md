<p align="center">
  <img src="./assets/runea-icon.png" alt="Runea icon" width="120" height="120">
</p>

<h1 align="center">Runea</h1>
<p align="center"><em>Run your business in one place.</em></p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-landing--page-a7ef35?style=flat-square&labelColor=193b31">
  <img alt="Type" src="https://img.shields.io/badge/type-static%20HTML-a7ef35?style=flat-square&labelColor=193b31">
  <img alt="License" src="https://img.shields.io/badge/license-unlicensed-lightgrey?style=flat-square">
</p>

---

## 📖 About the Project

**Runea** is billed as the *"calm operating system"* for independent businesses — a product concept that brings invoices, quotes, proposals, project management, expenses, and cashflow together into a single, calm workspace.

This repo contains a **static landing page** (single-file HTML) for the Runea product: a full marketing page with a hero section, feature list, dashboard showcase, testimonials, pricing, FAQ, and login/waitlist modals — all built with plain HTML, CSS, and vanilla JavaScript, with no framework or build step.

> This page is a **demo/template** — form buttons (login, waitlist, contact) are not wired up to a real backend.

---

## ✨ Page Features

The landing page tells the full Runea product story across several sections:

| Section | Description |
|---|---|
| 🏠 **Hero Section** | Headline, CTAs, and an animated mockup of the product dashboard |
| 🧭 **Navigation** | Responsive navbar with a feature dropdown menu and a mobile menu |
| 🧩 **Feature Grid** | 9 colorful feature cards: Invoices, Quotes, Proposals, Projects, Tasks, Customers, Expenses, Cashflow, Dashboard |
| 📊 **Insight/Calm Section** | Stats and a compact "insight board" chart on a dark background |
| 🆕 **Product Updates** | Timeline of the latest product updates |
| 🏢 **About Section** | A short story about the studio behind Runea |
| 💬 **Testimonials** | Customer review cards with a carousel |
| 💰 **Pricing** | 3 pricing tiers (Starter, Studio, Collective) with a monthly/yearly toggle |
| ❓ **FAQ** | Accordion of frequently asked questions |
| 📣 **Final CTA & Footer** | Closing call-to-action plus a footer with social links |
| 🍪 **Cookie Banner** | Cookie consent banner with a preferences option |
| 🪟 **Modals** | Login, Waitlist/Request Demo, Contact, Help Centre, and Privacy Notice modals |

### 🖼️ Product Features Showcased

- **Invoices** — Create, send, and track beautiful invoices that get paid on time.
- **Quotes** — Turn a good idea into a clear quote clients can say yes to.
- **Proposals** — Make the case for your best work with personal proposals.
- **Projects** — Keep every deliverable, deadline, and detail in one view.
- **Tasks** — Know what's next, what matters, and what can wait.
- **Customers** — Build a thoughtful record of the people and businesses you serve.
- **Expenses** — Capture costs as they happen, in real time.
- **Cashflow** — Understand your finances without building another spreadsheet.
- **Dashboard** — Start the day with an honest, calm picture of your business.

---

## 🛠️ Tech Stack

This project is **100% static** — no build step or external dependencies required to run it:

- **HTML5** — single-file semantic structure (`index.html`)
- **Pure CSS3** — custom properties (CSS variables), grid & flexbox, animations/transitions, responsive design via media queries
- **Vanilla JavaScript (ES6+)** — UI interactions: dropdown menu, mobile nav, FAQ accordion, testimonial carousel, pricing toggle, and open/close logic for every modal
- **Google Fonts** — `DM Sans`, `DM Mono`, `Space Grotesk`
- **Structured Data (JSON-LD)** — `SoftwareApplication` schema for SEO
- **Open Graph & Twitter Card** — metadata for social link previews

No framework (React/Vue/etc.), bundler, or package manager is used — just open the HTML file in a browser.

---

## 📁 Project Structure

```
.
├── index.html          # Main page (markup + CSS + JS in a single file)
├── runea-icon.png       # Favicon / app icon
├── runea-logo.png       # Logo used in metadata (Open Graph/JSON-LD)
├── og-image.jpg          # Open Graph preview image (1200x630)
└── README.md              # This documentation
```

> Note: the image files (`runea-icon.png`, `runea-logo.png`, `og-image.jpg`) are referenced inside the HTML but need to be added to the project root yourself for the favicon and social previews to display correctly.

---

## 🚀 Getting Started

Since this is a static page, no installation is required.

**Option 1 — Open directly**
```bash
# Just open the file in your browser
open index.html      # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

**Option 2 — Run a local server (recommended so relative paths behave)**
```bash
# Using Python
python3 -m http.server 8000

# then open
http://localhost:8000
```

**Option 3 — VS Code Live Server**
Open the project folder in VS Code, right-click `index.html` → **Open with Live Server**.

---

## 🎨 Design & Color Palette

The landing page uses a calm green theme inspired by natural, minimalist tones:

| Color | Hex | Usage |
|---|---|---|
| 🟢 Deep Green | `#193b31` | Primary dark color (header, footer, contrast sections) |
| 🟩 Green/Lime | `#a7ef35` / `#82c62d` | Accents, buttons, highlights |
| ⚪ Paper | `#f7f8f3` | Main background |
| ⚫ Ink | `#17221e` | Primary text color |
| 🩶 Muted | `#75807b` | Secondary text |
| 🍑 Peach / 🔵 Blue / 🟡 Yellow | `#f5d7bf` / `#d4e8ee` / `#f5edbb` | Feature card colors |

Typography combines **Space Grotesk** (headlines, large display text), **DM Sans** (body copy), and **DM Mono** (small code-like kicker labels).

---

## 📱 Responsiveness & Accessibility

- Fully **responsive** layout with a main breakpoint at `800px` (navigation switches to a mobile menu, grids collapse to a single column).
- Interactive elements use ARIA attributes (`aria-expanded`, `aria-modal`, `role="dialog"`, `role="menu"`) to support screen readers.
- Keyboard navigation support: the **Esc** key closes any open modal or menu.
- Clear focus states via `:focus-visible` with a lime-colored outline.

---

## 🧩 Interactive Components (JavaScript)

The script at the bottom of the page handles:
- Toggling the **feature menu** in the navbar and the **mobile menu**
- **FAQ accordion** (open/close questions)
- **Testimonial carousel** (scrolling review cards)
- **Billing toggle** between monthly/yearly pricing
- **Login**, **Waitlist/Request Demo** (with a success view after submit), **Contact**, **Help Centre**, and **Privacy Notice** modals
- **Cookie banner** with a preferences option
- Closing any overlay via its close button, clicking outside the modal, or the Esc key

> All forms in this demo trigger a simulated `alert()` and **do not send data to any server**.

---

## 🔍 SEO & Metadata

The page ships with production-ready metadata:
- Meta description, keywords, and canonical URL
- Full Open Graph & Twitter Card tags for social link previews
- JSON-LD structured data of type `SoftwareApplication` (including `AggregateOffer` pricing info)
- Multi-size favicon plus `apple-touch-icon`

---

## 📄 License

Not yet specified. Add a `LICENSE` file as needed before publishing or using this project commercially.

---

<p align="center">
  <img src="./assets/runea-icon.png" alt="Runea" width="28" height="28" valign="middle">
  <b>runea</b> — the calm operating system for independent businesses.
</p>
