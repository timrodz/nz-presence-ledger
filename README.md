# Presence Ledger

A working planner for tracking progress toward New Zealand citizenship eligibility. Log your trips outside NZ and see exactly how many days you can spend away while staying compliant with the citizenship presence requirements.

## Features

- **Easy trip logging** — Add trips by date picker or paste multiple dates at once
- **Eligibility tracking** — Real-time calculation against all three NZ citizenship rules:
  - 1,350 days present across the full 5-year window
  - 240 days present in each 12-month period
  - No more than ~4 months away in any rolling 12-month window
  - No more than ~15 months away total in the 5 years
- **Visual heatmap** — See your overseas time at a glance across the full 5-year window
- **Export & backup** — Copy trips as text to share or back up elsewhere
- **Completely private** — Data stored in browser only, nothing sent anywhere
- **No setup needed** — Single HTML file, no build process, works offline

## What it calculates

Based on [Immigration New Zealand's presence requirements](https://www.govt.nz/browse/passports-citizenship-and-identity/nz-citizenship/requirements-for-nz-citizenship/presence-requirements/):

- Days present in NZ during the last 5 years (counted backward from your application date)
- Each individual 12-month period to catch the 240-day minimum
- Your tightest rolling 12-month absence stretch
- Total overseas days against the 15-month guideline
- Your remaining overseas budget before hitting the 1,350-day threshold

Set your planned application date and add trips to see how much time you have left.

## Stack

- Single HTML file (no build process)
- Vanilla JavaScript (no frameworks)
- CSS custom properties for theming
- localStorage for client-side data persistence
- Google Fonts (Domine & Mona Sans)

## Usage

### Online
Open the live version at [your-github-username.github.io/presence-ledger](https://your-github-username.github.io/presence-ledger)

### Locally
Download `index.html` and open it in any modern browser. Works completely offline — all data stays in your browser.

### Adding trips

**One at a time:**
- Set a departure date and return date using the date pickers
- Click "Add trip"

**Bulk import:**
- Paste multiple dates in the format shown:
  ```
  2026-04-03 to 2026-04-06
  2026-08-14 to 2026-08-29
  ```
- Click "Add all lines"

**Export:**
- Click "Copy as text" to copy all your trips
- Paste into a text file to back up, or paste back into bulk-add to restore

## Important notes

- Trip length counts departure day through return day inclusive
- Immigration NZ's actual border-crossing day count may differ slightly — treat this as a planning tool
- The "4 months" and "15 months" limits use approximate day counts (122 and 456 days respectively) — confirm with INZ when you're close to applying
- If you moved to NZ after the start of your 5-year window, set your residence-granted date so only eligible days are counted
- Time spent overseas on Crown service for the NZ Government counts as time in NZ (don't log these as trips)

**Always confirm your actual eligibility with Immigration New Zealand before applying for citizenship.**

## Contributing

Found a bug? Have a feature idea? Feel free to open an issue or PR.

## License

MIT

---

Built for tracking NZ citizenship presence requirements. Data never leaves your browser.
