# Everlyn Internationals — website

Luxury import & export website with a scroll-driven 3D story (cargo → crane → sunset departure → night globe → night arrival), built with Next.js 16, React Three Fiber, GSAP and Framer Motion.

## Requirements

- [Node.js](https://nodejs.org) **20.9 or newer** (22 LTS recommended)

## Run it on your computer

```bash
npm install
npm run dev
```

Then open http://localhost:3000.

## Production build

```bash
npm run build
npm start
```

## Deploy (recommended: Vercel, free)

1. Push this folder to a GitHub repository.
2. Go to https://vercel.com/new, sign in with GitHub and import the repository.
3. Keep the defaults (Framework: Next.js) and click **Deploy**.

Any host that runs Node.js works too (Netlify, Render, a VPS with `npm run build && npm start`).

## Where to edit things

| What | File |
| --- | --- |
| Company name, contact details, products, stats, testimonials, FAQs | `src/content/site.ts` (placeholders are marked `TODO`) |
| Home page 3D story timeline (camera, ship, sunset, night) | `src/lib/story.ts` |
| Home page text panels | `src/components/home/StoryPanels.tsx` |
| Loading screen | `src/components/home/Loader.tsx` |
| Other pages | `src/app/<page>/page.tsx` |
| Colours and fonts | `src/app/globals.css`, `src/app/layout.tsx` |
| Logo image | `public/brand/everlyn-logo.jpg` |

## Before going live

- Replace every `TODO` in `src/content/site.ts` (address, phone, email, WhatsApp, IEC/GST, social links, domain).
- Replace the sample stats, testimonials and certifications with real ones.
- Contact and quote forms currently log submissions on the server (`src/app/api/enquiry/route.ts`). Connect an email service (e.g. Resend) there to receive them by email.
- Have the Privacy Policy and Terms pages reviewed.

## Credits

Sky and material textures in `public/hdri` and `public/textures` are from [Poly Haven](https://polyhaven.com), CC0 (public domain).
