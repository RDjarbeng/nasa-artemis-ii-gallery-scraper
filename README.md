# NASA Gallery Scraper

A lightweight Python utility that scrapes image metadata from the NASA Artemis II "Return to Earth" gallery and generates markdown files ready for static‑site generators such as Jekyll.

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

## Example output
```
---
title: 'Artemis II Return to Earth'
image: https://www.nasa.gov/wp-content/uploads/2023/09/53116398950-7b3a7274f6-o.jpg
image_alt: 'Artemis II crew members, shown inside the Neil Armstrong Operations and Checkout Building at NASA’s Kennedy Space Center in Florida, walk toward their Orion crew module on Aug. 8, 2023. From left are: Victor Glover, pilot; Reid Wiseman, commander; Christina Hammock Koch, mission specialist; and Jeremy Hansen, mission specialist. The crew module is undergoing acoustic testing ahead of integration with the European Service Module. Artemis II is the first crewed mission on NASA’s path to establishing a long-term lunar presence for science and exploration under Artemis.'
type: external
link: ''
category: Artemis II
labels:
  - Return to Earth
date: 2026-04-14T15:33:21+02:00
---

Artemis II crew members, shown inside the Neil Armstrong Operations and Checkout Building at NASA’s Kennedy Space Center in Florida, walk toward their Orion crew module on Aug. 8, 2023. From left are: Victor Glover, pilot; Reid Wiseman, commander; Christina Hammock Koch, mission specialist; and Jeremy Hansen, mission specialist. The crew module is undergoing acoustic testing ahead of integration with the European Service Module. Artemis II is the first crewed mission on NASA’s path to establishing a long-term lunar presence for science and exploration under Artemis.

```

Image link above goes to image:
<img width="1919" height="1279" alt="image" src="https://www.nasa.gov/wp-content/uploads/2023/09/53116398950-7b3a7274f6-o.jpg" />

## Usage
```bash
# Run the scraper with the default gallery URL
python nasa_gallery_scraper.py

# Or point it at a different gallery page
python nasa_gallery_scraper.py https://www.nasa.gov/gallery/return-to-earth/
```
The script will create a `_gallery/artemis-ii/<slug>.md` file for each image it discovers.

### NASA gallery links:

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
