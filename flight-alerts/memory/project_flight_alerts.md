---
name: project-flight-alerts
description: Flight alert app that monitors Google Flights for cheap European weekend trips and emails results
metadata:
  type: project
---

Built a flight alert tool in `flight-alerts/` (separate from the Mitchell Website).

**What it does:** Searches Google Flights (via `fast-flights` Python lib) for round-trip flights under $200, departing Thu evening and returning by Mon 6am, from BOS/BDL/JFK/LGA/EWR to 25 European airports, up to 12 weeks ahead. Emails deals to elliemariemitchell1@gmail.com from elliesawesomeflights123@gmail.com.

**How it runs:** GitHub Actions cron — twice daily (9am and 9pm ET). User runs it manually via "Run workflow" for testing.

**Why:** Free trip finder for weekend Europe trips.

**How to apply:** If revisiting this project, the files are in `flight-alerts/`. The Gmail App Password is stored as a GitHub Secret named `GMAIL_APP_PASSWORD` (not in code). Repo is private; if they want more frequent runs, suggest making it public for unlimited Actions minutes.
