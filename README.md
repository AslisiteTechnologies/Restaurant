# Maison Serein — Restaurant Portfolio Concept

An original fine-dining website concept for Aslisite Technologies. The restaurant, people, dishes, prices, opening hours, and location are fictional. Reservation, ordering, event, and contact interactions are browser-only demonstrations: no booking, message, purchase, payment, or delivery is processed.

## Stack

React 18, Vite, TypeScript, Tailwind CSS, Framer Motion, React Router, Zustand, and Lucide React. Cart and reservation demo state use Zustand persistence in local storage. There is no backend or secret configuration.

## Run locally

```bash
npm install
npm run dev
```

## Verify and build

```bash
npm run typecheck
npm run lint
npm test
npm run build
npm run preview
```

## Deployment

- **Build command:** `npm run build`
- **Output directory:** `dist`
- **Vercel:** use the Vite preset. `vercel.json` enables SPA route fallback.
- **Cloudflare Pages:** use the Vite preset. `public/_redirects` provides SPA route fallback.
- No domain is hardcoded; configure a subdomain such as `restaurant.demo.aslisite.com` in the hosting dashboard when ready.

The site uses Unsplash image URLs and Google Fonts, so those visuals need an internet connection. All images are lazy-loaded below the fold; Unsplash source URLs are used as remote demo assets. The project has no live API integrations, real address, real map pin, or production restaurant content.

## Routes

Homepage `/`, menu `/menu`, online ordering `/order`, dish details `/dish/:slug`, reservation `/reserve`, bag `/cart`, demo checkout `/checkout`, order confirmation `/order-confirmation`, story `/story`, chef `/chef`, gallery `/gallery`, private events `/events`, contact `/contact`, FAQ `/faq`, sample privacy `/privacy`, sample terms `/terms`, and a custom not-found page.
