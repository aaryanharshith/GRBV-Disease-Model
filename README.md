# GRBV Vineyard Spread Simulator

An interactive, browser-based agent model of grapevine red blotch virus (GRBV) spread by the three-cornered alfalfa hopper (*Spissistilus festinus*) across a 24 × 40-vine vineyard block.

## Features

- Daily simulation over 1–5 growing seasons
- Vector movement with along-row bias, seasonal population curve, and edge immigration
- Infection, latency, symptom onset, roguing, and insecticide controls
- Time scrubber, playback, and clickable timeline chart
- Click any vine to force it infected or healthy
- Clustering index compared against random mixing

## Project structure

```
grbv-vineyard-sim/
├── index.html      # The entire application (HTML, CSS, JavaScript)
├── vercel.json     # Vercel configuration and security headers
├── .gitignore
└── README.md
```

The site is a static page with no build step, no dependencies, and no external network calls.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy to Vercel from GitHub

1. Create a new GitHub repository and push this folder to it:

   ```bash
   git init
   git add .
   git commit -m "Initial commit: GRBV vineyard simulator"
   git branch -M main
   git remote add origin https://github.com/<your-user>/grbv-vineyard-sim.git
   git push -u origin main
   ```

2. Go to https://vercel.com/new, choose **Import Git Repository**, and select the repository.
3. Framework preset: **Other**. Build command and output directory can stay empty.
4. Click **Deploy**. Every push to `main` redeploys automatically.

## Notes on the model

Parameter defaults are illustrative and are not measured values for any specific vineyard. Literature anchors are cited on the page (Al Rwahnih et al., 2013; Sudarshana et al., 2015; Bahder et al., 2016) and should be verified against the primary sources before research use.

## License

Choose a license before publishing publicly (for example MIT).
