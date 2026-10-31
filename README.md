# 🖨️ Saabi Digital Cafe

Website for **Saabi Digital Cafe (CSC)**, Village Varpal, Amritsar — print, scan, xerox, online and government forms, PAN, voter ID, passport, PM Kisan, Ayushman card and more.

A single-page, animated website in **5 languages** (English, हिन्दी, ਪੰਜਾਬੀ, اردو, বাংলা). Plain HTML, CSS and JavaScript: no build step, no dependencies.

## ✨ Features

- 3D rotating cube hero that follows the mouse, floating digital symbols, typewriter of services
- Live **Open now / Closed now** badge (10 AM – 8 PM, India time)
- **Saabi Helper chatbot** 🤖 in all 5 languages: answers about services, documents usually needed, timings, location and how to contact, with Call and WhatsApp buttons
- **Meet your VLE** flip card (owner photo, CSC registration details), **documents and certificates** section, with tap-to-enlarge
- Service search box and a live **Open now** badge in the Visit us card
- 11 service cards with 3D tilt, shine, and an "Ask on WhatsApp" link that pre-fills the service name
- Animated map with moving traffic, Google Maps links
- Click confetti, cursor sparkle trail, scroll progress bar, animated silver-and-gold background
- Light / dark theme toggle, responsive layout, right-to-left support for Urdu, respects reduced-motion settings

## 🚀 Run locally

Open `index.html` in any modern browser (internet needed for the Google Fonts).

## 🌐 Publish free with GitHub Pages

1. Push this repo to GitHub (repo name suggestion: `saabi-digital-cafe`).
2. Open **Settings → Pages**.
3. Under **Build and deployment** choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and **Save**.
4. Your site goes live at `https://<your-username>.github.io/saabi-digital-cafe/` after a minute or two.

## ⚙️ Edit the content

Everything is in `index.html`:

| What | Where |
|---|---|
| Phone, WhatsApp, e-mail, address | search for|
| Text in the 5 languages | the `D` object near the bottom (`s1`…`s11` are the services) |
| Helper bot answers | the `B` object (replies), `DOC` and `SD` (documents per service) in the "HELPER BOT" script |
| Opening hours | the `stat()` function (`h>=10&&h<20`) and the bot's `hours` text |
| Colours | CSS variables at the top (`--blue`, `--sun`, …) and the "SILVER + GOLD BACKGROUND" block |

## 🤖 About the helper bot

The bot is **built into the page**: it matches keywords in the visitor's question and replies from the texts above. It needs no server, costs nothing and works on GitHub Pages, but it is **not a live AI model** and can only answer the topics it was written for. The documents it lists are the usual ones — the cafe should confirm current rules. A real AI chat would need a small backend to keep its API key secret.

## 📜 License

MIT — see [LICENSE](LICENSE).
