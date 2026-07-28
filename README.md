# Pin to Address — Precision Interactive Geocoder

A responsive, zero-dependency, single-file web application that allows users to click anywhere on an interactive OpenStreetMap to extract formatted street addresses, separated postal codes, and geographical coordinates.

## ✨ Features

- **Single-File Architecture**: Zero build steps, bundlers, or local Node.js dependencies. Works straight out of the box in any modern web browser.
- **Precision Interactive Geocoding**: Powered by [Leaflet.js](https://leafletjs.com/) and [OpenStreetMap](https://www.openstreetmap.org/), allowing users to pan, zoom, and drop pins globally.
- **Granular Data & One-Click Copy**: Separates geocoding outputs into three clean, independently copyable data fields with visual Clipboard API confirmation:
  - **Formatted Street Address**
  - **Postal / Zip Code**
  - **Raw Coordinates (Lat, Lng)**
- **Sleek Modular Glassmorphism UI**:
  - Modern design system utilizing tailored HSL tokens, smooth micro-animations, and full automatic **Dark Mode / Light Mode** adaptation.
  - Modular 3-part interface designed to keep the map unobstructed: floating top-left brand card, top-right GPS location control, and a compact location results card at the bottom.
- **Performance & Usage Compliance**:
  - **Session Memory Cache**: Caches reverse-geocoded results down to 5 decimal places (~1.1-meter accuracy). Re-selecting previously queried coordinates loads instantly without redundant network calls.
  - **Nominatim Policy Compliance**: Includes an automatic 1.2-second debounce rate limit indicator and explicit query string identification parameters.

---

## 🚀 How to Run

Click the GitHub page URL or follow these steps:

1. Download or clone this repository:
   ```bash
   git clone https://github.com/your-username/address-generator.git
   cd address-generator
   ```
2. Open `index.html` directly in any contemporary web browser (Chrome, Edge, Firefox, Safari):
   - Double-click the file in your file explorer, OR
   - Drag and drop `index.html` into your browser window, OR
   - Serve using a lightweight local development server (e.g., VS Code Live Server or `npx serve .`).

---

## 🛠️ Technology Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Markup & Logic** | HTML5 / Vanilla JS (ES6+) | Clean semantic DOM structure, asynchronous Fetch & Clipboard API |
| **Styling** | Vanilla CSS3 | Custom semantic CSS variables, responsive media queries, backdrop blur |
| **Map Engine** | [Leaflet.js (v1.9.4)](https://leafletjs.com/) | Lightweight open-source mapping library served via CDN |
| **Map Tiles** | OpenStreetMap | Free public raster tile layers |
| **Geocoder API** | [Nominatim](https://nominatim.openstreetmap.org/) | Direct browser-to-service JSONv2 reverse geocoding endpoints |

---

## 📝 License

This software is provided "as is" under the MIT License. Map tile and reverse geocoding data are copyright © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), powered by Nominatim.
