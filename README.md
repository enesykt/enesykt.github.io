# Enes Yakut — Academic Website

Personal academic website built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

- **Current Live URL:** [https://enesykt.github.io](https://enesykt.github.io)
- **Future Custom Domain (Planned):** `enesyakut.com`

---

## Local Preview & Publishing

1. **Preview locally:**
   ```powershell
   quarto preview
   ```
2. **Publish changes to GitHub Pages:**
   ```powershell
   git add .
   git commit -m "Update website content"
   git push origin main
   quarto publish gh-pages --no-prompt --no-browser
   ```

---

## Future Task: Connecting `enesyakut.com` Custom Domain

When `enesyakut.com` is purchased:

1. Create a file named `CNAME` in the root directory (`C:\academic-website\CNAME`) containing:
   ```text
   enesyakut.com
   ```
2. Update `site-url` in `_quarto.yml` to `https://enesyakut.com`.
3. In the domain registrar's DNS settings, add GitHub Pages `A` records for `@`:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
   and a `CNAME` record for `www` pointing to `enesykt.github.io`.
4. Enable **Enforce HTTPS** in GitHub Repository Settings → Pages.

