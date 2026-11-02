# M's Sound Factory Website

Live website: [calm-mermaid-20b981.netlify.app](https://calm-mermaid-20b981.netlify.app/)

A responsive static website for M's Sound Factory, an event sound and audio solutions business in Polokwane, Limpopo. The site is built with HTML, CSS, and vanilla JavaScript.

## Pages

- **Home — `index.html`:** Brand introduction, speaker hero image, company values, and a link to Services.
- **About — `about.html`:** Company introduction, event image gallery, image lightbox, mission and values, FAQ accordion, and a contact link.
- **Services — `services.html`:** Muted looping background video, a visitor-controlled showcase video, and searchable, filterable, sortable service cards.
- **Enquiry — `enquiry.html`:** Enquiry form with contact details, enquiry type, optional event date, and message.
- **Contact — `contact.html`:** Contact form, email and phone links, address, local-time display, embedded map, and directions link.

Every page shares the site navigation and footer. JavaScript updates the footer year automatically.

## Performance

- The latest inspection screenshot reports **98 Performance**, **100 Accessibility**, **92 Best Practices**, and **100 SEO**. [View the inspection screenshot](images/Screenshot%202026-11-01%20205737.png).
- The Home hero image is prioritized and asynchronously decoded for a faster visual start. [View the speaker image](images/speaker.jpeg).
- About-page gallery images load lazily and decode asynchronously.
- The Services showcase video uses `preload="none"` so it loads when a visitor chooses to play it.
- The background video appears only on the Services page and includes a static poster image.
- Reduced-motion preferences are respected by the shared stylesheet and reveal animations.
- The site uses browser-native HTML, CSS, and JavaScript without a framework or build step.

## Project structure

```text
.
├── index.html
├── about.html
├── services.html
├── enquiry.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── images/
│   ├── about-event.jpeg
│   ├── background-video.mp4
│   ├── best-in-town.jpeg
│   ├── services-showcase.mp4
│   ├── Screenshot 2026-11-01 205737.png
│   ├── speaker.jpeg
│   └── WhatsApp Image 2026-10-23 at 10.57.12.jpeg
├── robots.txt
├── sitemap.xml
└── .vscode/
    └── settings.json
```

## Shared code and assets

- **`css/style.css`** — Responsive layouts, dark visual theme, forms, gallery lightbox, FAQ styling, and reduced-motion styles.
- **`js/script.js`** — Footer year, local clock, back-to-top buttons, form validation and email-draft creation, service browsing, lightbox controls, accordion behavior, and reveal animations.
- **`images/speaker.jpeg`** — Home hero image and video poster.
- **`images/about-event.jpeg`** and **`images/best-in-town.jpeg`** — About-page gallery.
- **`images/background-video.mp4`** — Services-page background video.
- **`images/services-showcase.mp4`** — Services-page showcase video.
- **`images/Screenshot 2026-11-01 205737.png`** — Inspection score screenshot linked above.
- **`images/WhatsApp Image 2026-10-23 at 10.57.12.jpeg`** — Additional speaker image in the assets folder.
- **`robots.txt`** — Crawler access rules and sitemap location.
- **`sitemap.xml`** — Public URLs for the five website pages.
- **`.vscode/settings.json`** — Live Server port configuration (`5501`).

## Run locally

Open `index.html` in a browser, or launch the folder with the VS Code Live Server extension on port `5501`. No installation or build command is required.

## Interactive features

- Forms show field-level validation, open a pre-filled email draft for `mssoundfactory@gmail.com`, and display a concise confirmation.
- Service results respond to the search, category, and sort controls.
- The About gallery supports previous/next navigation, keyboard arrows, and closing the lightbox.
- FAQ items are interactive, and the back-to-top button provides smooth scrolling.

## Search and sharing

Each page includes a canonical URL, Open Graph metadata, and a Content Security Policy. The sitemap and robots file use the deployed Netlify address.
