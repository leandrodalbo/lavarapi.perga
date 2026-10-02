# Lavarapi website

One-page website for Lavarapi, a laundry in Pergamino. Live at **https://lavarapi.com**.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site |
| `logo.jpg` | Browser-tab icon and logo for Google |
| `image-passed-1.jpg` | Flyer shown in the Nosotros section |
| `PLAN.md` | How the site was built, step by step |
| `TDCG/` | The working method (ask before every change, one section at a time) |
| `info.txt`, `image-passed-0.jpg` | Source material, not used on the site |

## How to edit

1. Open `index.html` in any text editor.
2. Find the section by its label: `NAV`, `HERO`, `NOSOTROS`, `SERVICIOS`, `HORARIOS`, `CONTACTO`, `FOOTER`.
3. Colors and fonts are in the `tailwind.config` block near the top of the file.
4. Upload the changed files to the hosting.

There's no build step. Open `index.html` in a browser to preview.

## Business data and where it appears

When something changes, update every place listed:

| Data | Where it appears in `index.html` |
|---|---|
| Phones | Hero WhatsApp button, Horarios, Contacto buttons, footer, Google info (`application/ld+json` at the bottom) |
| Hours | Hero figures, Horarios, page description (`<meta name="description">`), Google info |
| Address | Hero, Horarios, Contacto, footer, page description, Google info |
| Instagram | Horarios, Contacto, Google info |

## Pending

Marked with `<!-- TODO -->` in `index.html`:

- Prices or promos for the services list (now "Consultar")
- The real story and names for Nosotros
- A real photo of the shop to replace the flyer
