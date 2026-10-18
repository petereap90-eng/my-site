# My site

A static personal homepage. No build step.

## Add a movie

Open `movies.json`, add an entry, save. Use a comma between entries.

    {
      "title": "Movie Title",
      "year": 2024,
      "watched": "2026-10-18",
      "rating": 4,
      "note": "One or two lines."
    }

Dates must be YYYY-MM-DD. Ratings can be 0.5 steps (3.5, 4, 4.5). The page sorts newest first by itself.

## Preview locally

    python3 -m http.server

Then open http://localhost:8000. Opening the HTML files directly won't work, because the pages load their data with fetch.
