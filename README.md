# Jewellery Shop Layout

A static educational / demo jewellery storefront: several HTML pages with responsive layout for mobile, tablet, and desktop.

## Design

Figma mockup: [Jewellery (no card)](https://www.figma.com/design/lsBAbtiBY7aNVy4UqSqjc6/Jewellery--no-card-?node-id=0-1&t=r9EsMmpUENf0ZCOX-1)

## Pages

- **Home** (`index.html`) — landing with promo sections and catalog previews.
- **Catalog** (`catalog.html`) — product grid; the filter link opens in a new tab.
- **Filter** (`filter.html`) — assortment filtering UI.
- **Login** (`login.html`) — sign-in form (email, password).

Cross-page navigation: home and catalog link to the login page; catalog links to the filter.

## Tech stack

| Tool | Role |
|------|------|
| HTML5 | Markup |
| [Tailwind CSS](https://tailwindcss.com/) (CDN) | Styling and responsive layout |
| Google Fonts: Cormorant Garamond, Poppins | Typography |

No build step or framework is required; a browser and network access for the CDN and fonts are enough.

## Responsive behavior

Tailwind breakpoints are used (`md:` and a custom `desktop:` breakpoint at **1366px**). Images under `img/` are provided with `-mobile`, `-tab`, `-desktop` (and similar) suffixes for different viewport widths.

## Run locally

1. Clone the repository or download the archive.
2. Open `index.html` in a browser **or** serve the project root with a simple static server (for example `npx serve` or your editor’s Live Server) so paths to `img/` resolve reliably.

## Repository layout

```
jewellery-shop-layout/
├── index.html      # home
├── catalog.html    # catalog
├── filter.html     # filter
├── login.html      # login
└── img/            # page assets (responsive variants)
```

## Purpose

This project is a layout reference for a jewellery shop UI. There is no backend or real authentication.