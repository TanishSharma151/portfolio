# Portfolio: Tanish Raj Sharma

Interactive 3D portfolio for freelance work: operations software for multi-branch retailers.
A static site (plain HTML, CSS and JavaScript, Three.js included in `vendor/`). There is no build step.

## Run it locally

```bash
npx serve . -l 5070
```

Then open http://localhost:5070.

## Folders

| Path | What it is |
|---|---|
| `index.html` | The whole site (styles and script inline) |
| `img/` | Project screenshots, each in 4 sizes (full, 1100, 560, 360 px) |
| `fonts/`, `vendor/` | Self-hosted fonts and Three.js |
| `Tanish_Raj_Sharma_Resume.docx` | Résumé download |
| `_headers`, `vercel.json` | Cache rules for Cloudflare Pages / Vercel |

## Features that stay off until a value is set

Near the top of the script in `index.html`:

| Variable | Feature |
|---|---|
| `FORM_KEY` | Contact form delivery ([Web3Forms](https://web3forms.com) access key). Until set, the form opens the visitor's email app. |
| `CF_TOKEN` | Cloudflare Web Analytics token (anonymous, cookie-free visit statistics) |
| `BOOK_URL` | Cal.com / Calendly link for a "Book a call" button |
| `CHAT_URL` | Address of the chat Worker. Until set, the chat answers from built-in text. |

## Notes

- Screenshots of the Sales Tracker and Operations Suite use made-up demo data. The storefront screenshots are of a staging site.
- The AI chat Worker (Cloudflare Worker + Groq) is kept in a separate folder and is not part of this site.
