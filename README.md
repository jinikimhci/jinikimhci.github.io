# Academic Personal Website

This repository contains a minimal academic portfolio website built with plain HTML, CSS, and JavaScript.

## 1. How to preview the site locally

From the project root, run:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## 2. Where to change the About information

Edit the about text in `js/data.js`.

Look for the `about` array near the top of the file and update the paragraphs there.

## 3. Where to add or edit News

Edit the `news` array in `js/data.js`.

Each news item uses this shape:

```js
{ date: "2026", text: "Your news item here." }
```

## 4. Where to add or edit Publications

Edit the `publications` array in `js/data.js`.

Each publication entry supports:

- `badge` for the venue/year badge
- `year`
- `title`
- `authors`
- `venue`
- `award` (optional)
- `highlight` (optional subtle highlight)
- `links` with labels and URLs

## 5. Where to put the profile image and CV

Place your profile photo at:

```text
assets/images/profile.jpg
```

Place your CV at:

```text
assets/files/jini-kim-cv.pdf
```

The site currently includes a placeholder image and a placeholder CV file so the links work immediately.

## 6. How to commit and push updates to GitHub Pages

From the project root:

```bash
git add .
git commit -m "Update academic website"
git push origin main
```

Then in GitHub:

1. Open the repository on GitHub.
2. Go to Settings > Pages.
3. Set the source to GitHub Actions or Deploy from a branch.
4. If you use the branch method, publish the `main` branch root or the appropriate folder.

This project is designed for direct hosting with GitHub Pages, so you can keep the site simple and update content in `js/data.js` without editing HTML repeatedly.
