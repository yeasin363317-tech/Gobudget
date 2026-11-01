# GoBudget landing page

Premium responsive black-glass product landing page for GoBudget. It is a static HTML/CSS/JS site with no runtime dependencies.

## Files

- `index.html` — responsive landing page, accessible FAQ accordion, navigation, feature sections, privacy explanation and real APK CTA.
- `release.json` — verified version, APK size, Android minimum version and direct APK URL.
- `assets/` — real app frames extracted from the supplied screen recording and used as labelled product screenshots.

## Local preview

```bash
cd landing
python3 -m http.server 4173
```

Open `http://localhost:4173`.

## Vercel deployment

Create a Vercel project with the repository root set to `landing/`. Use no build command and set the output/publish directory to `.`. The direct APK CTA is configured in `index.html` and points to the verified standalone release artifact in `release.json`.

The page makes only claims supported by the current app: local-first core records, offline operation for everyday tracking, multiple wallets, transactions, budgets, savings goals, analytics, categories and settings. It explicitly explains that local data is not automatically encrypted or cloud-backed-up.
