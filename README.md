# Google Maps Web Scraper (Modified)

A Chrome/Brave browser extension that scrapes business data from Google Maps and automatically tests each website's page speed using the Google PageSpeed Insights API.

This is a modified version of the original Google Maps Easy Scrape extension by [the original creator](https://www.youtube.com/watch?v=8VckTa1Wgwc). The core scraping functionality is the same — this version adds **automated PageSpeed Insights testing** so you can identify businesses with slow websites as potential leads.

## What It Does

- Scrapes business listings directly from a Google Maps search, including:
  - Business name
  - Rating & review count
  - Phone number
  - Industry
  - Address
  - Website URL
  - Google Maps link
- **Automatically runs each scraped website through Google's PageSpeed Insights API** and records the performance score
- Exports everything to a downloadable CSV

With this tool you can scrape ~400 leads in roughly 20 minutes with page speeds tested and recorded — a process that would take 10+ hours manually.

## Installation

1. Download or clone this repository and extract the files.
2. Open your Chromium-based browser (Chrome, Brave, Edge, etc.).
3. Navigate to the extensions page:
   - **Chrome:** `chrome://extensions`
   - **Brave:** `brave://extensions`
4. Enable **Developer mode** (toggle in the top-right corner).
5. Click **Load unpacked** and select the extracted extension folder.
6. Pin the extension for easy access.

## Setup

You'll need your own **Google PageSpeed Insights API key**:

1. Go to [PageSpeed Insights API — Get Started](https://developers.google.com/speed/docs/insights/v5/get-started).
2. Generate a free API key.
3. Open the extension's source code and paste your key into the API key variable.

## Usage

1. Go to [Google Maps](https://www.google.com/maps).
2. Search for a business type and location (e.g., "HVAC Dallas Fort Worth").
3. **Scroll all the way down** through the results until you see "You've reached the end of the list." This loads all available listings.
4. Click the extension icon and hit **Scrape Google Maps**.
5. **Leave the scraping window open for 1–2 minutes** while the PageSpeed tests run.
6. Name your file, then click **Download CSV**.

## Notes & Limitations

- **PageSpeed results cover roughly 80–90% of scraped sites.** Some will return `error` — these can be tested manually, though many also error on Google's own PageSpeed site.
- Some businesses don't have a website linked on Google Maps, so no URL or speed score will be available for those.
- The extension only works on Google Maps tabs. If you try to run it elsewhere, it will redirect you to Google Maps.
- Works on any Chromium-based browser (Chrome, Brave, Edge, Arc, etc.) on both Mac and PC.

## Credits

Original Google Maps Easy Scrape extension by [this creator](https://www.youtube.com/watch?v=8VckTa1Wgwc). Modified to include automated PageSpeed Insights testing.
