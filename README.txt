ARTISANS HOT DOGS — WEBSITE FOLDER
Cleaned up by Eva on 2026-10-03. Nothing was deleted — old versions
live in _archive/, scratch notes in _notes/.

LIVE SITE FILES (upload these to host the site)
  index.html          Homepage — menu, catering, nav. Links to locations.html
  locations.html      "Where to Find Us" live map. Reads your Google Sheet
                      ("Location Coordinates") and moves the pin. Refreshes
                      every 5 minutes. No API key needed.
  grab-coords.html    YOUR PRIVATE TOOL — not linked from the site. Open it on
                      your phone at the trailer, tap "Grab My Location", copy
                      the numbers, paste into row 2 of the sheet. Bookmark it.
  style.css           The site stylesheet.
  images/             All pictures (menu dogs, catering shots, hero card).

HOW TO RUN IT ON YOUR CHROMEBOOK
  python3 -m http.server 8000 --directory "/mnt/chromeos/MyFiles/Documents/Zen River"
  Then open: http://localhost:8000/index.html

HOW TO MOVE THE MAP PIN (from your phone)
  1. Open grab-coords.html on your phone at the trailer (or Google Maps).
  2. Copy the latitude & longitude.
  3. Google Sheets app → "Location Coordinates" → row 2 → paste.
  4. The website pin follows within 5 minutes. You never touch the site files.

OTHER FOLDERS
  docs/               Licensing Criteria PDFs (health dept paperwork).
  _archive/           Old versions: index1.html (index2.html was an identical
                      duplicate), workingindex.html (said "Artisan" singular),
                      locations1.html, broken.html, website.css (duplicate of
                      style.css), backup.txt, index.txt, grab-coords-duplicate.txt
                      (you saved the grabber page twice), location.json /
                      locations.json (old coordinate snippets).
  _notes/             Scratch files: startupcmmds.txt (your server commands),
                      AiPrompt.txt, Googlers.txt, whatMovesTheMarkets.txt.

NOTES
  - Images were moved from the folder root into images/ and the 9 references
    in index.html were updated. If any picture ever looks broken, check that
    the images/ folder uploaded with the site.
  - The homepage title says "Artisans Hot Dogs" (plural). workingindex.html
    said "Artisan" (singular) — flag which one you want before we lock it in.
