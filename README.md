# Command Dashboard

A customizable futuristic browser dashboard designed for a Chrome New Tab experience.

## Features

- Futuristic HUD-style interface
- Google, Bing, DuckDuckGo, and YouTube search
- Live digital clock
- Quick-access links
- Custom accent color picker
- HEX color input
- Preset themes
- Persistent theme and search-engine settings with `localStorage`
- Keyboard shortcuts
- Responsive layout
- Chrome Manifest V3 support

## Project Structure

```text
command-dashboard/
├── index.html
├── style.css
├── script.js
├── manifest.json
├── README.md
├── assets/
│   └── icons/
│       └── icon128.png
└── font/
    └── KodeMono-Regular.ttf
```

## Run as a normal webpage

Open `index.html` in a browser.

The Kode Mono font is optional. If `font/KodeMono-Regular.ttf` is not present, the interface falls back to a monospace font.

## Install as a Chrome New Tab extension

1. Open `chrome://extensions/`
2. Enable **Developer mode**
3. Click **Load unpacked**
4. Select this project folder
5. Open a new tab

The `manifest.json` uses Chrome's `chrome_url_overrides.newtab` feature to replace the default New Tab page.

## Theme Controls

Open the `◈` button to access the theme panel.

You can use:

- The color picker
- A six-digit HEX value
- Preset colors
- Reset to the default red theme

Examples:

```text
#ff003c
#00e5ff
#8b5cf6
#00ff66
#0088ff
```

The selected accent is saved locally in the browser.

## Keyboard Shortcuts

| Key | Action |
|---|---|
| `/` | Focus search |
| `Enter` | Search |
| `Esc` | Close theme panel |

## Search Engines

The current search options are:

- Google
- Bing
- DuckDuckGo
- YouTube

The selected search engine is remembered locally.

## Customization

The main theme values are controlled by CSS variables in `style.css`:

```css
:root {
    --accent: #ff003c;
    --accent-rgb: 255, 0, 60;
}
```

The JavaScript changes these variables when the user selects a different color.

## GitHub

For a normal GitHub repository, it is better to keep the source files visible in the repository and use the ZIP as a downloadable package.

Recommended repository structure:

```text
repository/
├── index.html
├── style.css
├── script.js
├── manifest.json
├── README.md
├── assets/
└── font/
```

The ZIP can be uploaded separately as a release/download package.

## License

Add your preferred license here.

## Credits

Built as a reusable customizable dashboard interface for browser and new-tab projects.
