# BLC Spring Conference 2026

Conference landing page for the Blended Learning Consortium Spring Conference 2026.

**Date:** Thursday 22nd May 2026
**Venue:** Artrix, Bromsgrove Campus — Heart of Worcestershire College

---

## Getting started

No build tools or dependencies. Open `index.html` directly in a browser, or use the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) VS Code extension for auto-reload on save.

---

## File structure

```
/
├── index.html          # All HTML, CSS and JS in one file
└── assets/
    └── images/
        ├── BLC logo - landscape colour_2x.png
        └── How dark logo.PNG
```

---

## How to update content

### Programme / session details

Session data lives in the `sessions` object in the `<script>` block near the bottom of `index.html`. Each session has:

```js
keynote1: {
  title: 'Opening & Keynote 1',
  time: '09:30 – 10:10',
  location: 'Artrix, Bromsgrove Campus',
  speaker: 'Speaker name',           // set to null to hide
  description: 'Session description.',
  eventbriteUrl: null,               // paste Eventbrite URL here to show booking button
},
```

Setting `eventbriteUrl` to a URL will automatically show a **Book your place on Eventbrite** button in the session modal.

### Venue link

The venue link in the hero is an `<a>` tag wrapping the venue name. Update the `href` there if the URL changes.

### Sponsors

Sponsor cards are in the `#sponsors` section. Each is a `.sponsor-card` div — add an `<img>` tag for logo images, or use `.sponsor-name` for text-only. Add `.dark` to the card for a dark background (used for the HoW logo).

### Conference theme

The hero title currently reads `[Conference Theme Here]` — replace that placeholder text once the theme is confirmed.

---

## Eventbrite links

When Eventbrite listings go live, update `eventbriteUrl` in the relevant session objects. The booking button will appear in the modal automatically. Also update the main **Register on Eventbrite** buttons in the hero and the Register section — search for `href="#"` to find them.
