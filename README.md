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

## Add a photo

1. Resize to about 1600px on the long side and export as JPEG. Remove location data.
2. Put the file in the `photos/` folder.
3. Add a line to `photos.json`:

       { "file": "my-photo.jpg", "caption": "Optional caption" }

## Preview locally

    python3 -m http.server

Then open http://localhost:8000. Opening the HTML files directly won't work, because the pages load their data with fetch.
