# United Hope Foundation – Static Web Experience

This project is a polished single-page experience for a fictional non-profit. It combines a marketing landing page, modal flows (login, campaign creation, donation), and a stats dashboard, all powered by handcrafted HTML/CSS/JS—no build tooling required.

## Highlights
- Immersive hero carousel and featured campaign cards rendered from `campaignData`.
- Interactive donation flow with preset/custom amounts, payment selection UI, confetti celebration, and mock success step.
- Login and “Start a Campaign” modals with modern form styling plus file-upload affordances.
- Analytics/dashboard overlay featuring stat cards and two Chart.js visualizations.
- Fully responsive layout with rich animations, gradients, and Font Awesome iconography defined in `style.css`.

## Project Structure
- `index.html` – markup, campaign data, and all interactive logic (carousel, modals, donation handling, dashboard setup).
- `style.css` – responsive layout system, utility classes, animations, modal/dashboard styling, and theming tokens.

## Getting Started
1. Install dependencies (served via CDN):
   - Font Awesome 6.4
   - Chart.js (loaded from `cdn.jsdelivr.net`)
2. Open `index.html` in any modern browser.  
   - For smoother development, use a lightweight HTTP server (e.g., VS Code Live Server, `python -m http.server`, or `npx serve`).

## Customization Tips
- **Campaigns**: Update the `campaignData` array in `index.html` to change stories, progress, and imagery.
- **Branding**: Adjust CSS variables at the top of `style.css` to retheme colors, typography, and spacing.
- **Charts**: Modify `initializeDashboardCharts()` in `index.html` to feed real analytics or adjust datasets.
- **Assets**: Replace carousel backgrounds and card imagery with organization-specific visuals.

## Browser Support & Testing
- Optimized for evergreen browsers (Chrome, Edge, Firefox, Safari). No polyfills included; add them if you must target legacy browsers.
- Since logic is entirely client-side, recommended testing steps:
  - Exercise each modal (login, campaign, donation, success).
  - Validate CTA anchors and smooth scrolling.
  - Resize viewport to confirm responsive layouts.
  - Reopen dashboard multiple times to ensure Chart.js instances are destroyed/recreated cleanly.

## Deployment
Because the site is static, you can deploy via any static host (GitHub Pages, Netlify, Vercel, S3, etc.). Upload both files as-is; no build step is required.

