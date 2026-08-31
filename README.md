[![GitHub Pages](https://img.shields.io/github/pages/status/NikhilShimpy/Ask-her-out-/main?label=GitHub%20Pages)](https://nikhilshimpy.github.io/Ask-her-out-/) [![Live Demo](https://img.shields.io/website?url=https://nikhilshimpy.github.io/Ask-her-out-/)](https://nikhilshimpy.github.io/Ask-her-out-/)

# Ask Her Out

Live demo: https://nikhilshimpy.github.io/Ask-her-out-/

A playful, static "Will you be my Valentine?" web page that guides the visitor through a small set of acceptance/refusal pages. The site uses Tenor GIF embeds for visuals and a tiny bit of JavaScript to make the "No" button move for comedic effect.

## Features
- Simple, mobile-friendly layout (HTML + CSS).
- Tenor GIF/sticker embeds to add expressive visuals.
- A fun interaction: on the final "No" page the "No" button moves randomly when hovered.
- Ready to host on GitHub Pages (already deployed at the live demo link above).

## Project structure
```
index.html        — main landing page (Yes / No)
yes.html          — "Yes" response page
no1.html          — first "No" response page
no2.html          — second "No" response page
no3.html          — final "No" page (contains moving "No" button)
style.css         — shared styling
script.js         — moves the "No" button on hover
```

## How to run locally
Open `index.html` in your browser, or serve the folder with a local static server:

```bash
# From project root
python -m http.server 8000
# visit http://localhost:8000
```

No build or dependencies are required.

## How it works (brief)
- Each page is a static HTML file styled by `style.css`.
- GIFs/stickers are embedded using Tenor's embed script: `https://tenor.com/embed.js`.
- `no3.html` includes `script.js` which defines `moveRandomEl()` — this sets random `top` and `left` percentages on the "No" link when the mouse enters it, making it harder to click.

## Customization ideas
- Replace Tenor embeds with local images or other CDN images if you want offline or privacy-friendly operation.
- Change texts in the `<h1>` tags to personalize the message.
- Add sharing buttons or a mailto link to send the person a message if they click "Yes".
- Add a CSS animation for button hover states to make interactions smoother.

## Credits
- Tenor (tenor.com) for GIF/sticker embeds.
- Built by NikhilShimpy.

## License
No license file is included in this repository. If you want others to reuse this project, add a LICENSE (e.g., MIT) to the repo.
