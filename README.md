# Franch Events

Static one page site for Franch Events (Franch Enterprises): 360° booth hire, event videography, photography and editing in Gauteng.

Plain HTML and CSS in a single file, with a small bit of JavaScript for the sound toggles and the WhatsApp enquiry form. No build step, no dependencies. Fonts come from Google Fonts.

## Files

    index.html     the whole page
    assets/        photos, booth clips and their poster frames

## Run it locally

Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8000

## Put it on GitHub Pages

1. Create a repo and push these files to the root of the `main` branch.
2. Repo Settings, then Pages, then set Source to "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site goes live at `https://<user>.github.io/<repo>/` in a minute or two.

For a custom domain, add it under Settings, then Pages, then Custom domain, and point the domain's DNS at GitHub Pages.

## Things to change

- Phone, WhatsApp and email live in the header, hero, booking section, mobile bar and footer. Search `1805` and `1806` to find them all.
- Prices are in the `#packages` section.
- Booth clips are the six `assets/booth-clip-*.mp4` files. Each one has a matching `.jpg` poster frame that shows before the video loads. Keep replacements short and compressed, roughly 9 seconds at 432px wide, or the page gets heavy.
- The enquiry form has no server. It builds a WhatsApp message and opens wa.me, so nothing is stored anywhere.
