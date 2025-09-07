# Autodiff4Astro Demos

Interactive, self-contained demos to embed as iframes in slides.com for a lecture on automatic differentiation. Hosted via GitHub Pages.

## GitHub Pages

- Enable Pages: Settings → Pages → Deploy from branch → `main` / root.
- The site will be available at:
  - Project page: `https://eiffl.github.io/Autodiff4Astro/`

All links in this repo use relative paths so they work on project pages.

## Structure

- `index.html` — landing page that lists demos.
- `demos/derivative-definition/` — first animation illustrating the definition of a derivative with a live secant→tangent visualization.

## Embedding in slides.com

Use an iframe block in your slide and point to the demo page. Example:

```
<iframe src="https://eiffl.github.io/Autodiff4Astro/demos/derivative-definition/"
        width="100%" height="520" style="border:0;" allow="fullscreen"></iframe>
```

Adjust `height` to fit your slide layout. The content is responsive and scales with the iframe size.

## Adding new demos

1. Duplicate `demos/derivative-definition` as `demos/<your-demo>/`.
2. Update the `<title>` and page copy inside your new `index.html`.
3. Keep all assets self-contained in the demo folder.
4. Add a link card to the root `index.html`.

## Local preview

You can open the HTML files directly in a browser, or serve locally.

```bash
python3 -m http.server 8000
# Then open http://localhost:8000/
```

License: see `LICENSE`.
