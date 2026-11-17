# CleanPlate

CleanPlate is a static educational web-app prototype that helps users understand ingredient labels.

## Features
- Ingredient list analysis using a local rule-based dictionary and regular expressions
- Detection of selected sugar-related ingredients and selected food additives
- Plain-language explanations for recognized ingredients
- Three interface languages: English, Russian and Kazakh
- Sample ingredient lists
- Side-by-side ingredient comparison
- Responsive premium-style interface
- Ingredient text is processed in the browser; no backend or API key is required

## Run locally
Open `index.html` in a browser. For a local development server, use the VS Code Live Server extension or Python's built-in server:
```bash
python3 -m http.server 8000
```
Then open `http://localhost:8000`.

## Deploy to Vercel
1. Create a GitHub repository named `cleanplate`.
2. Upload `index.html`, `styles.css`, `app.js`, and `README.md` to the repository root.
3. Sign in to Vercel with GitHub.
4. Select **Add New → Project**, import `cleanplate`.
5. Framework Preset: **Other**. Root Directory: `./`. Build Command: leave empty. Output Directory: `./`.
6. Click **Deploy**. Vercel will provide a public URL.

## Important limitations
- The ingredient dictionary is a small demonstration dataset, not a complete food database.
- Ingredient matching is based on text patterns; packaging OCR, barcode lookup, and external product databases are not included.
- The numeric indicator is an illustrative ingredient-awareness indicator only. It is not a scientific nutrition score, safety rating, or medical recommendation.
- A listed ingredient does not reveal its quantity per serving. Ingredient order is generally based on weight at the time of addition, subject to local labelling rules.
- Regulatory rules differ by country. Verify additive permissions and product-specific information with reliable local sources.
- The app does not assess allergens comprehensively. Always check the package's allergen statement.

## Tech
HTML, CSS, vanilla JavaScript, regular expressions. No framework, server, API key, or build step required.
