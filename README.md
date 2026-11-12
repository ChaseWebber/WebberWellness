# WebberWellness

The public site is [https://www.webberwellness.com](https://www.webberwellness.com). It is hand-written HTML and CSS: a home page, two legal pages, and a 404 page. This file describes the site, the brand, and how a change goes live.

## About

WebberWellness is the father-and-son team of Dr Chase Webber and Chad Webber.

- **Dr Chase Webber** is a naturopathic doctor, and the creator of Ask ANA and The Wellness Formula. The home page credits him with 35 years of wellness and natural medicine experience. The hero labels him Naturopathic Doctor and Author.
- **Chad Webber** is the creative and technical lead, qualified in creative design, VFX compositing and sound engineering.

The about section calls them “a father and son team” with “more than 35 years in the wellness world.”

## What the site offers

The home page leads with Ask ANA, then “Work with us”. That intro reads: “Consulting, retreats and coaching, shaped by The Wellness Formula.”

| Offer | How the page describes it | Contact |
| --- | --- | --- |
| Ask ANA | Advanced Naturopathic Assistant for everyday wellbeing. Details under [Ask ANA](#ask-ana). | [App Store](https://apple.co/4xN2mFh) |
| Spa and hospitality consulting | Selective collaborations: auditing of wellness and spa facilities, and development of new wellness centres. | drchase@webberwellness.com |
| Hetki sauna partnership | The authentic Finnish sauna experience for a home or retreat. WebberWellness represents Hetki in the Indian Ocean region. | chad@webberwellness.com |
| Retreats | Small-group retreats inspired by The Wellness Formula, planned for 2027, with personal guidance from Dr Chase. | drchase@webberwellness.com |
| Coaching | An online coaching programme for aspiring coaches and wellness professionals, so they can implement the Wellness Formula method with their clients. | drchase@webberwellness.com |
| Journal | Mindfulness, movement, nutrition, breathing, hydrotherapy, sleep and rejuvenation, published on Substack. | [wellnessformula.substack.com](https://wellnessformula.substack.com/) |

The page also includes a breathing guide (“Begin with a breath”) and a three-step “day with ANA”: sunrise Breath, morning Move, afternoon Mind.

YouTube: [https://www.youtube.com/@WebberWellness-DrChaseWebber](https://www.youtube.com/@WebberWellness-DrChaseWebber)

## Ask ANA

ANA is the Advanced Naturopathic Assistant. On the page the product is Ask ANA. Structured data names it “Ask ANA: Wellness AI” as well.

Every download button uses [https://apple.co/4xN2mFh](https://apple.co/4xN2mFh).

The page says the app is for iPhone, iOS 26+. Structured data says the operating system is “iOS 26.0 or later”, gives the App Store id `6740890338`, and includes a longer download URL that the buttons do not use: `https://apps.apple.com/us/app/ask-ana-wellness-ai/id6740890338`.

The closing section states the price in these words:

> Free to download, with 5 questions to ANA, 5 goals, and all the Wellness Guides, Blog and Daily Affirmations. Upgrade for $6.99/month or $49.99/year, both with a 7-day free trial.

Shorter lines elsewhere say “Free to download · 7-day free trial on Premium”. Under the day section that line adds “· iPhone, iOS 26+”. Structured data lists the Premium prices as 6.99 and 49.99 USD, each after a 7-day free trial.

The footer says wellness education supports informed choices and does not replace individual medical care, and that Ask ANA does not provide medical advice, diagnosis or treatment.

## Brand colours

Colours live as variables on `:root` in `styles.css`. Body text is `color: var(--navy)`.

| Colour | Variable | Hex in the stylesheet |
| --- | --- | --- |
| Navy | `--navy` | `#10243E` |
| Accent blue | `--blue` | `#2F8FEA` |
| Teal (Fresh Teal) | `--teal` | `#43b1b8` |

`#43b1b8` is the same colour as `#43B1B8`. The words “Fresh Teal” are not in the stylesheet. The variable is `--teal`.

Also on `:root`: `--green` `#76C277` (Food), `--orange` `#FFA944` (Move, and the dash before kickers), `--cream` `#F7F5EF` (footer, and the base breath-band fill, which `breath-band--navy` overrides on the live page), `--mint` `#EAF5F7` (header, hero, day section), `--soft` `#F5F8FA` (about and journal), `--line` `#CDE7F3` (card borders) and `--white` `#fff`. Roles, journal excerpts and the legal lines use `#3a536f`.

### How to use the colours

- Keep body copy in navy. Do not set body text in `#2F8FEA`. Blue is the keyboard-focus outline, the footer-link hover underline, the Mind pillar marker, and the fill of the 404 download button.
- On a teal background, use navy text. The header **Get the App** button (`.btn-teal`) and the eyebrow on the navy breath band already do this. Do not use white text on teal.
- White text is for navy backgrounds: the closing band, the breath band, navy buttons, and the “Begin with a breath” eyebrow.
- Buttons in `styles.css`:
  - `.btn-navy` — navy fill, white text. Used for “Back to the home page” on the 404 page.
  - `.btn-teal` — teal fill, navy text. Used for “Get the App” in the header.
  - `.btn-store` — `#2F8FEA` fill, navy text. Used only for the 404 download button.
  - `.btn-ghost` — transparent, navy border, navy text. On hover the fill turns navy and the text turns white. Used on the “Work with us” cards.

## Fonts

Headings are Montserrat. Body copy is Open Sans. Both files are self-hosted. No page loads Google Fonts.

| File | `@font-face` in `styles.css` |
| --- | --- |
| `fonts/montserrat.woff2` | `font-family: "Montserrat"`; `font-weight: 500 800`; `font-display: swap` |
| `fonts/open-sans.woff2` | `font-family: "Open Sans"`; `font-weight: 400 700`; `font-display: swap` |

The stacks are `--head: "Montserrat", system-ui, sans-serif` and `--body: "Open Sans", system-ui, sans-serif`. Headings use `font-weight: 700`. The home page, both legal pages and the 404 page preload both font files.

## Brand and copy rules

- Refer to ANA as **her**. The day section says “get her supportive response.”
- Her name is Advanced Naturopathic Assistant. The pillars section says: “ANA is built on Dr Chase’s Wellness Formula. Small, steady actions across Mind, Food, Breath, Move and Sleep.”
- The five pillars, in that order:
  - **Mind** — Notice. Breathe. Choose.
  - **Food** — Protein first. Colour next. Eat real.
  - **Breath** — Slow. Gentle. Rhythmic.
  - **Move** — Move more. Sit less. Stay strong.
  - **Sleep** — Rest. Repair. Renew.
- She is an assistant: an educational wellness assistant. Do not call ANA a doctor. Dr Chase is the naturopathic doctor.
- Do not make medical claims. Keep the meaning of the footer: Ask ANA does not provide medical advice, diagnosis or treatment.
- Describe the app as iPhone, iOS 26 or later. Do not mention iPad or Android.
- “Get-Real Wellness” is a retired name. Do not use it.

## File and folder structure

```
.
├── index.html                     Home page
├── privacy-policy.html            Privacy policy for the app
├── terms-conditions.html          Terms for the app
├── 404.html                       Unknown-URL page
├── styles.css                     All layout and brand CSS
├── CNAME                          Custom domain: www.webberwellness.com
├── robots.txt                     Crawler rules and the sitemap URL
├── sitemap.xml                    Public page URLs
├── favicon.ico                    Root icon at 16, 32 and 48 px
├── fonts/
│   ├── montserrat.woff2           Heading font
│   └── open-sans.woff2            Body font
├── img/                           Web-ready images for the live site. See below.
│   ├── journal/                   mind.webp, food.webp, sleep.webp (800×450)
│   └── pillars/                   mind, food, breath, sleep as WebP; move.svg
├── images/                        Originals kept for possible later use.
│   └── icons/                     appstore, instagram, substack, x and youtube SVGs
└── .github/workflows/static.yml   GitHub Pages deploy
```

Chase’s rule: `images/` is a resource folder for original images we might use later. Correctly sized, web-ready versions go in `img/` for the live site (WebP, sized as in [Adding or replacing images](#adding-or-replacing-images)). Pages only ever reference `img/`.

`images/` currently holds `appstore_black.png`, `banner.png`, `favicon-chrome-512x512.png`, `hetki_sauna.jpg`, `hospitality_consult.png`, `phone1.png` through `phone6.png`, and `icons/` (`appstore.svg`, `instagram.svg`, `substack.svg`, `x.svg`, `youtube.svg`).

The deploy workflow publishes the whole repository, so files in `images/` are publicly reachable.

Two files in `img/` are not referenced by any page: `phone1.webp` and `phone6.webp`.

## Pages and URLs

| URL | File | Role |
| --- | --- | --- |
| `/` | `index.html` | Home page. `lang="en-GB"`. |
| `/privacy-policy.html` | `privacy-policy.html` | Privacy policy. Last updated 22 September 2026. |
| `/terms-conditions.html` | `terms-conditions.html` | Terms. Last updated 22 September 2026. |
| Any unknown path | `404.html` | Served by GitHub Pages. `noindex`. Not listed in the sitemap. |

**Leave `/privacy-policy.html` and `/terms-conditions.html` exactly as they are.** The App Store listing links to those URLs. Renaming or moving either file breaks that listing. The home footer and the 404 page already point at those root paths.

On the legal pages the product is still called the “Wellness app” (the terms also say “Wellness App”), and the provider is named Dr CHASE WEBBER. Both pages give the contact drchase@webberwellness.com. Their `lang` is `en`. Their CSS and image links are relative (`styles.css`, `img/...`), which works because the pages sit at the site root.

## Home-page sections and anchors

| Anchor | What it is |
| --- | --- |
| `#top` | Hero. “Live life well. A wiser approach to wellbeing.” App Store badge and Dr Chase’s photo. |
| `#breath` | “Begin with a breath”, including the breathing guide. |
| `#day` | “A day with ANA”: 06:30 Breath, 07:30 Move, 17:30 Mind. Header: “A day with ANA”. |
| `#pillars` | The Wellness Formula and the five pillars. Header: “The Formula”. |
| `#about` | “Meet the team”. Linked as “About” from the legal pages and the 404 page. |
| `#work` | Spa consulting, Hetki, retreats, coaching, and a journal card. Header: “Work with us”. |
| `#journal` | Three latest Substack posts. Header: “Journal”. |
| `#get-ana` | Closing download block and the full pricing line. Linked as “App” from the legal pages and the 404 page. |

Other ids, for the interface rather than the menu: `#main` (skip link), `#nav` (the menu), `#breath-anim`, `#breath-live`, `#breath-pause`, and `#journal-card` (the journal card inside `#work`).

The header **Get the App** button goes to the App Store, not to `#get-ana`.

## Hosting and deployment

GitHub Pages serves the site from the `main` branch. `.github/workflows/static.yml` runs on a push to `main`, and when someone starts it by hand. It checks out the repository, uploads the whole tree, and deploys that tree. There is no framework and no build step. The CSS file itself is marked as hand-written.

`CNAME` contains `www.webberwellness.com`.

- Every change goes through a pull request. Chase reviews it and merges it. Do not push straight to `main`.
- The domain and DNS are at GoDaddy. Do not change DNS unless Chase asks. Zoho email depends on those records.

## SEO

`robots.txt` allows every crawler and names `https://www.webberwellness.com/sitemap.xml`.

`sitemap.xml` lists three URLs:

- `https://www.webberwellness.com/` with `<lastmod>2026-11-05</lastmod>`
- `https://www.webberwellness.com/privacy-policy.html` (no `lastmod`)
- `https://www.webberwellness.com/terms-conditions.html` (no `lastmod`)

When a listed page changes, update its `lastmod`. When you add a public page, add a `<url>`. Keep `404.html` out of the sitemap.

`index.html` has a meta description, a canonical URL (`https://www.webberwellness.com/`), Open Graph tags (type, site name, title, description, url, image, image width 1200, image height 630, and image alt), a Twitter large-image card, and JSON-LD for the app, for Dr Chase Webber, and for the WebberWellness organisation. `theme-color` is `#10243E`.

The preview image is `img/og-image.jpg`, 1200×630, about 99 KB. WhatsApp and LinkedIn keep a cached preview for days. LinkedIn Post Inspector refreshes the LinkedIn cache.

## Favicon and the 404 page

| File | Pixels | Use |
| --- | --- | --- |
| `favicon.ico` | 16×16, 32×32 and 48×48 | At the site root. No HTML file links it. Browsers ask for `/favicon.ico` themselves. |
| `img/favicon-64.png` | 64×64 | `<link rel="icon">` on every page. |
| `img/apple-touch-icon.png` | 180×180 | `<link rel="apple-touch-icon">` on every page. |

GitHub Pages uses `404.html` for an unknown URL, including a nested path such as `/a/b`. Links in that file are root-absolute (`/styles.css`, `/fonts/...`, `/img/...`, `/`, `/privacy-policy.html`, `/terms-conditions.html`, `/index.html#get-ana`), so the page still loads its CSS and images from a nested path. It sets `<meta name="robots" content="noindex">`. “Back to the home page” is `.btn-navy`. “Download Ask ANA on the App Store” is `.btn-store`.

## Adding or replacing images

Save page images as WebP in `img/`. Files that are already not WebP, and should stay that way, are `img/og-image.jpg`, `img/app-store-badge.png`, the two favicon PNGs, and `img/pillars/move.svg`. When you replace a picture that a page already uses, keep the file name so the HTML does not need an edit.

`.card img` sets `aspect-ratio: 16/10` and `object-fit: cover`, so card photos should be about 16:10. Today those are `hospitality.webp` at 1000×600 (about 96 KB) and `hetki-sauna.webp` at 1000×596 (about 136 KB). Journal cards use `aspect-ratio: 16/9`; the three files in `img/journal/` are 800×450. The pillar WebP files are 800×800. Move is `img/pillars/move.svg`. The hero crop is square: `chase-hero.webp` is 900×900. Phone screens display at about 240 pixels wide (`min(240px, 70%)`).

Aim for under about 200 KB a picture. `chase-hero.webp` is the current file over that line, at about 266 KB.

Give every `<img>` a `width` and a `height`, and alt text that describes the picture. The logo, the pillar art and the journal thumbnails currently use empty alt, because the heading beside them carries the words.

Some attributes do not match the pixels in the file. After a replacement, set `width` and `height` to the new pixel size.

| File | Pixels in the file | `width` and `height` in `index.html` |
| --- | --- | --- |
| `img/phone3.webp` | 645×1332 | 600×1239 |
| `img/phone4.webp` | 645×1332 | 600×1239 |
| `img/dr-chase.webp` | 720×720 | 720×719 |
| `img/ana-icon.webp` | 320×320 | 120×120 |
| `img/ww-mark.webp` | 192×191 | 40×40, the size it is shown at |
| `img/app-store-badge.png` | 499×167 | 180×60 |

`img/phone5.webp` (600×1239), `img/chad.webp` (720×654) and `img/og-image.jpg` (1200×630) already match the numbers in the HTML.
