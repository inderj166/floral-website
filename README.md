# Floral Photography

A simple, elegant photography website. Only you can add photos (via GitHub). Visitors can view your gallery and click Like on any photo — no login, no backend, no setup required.

## Features

- Scrolling welcome banner: "Welcome to my world of floral photography"
- White background with black and blue text
- Elegant flower quotes in the four corners of the page (desktop view)
- Photo gallery — you control what's shown
- Like button on each photo (no comments)

## How Likes Work

This site has **no backend/database** (kept intentionally simple, no Firebase needed). Each visitor's likes are saved in their own browser only. That means:
- If you like a photo, it stays "liked" for you even if you come back later
- Other visitors won't see your likes, and you won't see theirs
- This is a trade-off for simplicity — if you ever want *everyone* to see the same like count, that requires a small backend, which we can add later

## How to Add a Photo

1. In your GitHub repo, open (or create) the `photos` folder, then **Add file → Upload files** to upload your image (e.g. `rose1.jpg`).
2. Open `index.html`, click the pencil (edit) icon, and find:
   ```js
   const PHOTOS = [
   ];
   ```
3. Add a line inside the brackets:
   ```js
   { id: "rose1", file: "photos/rose1.jpg", caption: "First light on a garden rose" },
   ```
4. Commit the change. Your photo now appears live on the site.

## Hosting on GitHub Pages

Go to **Settings → Pages**, set Source to the `main` branch and `/ (root)` folder, and save. Your site will be live at:
`https://inderj166.github.io/<your-repo-name>/`
