# axentra – interactive flower-field scene

A single-page website: a girl turns and walks toward the sunlight, glowing butterflies circle around her, the plants sway with the wind and follow your cursor, and a built-in beat plays when you press **Play**.

## What is inside

| File | Purpose |
| --- | --- |
| `index.html` | The whole site. Self-contained: images, styles and scripts are inside this one file, so it also works when you double-click it. |
| `source-layers/` | The separate image layers (background, girl, front plants) in case you want to edit them. They are already embedded in `index.html`. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

## Run it locally

Open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari). WebGL is required.

## Put it on GitHub

```bash
cd axentra-site
git init
git add .
git commit -m "Add axentra interactive site"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

Then, on GitHub, go to **Settings → Pages**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save. Your site will appear at `https://<your-username>.github.io/<your-repo>/` after a minute or two.

## Notes

- Sound only starts after a click on Play (browsers block autoplay).
- The music is generated in the browser with the Web Audio API, so there are no audio files.
- Motion is reduced for visitors who have "reduce motion" turned on.
