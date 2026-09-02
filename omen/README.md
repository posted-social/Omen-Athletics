# Omen Athletics website

Single-page static site for Omen Athletics, a social wellness club in downtown St. Louis.

## Structure

```
index.html            The whole page: markup, CSS, and one small script
assets/img/           Photos (cropped and compressed from client creative)
assets/brand/         Full logo kit, black and white variants (transparent PNG)
favicon.png
.nojekyll             Tells GitHub Pages to serve files as-is
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

## Deploy with GitHub Pages

1. Create a new GitHub repository and push this folder to the `main` branch.
2. In the repo, open **Settings > Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. The site publishes at `https://<user>.github.io/<repo>/`. For a custom domain, add it under **Custom domain** and create a `CNAME` file containing the domain.

## Editing

- Prices, class times, and copy are plain HTML in `index.html`. Search for the section id: `#memberships`, `#schedule`, `#included`, `#visit`.
- Free-class buttons point to `https://lp.omenathleticsstl.com/`.
- The class schedule is the WellnessLiving widget in the `#classes` section. It only renders on a real host (not from `file://` in some browsers).
- Fonts: the CSS stack is Helvetica first, then Archivo from Google Fonts as the web fallback. Swap in a licensed Helvetica webfont if available.
- Brand files: every logo, tag, and icon ships as `-black.png` and `-white.png`. Use black on white/gray, white on black/orange. Don't mix logo variations (per the brand guide).
- Replace the compressed photos in `assets/img/` with higher-resolution originals when you have them, keeping the same filenames.
