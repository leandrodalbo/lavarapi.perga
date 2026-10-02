# Plan: Lavarapi website

## Goal

A simple one-page website in Spanish for Lavarapi, a laundry in Pergamino. It should show what they do, the hours and address, and make it easy to get in touch by WhatsApp or phone.

## What we have

- **Template:** `index.html`, "The Copper Fig". It's a single page built with Tailwind, with no build step. Colors and fonts are set in one small config block near the top of the file.
- **Logo:** `logo.jpg`, 150×150. Sky blue, white bubbles, pink towels. The site colors come from it, with a dark navy (`#0f2a43`) for the dark backgrounds. We tried the flyer's royal blue (`#1a4fa0`): it clashed with the logo and made light blue text hard to read. The logo is used as the browser-tab icon only, not in the nav bar.
- **Visible name:** **Lavarapi** (not LavaRapi).
- **Business info** (from `info.txt`):
  - Monroe 532, Pergamino
  - 2477 611241 / 2477 455395
  - Monday to Friday 8–20 hs, Saturday 8–13 hs
  - "Servicio de lavandería en general" (general laundry service)
  - Instagram: lavarapi.perga
- **Flyers:** `image-passed-0.jpg` and `image-passed-1.jpg`. They add:
  - Name written "LavaRapi", tagline "Lavadero de ropa"
  - Services: lavado, secado y planchado (washing, drying, ironing)
  - Pickup and delivery: "Retiramos la ropa de tu casa y te la llevamos hasta la puerta"
  - WhatsApp on both numbers
  - A second logo (navy and sky-blue washing machine). We keep `logo.jpg` for the site.

## Constraints

- Keep the template's structure, layout and visual style.
- Work one section at a time, and ask before every change (see `TDCG/`).
- Where we don't have the content yet, use placeholder text marked with a `<!-- TODO -->` comment.

## Steps

| # | Step | Kind | Status |
|---|---|---|---|
| 0 | Colors and fonts based on the logo, page in Spanish, page title | Style: you confirm, then I apply | Done |
| 1 | Nav bar + hero (welcome block) | Section | Done |
| 2 | Nosotros (about us), replacing "Our Story" | Section | Pending |
| 3 | Servicios (services), replacing the menu: lavado, secado, planchado, retiro y entrega a domicilio | Section | Pending |
| 4 | Horarios y ubicación (hours and location) | Section | Pending |
| 5 | Contacto (WhatsApp / call / Instagram), replacing "Reserve" | Section | Pending |
| 6 | Footer + search-engine business data (Restaurant → laundry) | Section | Pending |

For each step, the loop is:

1. I write a short spec (what changes and the exact texts).
2. You approve it.
3. I apply it.
4. You check it in the browser.
5. We fix anything that's off.
6. Commit.

## Assumptions to confirm

- ~~Both phone numbers are mobiles with WhatsApp.~~ Confirmed by the flyer. WhatsApp links: `wa.me/5492477611241` and `wa.me/5492477455395`.
- We don't have photos yet. The one photo spot keeps its placeholder box until there's a real photo of the shop.
- Prices are unknown for now, so the services list either shows placeholder prices or no prices at all.

## Open decisions

1. **Tests:** should section changes just be approved by you, the same as style changes? Or do you want small automated checks per section (address, phones, links)?
2. **Git:** this folder isn't a repository yet. Should we run `git init` so each step can be committed?
