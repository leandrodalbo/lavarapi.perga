# Plan: Lavarapi website

How the site was built, step by step. For how to edit it, see `README.md`.

## Goal

A simple one-page website in Spanish for Lavarapi, a laundry in Pergamino. It should show what they do, the hours and address, and make it easy to get in touch by WhatsApp or phone.

## What we had

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
| 0 | Colors and fonts based on the logo, page in Spanish, page title | Style | Done |
| 1 | Nav bar + hero (welcome block) | Section | Done |
| 2 | Nosotros (about us), replacing "Our Story" | Section | Done |
| 3 | Servicios (services), replacing the menu: lavado, secado, planchado, retiro y entrega a domicilio | Section | Done. Prices and promos requested from the family. |
| 4 | Horarios y ubicación (hours and location) | Section | Done |
| 5 | Contacto (WhatsApp / call / Instagram), replacing "Reserve" | Section | Done |
| 6 | Footer + search-engine business data (Restaurant → laundry) | Section | Done |
| – | Cleanup: Spanish anchors, section labels, dotted-line color | Review | Done |
| 7 | Published at https://lavarapi.com | Release | Done |

For each step, the loop was:

1. Write a short spec (what changes and the exact texts).
2. Approve it.
3. Apply it.
4. Check it in the browser.
5. Fix anything that's off.

## Assumptions

- **WhatsApp:** both phone numbers have WhatsApp. Confirmed by the flyer. WhatsApp links: `wa.me/5492477611241` and `wa.me/5492477455395`.
- **Photo:** we don't have photos yet. The one photo spot (Nosotros) shows the pickup-and-delivery flyer (`image-passed-1.jpg`) until there's a real photo of the shop.
- **Prices:** unknown for now, so the services list shows "Consultar" instead of prices.

## Decisions

- **Tests:** none. Each section was specified, approved, applied and checked in the browser.
- **WhatsApp buttons:** open the chat with no ready-made message.
- **Pickup message:** said in the hero, Nosotros and the Servicios box, each time worded differently. Horarios and Contacto don't repeat it.

## Pending

- Prices or promos for the services list (requested from the family)
- The real story and names for Nosotros
- A real photo of the shop to replace the flyer
- **Git:** this folder isn't a repository yet. Should we run `git init`?
