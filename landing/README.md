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

The primary CTA uses the clean artifact name **GoBudget.apk**. The hero marketing dashboard is explicitly labelled as an illustrative preview; the product showcase uses frames from the supplied app recording.


## Reference-aligned edition

The landing page now follows the supplied black-morphism reference: sticky glass navigation, monochrome premium palette, bento feature grid, metrics strip, floating device chips, horizontally scrollable mobile screenshot cards, and polished download/FAQ sections. The screenshot cards use the supplied marketing-style assets (`m-dashboard.jpg`, `m-wallets.jpg`, `m-expense-form.jpg`, `m-settings.jpg`).


## Dynamic marketing screenshots

`marketing-preview.html` is the editable source for the populated preview set. It uses one consistent sample account across Dashboard, Wallets, Activity, Analytics and Settings, with matching USD totals, wallet balances, categories and recent transactions. The rendered `m-*.jpg` files are used by the landing page screenshot cards.
