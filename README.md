# All I Am, I Ran — Kat's 2025 Great Walks Website

A celebration website for Kat's incredible achievement of running all 10 of New Zealand's Great Walks in 2025.

## Setup Instructions

### 1. Add Your Photos
Place all 95 photos in the `photos/` folder. The filenames should match exactly as listed (they're already configured in the site).

### 2. Add Google Maps API Key (Required for Map)
The interactive map uses Google Maps. To enable it:

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a project (or use an existing one)
3. Enable the "Maps JavaScript API"
4. Create an API key from the Credentials page
5. Open `index.html` and find this line near the bottom:
   ```html
   src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap&loading=async"
   ```
6. Replace `YOUR_API_KEY` with your actual API key

**Note**: Google Maps API has a generous free tier (28,000 map loads/month). For a personal gift site, you'll never hit the limit.

If you skip this step, the map will show a friendly placeholder message.

### 3. Update Gift Links
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

### 4. View Locally
Simply open `index.html` in a web browser. No server required!

For best results, use a modern browser (Chrome, Firefox, Safari, Edge).

### 5. Optional: Host Online
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
- **Google Maps** with accurate markers for all 11 track locations
- **Photo gallery** with lightbox (95 photos, masonry layout)
- **Poem pages** for each track
- **"One More To Go"** section for Hump Ridge
- **Gift links** for Strava art and book
- **Personal message** from you
- **Ambient NZ bird sounds** (click the speaker icon)
- **Fully responsive** for mobile viewing

## Map Track Locations

The Google Map includes accurate GPS coordinates for all tracks:

| Track | Coordinates | Location |
|-------|-------------|----------|
| Routeburn Track | -44.7354, 168.1846 | Routeburn Shelter, near Glenorchy |
| Rakiura Track | -46.8997, 168.1269 | Oban, Stewart Island |
| Tongariro Northern Circuit | -39.1979, 175.5422 | Whakapapa Village |
| Abel Tasman Coast Track | -40.9786, 173.0058 | Marahau |
| Lake Waikaremoana | -38.7397, 177.0608 | Te Urewera |
| Heaphy Track | -40.9167, 172.5500 | Brown Hut, Kahurangi NP |
| Paparoa Track | -42.3661, 171.4078 | Blackball |
| Milford Track | -45.1265, 167.7433 | Glade Wharf, Lake Te Anau |
| Kepler Track | -45.4359, 167.7106 | Te Anau |
| Hump Ridge Track | -46.1322, 167.4578 | Rarakau, Tuatapere |

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
