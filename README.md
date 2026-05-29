# levi.dev — Website Files

## How to add your photo

1. Save your photo as `levi-hero.jpg` (the original) inside `images/photos/`
2. Also save a WebP version as `levi-hero.webp` in the same folder (you can convert free at https://squoosh.app — drag your photo, choose WebP, quality 82, download)
3. The site will automatically use the WebP version for speed and fall back to the JPG

The ideal photo size is **1000x1000px** or larger (square crop works best for the hero).

## How to add your social links

Open `index.html` and `es/index.html` and find the `sameAs` array in the JSON-LD block near the top. Add your profile URLs there, for example:

```json
"sameAs": [
  "https://levi.dev",
  "https://www.linkedin.com/in/YOUR_HANDLE/",
  "https://x.com/YOUR_HANDLE",
  "https://github.com/YOUR_HANDLE"
]
```

Also add a WhatsApp contact link in the contact section if you want one:
```html
<a href="https://wa.me/50300000000" class="contact-item">
```

## File structure

```
levi-dev-website/
├── index.html          — English homepage
├── es/
│   └── index.html      — Spanish homepage
├── images/
│   └── photos/
│       ├── levi-hero.jpg     ← place your photo here
│       └── levi-hero.webp    ← and the WebP version here
├── llms.txt            — AI-readable profile (short)
├── llms-full.txt       — AI-readable profile (full)
├── robots.txt
├── sitemap.xml
├── 404.html
└── .nojekyll
```

## Deployment

Next step: use the **cloudflare-pages-deploy** skill to push this folder to GitHub and deploy it on Cloudflare Pages with your `levi.dev` domain.

## Requesting changes

Send updated text or photos anytime and the site can be updated in minutes.
