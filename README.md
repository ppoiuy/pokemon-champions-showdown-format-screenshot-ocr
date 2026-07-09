# Pokemon Champions Showdown Format Screenshot OCR

Convert Pokemon Champions team detail screenshots into Pokemon Showdown import text.

Live site: https://ppoiuy.github.io/pokemon-champions-showdown-format-screenshot-ocr/

## Usage

1. Open the site.
2. Take your screenshots:
   - From the Pokemon Champions home page: **Train** → **Replica Teams** → **Share Your Battle Teams** → choose a team → **View Details**
   - Screenshot the **Moves & More** tab (shows all 6 Pokemon)
   - Screenshot the **Stats** tab (shows all 6 Pokemon)
3. Upload both screenshots.
4. Enter your Gemini API key.
5. Click **Import screenshots**.
6. Review the results in the Team Editor and fix any OCR mistakes.
7. Copy the generated Showdown paste from the export panel.

## Gemini API Key

A Gemini API key is required.

Get a free API key from Google AI Studio:
https://aistudio.google.com/app/apikey

The app persists your key locally when **Save key** is enabled.

## Toggles

- **Auto-format Mega** — automatically rewrites species to the Mega form and swaps the ability when a Mega stone item is detected
- **Fuzzy match** — corrects close OCR misspellings against the Showdown dataset using Levenshtein distance
- **Form lookup** — asks Gemini to identify the Pokemon sprite and return the correct form name (Rotom-Wash, Lycanroc-Midnight, etc.)

## Privacy

- Your API key is stored in your browser's local storage when saved.
- Screenshots are sent to Google's Gemini API for OCR processing.
- No data is stored on any server.

## Validation

The app shows warnings for invalid species, items, abilities, moves, natures, or stat point totals. Validation uses Pokemon Showdown data as a baseline.
