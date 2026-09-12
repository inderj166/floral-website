## Floral Photography Website 

A simple, elegant photography website. Visitors can view my gallery and click Like on any photo — no login, no backend, no setup required.

## Live Site

**[https://inderj166.github.io/floral-website/](https://inderj166.github.io/floral-website/)**

## Features :

- Scrolling welcome banner: "Welcome to my world of floral photography"
- black background with white and blue text
- Elegant flower quotes in the four corners of the page (desktop view)
- Photo gallery — you control what's shown
- Like button on each photo (no comments)

## How Likes Work

This site has **no backend/database** (kept intentionally simple, no Firebase needed). Each visitor's likes are saved in their own browser only. That means:
- If you like a photo, it stays "liked" for you even if you come back later
- Other visitors won't see your likes, and you won't see theirs
- This is a trade-off for simplicity — if you ever want *everyone* to see the same like count, that requires a small backend, which we can add later

## How to Add a Photo

You can add as many photos as you like — just repeat these steps for each one.

1. In your GitHub repo, open the `photos` folder, then **Add file → Upload files** to upload your image (e.g. `rose1.jpg`).
2. Open `index.html`, click the pencil (edit) icon, and find:
   ```js
   const PHOTOS = [
   ];
   ```
3. Add a line inside the brackets for each photo:
   ```js
   const PHOTOS = [
     { id: "rose1", file: "photos/rose1.jpg", caption: "First light on a garden rose" },
     { id: "rose2", file: "photos/rose2.jpg", caption: "Deep red bloom" },
   ];
   ```
   Each photo needs a unique `id`, the correct `file` path, and any `caption` you like.
4. Commit the change. Your photo(s) now appear live on the site.

## Hosting on GitHub Pages

Go to **Settings → Pages**, set Source to the `main` branch and `/ (root)` folder, and save. Your site will be live at:
`https://inderj166.github.io/floral-website/`

