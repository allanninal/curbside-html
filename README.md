# Curbside: a free HTML website template for food trucks

<p align="center">
  <a href="https://www.allanninal.dev/templates/food-truck/"><b>View the live demo</b></a>
  &nbsp;&middot;&nbsp;
  <a href="https://checkout.freemius.com/theme/43083/plan/75012/"><b>Get the WordPress version</b></a>
</p>

<p align="center"><img src="screenshots/home-desktop.webp" alt="Curbside: home, desktop" width="420"> <img src="screenshots/home-mobile.webp" alt="Curbside: home, mobile" width="180"> <img src="screenshots/menu-desktop.webp" alt="Curbside: menu, desktop" width="420"> <img src="screenshots/journal-desktop.webp" alt="Curbside: journal, desktop" width="420"></p>

Curbside is a free, plain-HTML website for a food truck. Open `index.html` and it works: no build step, no framework, no account. Edit the text in any editor and upload the folder to any web host.

## What's inside

- **Hero** — a photo of smoke over the grill, a quick look at the next three stops, two calls to action
- **This week's schedule** — seven day cards with place, neighbourhood, time, address, a note and a Directions link; an "updated" date, an optional cancellation banner, an Add to calendar file (`/schedule.ics`) and schema.org `Event` data for each stop
- **Menu** — three tabs (Tacos, Sides & Extras, Drinks) with prices and dietary tags (gluten-free, vegan, dairy-free, spicy, bestseller, new), plus a "Contains" allergen line on every item (US nine and coconut) and the allergy notice
- **Menu page** — the whole menu on one printable page
- **Where to find us** — phone, email, social links
- **Book the truck** — three catering packages, an inquiry form (event, date, service window, headcount, address, parking and power, budget, dietary needs) and a custom-quote band
- **Pre-order** — text and a link-out button to your own ordering page (`truck.orderUrl`)
- **Our story** — the pitmaster's story and a stats band
- **Gallery** — six photographs with descriptive alt text
- **Journal** — three posts and their pages
- **Contact** — a plain form that opens the visitor's email app (no back end)
- **Photo credits** — footer block, removable once you swap the photos
- **Schema.org JSON-LD** — `FoodEstablishment` and `Menu`
- Self-hosted fonts, no trackers, no analytics, no external scripts.
- Works from `file://` and from any host or sub-folder: every link is relative.

## Quick start

1. Download or clone this repository.
2. Open `index.html` in your browser. That is the whole site.
3. Edit the `.html` files in a text editor and reload.

```bash
git clone https://github.com/allanninal/curbside-html.git
cd curbside-html
open index.html        # macOS; on other systems double-click the file
```

## Customise

- **Text:** open the page (`index.html`, `menu/index.html`, `journal/index.html`, `contact/index.html`) and edit it. The business details in the demo (name, address, phone, email, hours, owner or chef) are made up; search for them and replace every one, including the `ld+json` block in `index.html`.
- **Colours and type:** the stylesheet in `assets/` starts with CSS variables (`--color-*`). Change them in one place.
- **Photos:** replace the files in `images/` with your own, keeping the names or updating the pages. Then delete the `<details data-photo-credits>` block from the footer of each page.
- **Placeholder address:** the pages carry `https://example.com/` in the canonical and social-card tags. Replace it with your domain.
- **Contact form:** it has no back end. As shipped it opens the visitor's email app. To receive messages from the page itself, point the form's `action` at a form service (Formspree, Formspark, Web3Forms, Netlify Forms) and follow that service's instructions.

## Deploy

It is a folder of static files, so any static host works.

- **GitHub Pages:** Settings, Pages, deploy from a branch, `main`, `/ (root)`.
- **Netlify or Cloudflare Pages:** drag the folder in, or connect the repository. No build command; publish directory is the repository root.
- **Any web host:** upload the folder with FTP or your host's file manager.

## Measured scores

Lighthouse mobile, this folder served as static files, median of three runs (11 November 2026):

| Page | Performance | Accessibility | Best practices | SEO |
|---|---:|---:|---:|---:|
| Home | 92 | 100 | 100 | 100 |
| Menu | 100 | 100 | 100 | 100 |
| Journal | 91 | 100 | 100 | 100 |
| Contact | 100 | 100 | 100 | 100 |

Your scores will vary with your host and photos.

## Licence

- **Code:** MIT, see [LICENSE](LICENSE).
- **Photographs:** not MIT; each is under its source's licence, see [CREDITS.md](CREDITS.md). Replace them with your own before launch.
- **Fonts:** SIL Open Font License 1.1, see [`licenses/`](licenses/).

## Want it on WordPress?

Curbside is also a WordPress block theme: one click imports the demo, and everything stays editable in the editor. [Get the WordPress version](https://checkout.freemius.com/theme/43083/plan/75012/). The HTML edition here stays free either way.

## Support

If this saved you time, you can [tip on Ko-fi](https://ko-fi.com/allanninal). It is optional and appreciated.
