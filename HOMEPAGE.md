# Dead Simple — Holding Page

## What this is
A single-page holding page for deadsimplestudio.com. Nothing more.

## Requirements
- Black background (#000), full viewport
- Dead Simple logo centered horizontally and vertically
- No text, no links, no animation, no interactivity
- Responsive — works on desktop and mobile
- Hosted on GitHub Pages
- Favicon should be the inverted logo (white background, black mark)

## Logo
The logo is an SVG. Use it exactly as provided — do not redraw or approximate it.

```svg
<svg width="640" height="640" viewBox="0 0 640 640" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="128" y="156" width="149" height="149" fill="white"/>
<rect x="488" y="401" width="80" height="336" transform="rotate(90 488 401)" fill="white"/>
<path d="M512 191.154L472.153 231L512 270.846L477.846 305L438 265.153L398.154 305L364 270.847L403.846 231L364 191.153L398.153 157L438 196.846L477.847 157L512 191.154Z" fill="white"/>
</svg>
```

For the favicon, invert the fills (black mark on white background):

```svg
<svg width="640" height="640" viewBox="0 0 640 640" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect width="640" height="640" fill="white"/>
<rect x="128" y="156" width="149" height="149" fill="black"/>
<rect x="488" y="401" width="80" height="336" transform="rotate(90 488 401)" fill="black"/>
<path d="M512 191.154L472.153 231L512 270.846L477.846 305L438 265.153L398.154 305L364 270.847L403.846 231L364 191.153L398.153 157L438 196.846L477.847 157L512 191.154Z" fill="black"/>
</svg>
```

## File structure
```
/
├── index.html
└── favicon.svg
```

## Technical notes
- Single HTML file, inline CSS, no external dependencies
- Logo should render at approximately 120px on desktop, 90px on mobile
- `<title>` should be "Dead Simple"
- `<meta name="description">` should be "Dead Simple — a product studio."
- Use `min-height: 100dvh` with `100vh` fallback for full viewport

## Deployment
- GitHub Pages from the `main` branch root
- Custom domain: deadsimplestudio.com
- Add CNAME file with `deadsimplestudio.com`
