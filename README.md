# NASA Gallery Scraper

A lightweight Python utility that scrapes high‑resolution images from the NASA Artemis II "Return to Earth" gallery and generates markdown files ready for static‑site generators such as Jekyll.

## Features
- Automatic extraction of image URLs, alt‑text, and full descriptions.
- Generates clean, SEO‑friendly markdown files with a consistent front‑matter format.
- Handles pagination and rate‑limits with a polite 1 second delay between requests.

## Prerequisites
- Python 3.8+ (tested on Windows 10/11)
- `pip` for installing dependencies

## Installation
```bash
# Clone the repository (once it is pushed to GitHub)
git clone https://github.com/your‑username/nasa_gallery_scraper.git
cd nasa_gallery_scraper

# Install required packages
pip install -r requirements.txt
```

## Usage
```bash
# Run the scraper with the default gallery URL
python nasa_gallery_scraper.py

# Or point it at a different gallery page
python nasa_gallery_scraper.py https://www.nasa.gov/gallery/return-to-earth/
```
The script will create a `_gallery/artemis-ii/<slug>.md` file for each image it discovers.

NASA gallery links:

https://www.nasa.gov/gallery/journey-to-the-moon/
https://www.nasa.gov/gallery/artemis-ii-launch/
https://www.nasa.gov/gallery/artemis-ii-astronauts/
https://www.nasa.gov/gallery/artemis-ii-flight-day-highlights/
https://www.nasa.gov/gallery/artemis-ii-mission-science/
https://www.nasa.gov/gallery/nasas-space-launch-system-rocket/
https://www.nasa.gov/gallery/nasas-orion-spacecraft/
https://www.nasa.gov/gallery/ground-systems/
https://www.nasa.gov/gallery/nasas-space-launch-system-rocket/page/2/
https://www.nasa.gov/gallery/nasas-space-launch-system-rocket/page/3/

https://www.nasa.gov/gallery/artemis-ii-splashdown-and-return/page/3/
https://www.nasa.gov/gallery/artemis-ii-splashdown-and-return/page/2/
https://www.nasa.gov/gallery/artemis-ii-splashdown-and-return/


## License
MIT © 2026 Richard Djarbeng – see the [LICENSE](LICENSE) file for details.
