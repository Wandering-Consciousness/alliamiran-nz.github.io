# All I Am, I Ran — Kat's 2025 Great Walks Website

A celebration website for Kat's incredible achievement of running all 10 of New Zealand's Great Walks in 2025.

## Setup Instructions

### 1. Add Your Photos
Place all 95 photos in the `photos/` folder. The filenames should match exactly as listed (they're already configured in the site).

### 2. Update Gift Links
Open `index.html` and find these lines near the bottom (search for "stravaLink" and "bookLink"):

```html
<a href="#" class="gift-link" id="stravaLink">View the Route →</a>
```
```html
<a href="#" class="gift-link" id="bookLink">Get the Book →</a>
```

Replace the `href="#"` with:
- **Strava Art**: Your Strava activity URL once you've run "ALL I AM I RAN"
- **Book**: Your Amazon gift certificate URL for "Wild" by Cheryl Strayed

### 3. View Locally
Simply open `index.html` in a web browser. No server required!

For best results, use a modern browser (Chrome, Firefox, Safari, Edge).

### 4. Optional: Host Online
To share the URL with Kat, you can host it on:
- **Netlify** (free): Drag and drop the folder at netlify.com/drop
- **GitHub Pages** (free): Push to a repo and enable Pages
- **Your own domain**: Upload via FTP

**Suggested domain**: `alliamiran.nz`

## File Structure

```
kat-great-walks/
├── index.html          # Main website
├── photos/             # Put all 95 photos here
│   └── (your photos)
├── poems/              # Individual poem pages
│   ├── rakiura.html
│   ├── tongariro.html
│   ├── abel-tasman.html
│   ├── heaphy.html
│   ├── kepler.html
│   ├── milford.html
│   ├── routeburn.html
│   ├── waikaremoana.html
│   └── paparoa.html
└── README.md           # This file
```

## Features

- **Animated haiku** on hero section
- **Counting stats** (521km, 10 Great Walks, etc.)
- **Interactive map** of New Zealand with track locations
- **Photo gallery** with lightbox (95 photos, masonry layout)
- **Poem pages** for each track
- **"One More To Go"** section for Hump Ridge
- **Gift links** for Strava art and book
- **Personal message** from you
- **Ambient NZ bird sounds** (click the speaker icon)
- **Fully responsive** for mobile viewing

## Audio Note

The site includes ambient tūī birdsong from Wikimedia Commons (Creative Commons licensed). It's muted by default — click the speaker icon in the bottom right to enable.

## Customization

### Change the personal message
Find this section in `index.html`:
```html
<section class="message">
    <div class="message-content">
        <p>Merry Xmas sis! Awesome effort on the 2025 Great Walks...</p>
```

### Add more poems
If Kat writes poems for the other tracks, you can update the placeholder pages in `poems/`.

---

Merry Christmas! 🎄🏃‍♀️
