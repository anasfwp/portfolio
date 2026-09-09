# Anas Shabbir — Portfolio Site

Static single-page portfolio for Anas Shabbir, a full-stack software developer. No build step, no frameworks — just `index.html`, `style.css`, and `script.js`.

**Live:** https://anasfwp.github.io/portfolio/

## About me

Full-stack software developer working across Python/Django, PHP, C#/.NET, JavaScript, and AI/LLM application development (OpenAI/Gemini APIs, agent orchestration, RAG). I handle the whole lifecycle of a product — planning, development, deployment, and long-term maintenance — and have shipped e-commerce stores, booking platforms, custom WordPress plugins, AI agent/chatbot systems, and ERP deployments for clients in Pakistan, the UK, Malaysia, and beyond.

- **Email:** anasshabbir5332@gmail.com
- **WhatsApp:** +92 302 1931965
- **LinkedIn:** https://linkedin.com/in/anas-wordpress-dev

## Site sections

Home · Client Work · Products & Projects · Skills · About · Contact — all in one scrollable page, built for a 95+ PageSpeed score (no external fonts, no JS libraries, inline SVG icons only).

## Deploy to GitHub Pages

This repo is set up to serve directly from GitHub Pages:

1. Push `index.html`, `style.css`, `script.js`, and this `README.md` to the `main` branch (see commands below).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
5. GitHub will publish the site at `https://anasfwp.github.io/portfolio/` within a minute or two.

## Deploy to Hostinger (or any static host)

1. **Create the subdomain/domain folder**: In hPanel, go to **Domains → Subdomains** and point it at a folder such as `public_html/portfolio` (or use your root domain folder).
2. **Upload the files**: Use hPanel's **File Manager** (or an FTP client like FileZilla) to upload `index.html`, `style.css`, and `script.js` into that folder. Keep all three files in the same directory — do not put them in subfolders.
3. **DNS/propagation**: Subdomains created in hPanel are usually live within a few minutes. If it doesn't resolve right away, allow up to a few hours for DNS propagation.
4. **Verify**: Visit the live URL and check:
   - The Contact buttons open WhatsApp/email/LinkedIn correctly
   - The site loads over HTTPS (Hostinger issues a free SSL cert automatically — enable it under **SSL** in hPanel if it isn't active yet)
5. **Optional — cache headers**: Static hosting on Hostinger already serves these files efficiently; no extra configuration is required for good PageSpeed scores.

## Local preview

Just open `index.html` in a browser, or serve the folder locally:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Notes

- Dark theme, single accent color, system font stack — no external fonts or JS libraries, keeping load times minimal.
- All icons are inline SVG (no image requests).
- Tested responsive breakpoints: 360px, 768px, 1200px.
