# Quest Webloader

A sideloader and app manager for Meta Quest headsets that runs entirely in your browser. Just open the page and plug in your device.

**[webloader.app](https://webloader.app/)**

<img width="816" height="481" alt="image" src="https://github.com/user-attachments/assets/6d6d27ba-40ab-4bf4-9d41-5c5c20c4f5a4" />

## Features

- **Sideload Apps** — drag & drop APKs or folders to install
- **Manage Apps** — view, search, and sort all installed apps
- **Uninstall Apps** — remove apps from your device directly within the browser
- **Export Apps** — puill apps from your Quest to your PC as a zip
- **Device Info** — battery, storage, model, and firmware at a glance
- **Local Library** — point at a local folder on your PC to manage your local app collection, with version comparison against what's installed
- **Fully local** — nothing is uploaded anywhere, all processing happens in your browser

## Requirements

- A browser with WebUSB support, such as chromium-based browsers (Chrome, Edge, Opera, Brave)
- A USB cable that supports data
- Developer mode enabled on your Quest

## How it works

Quest Webloader implements the ADB protocol over WebUSB entirely in JavaScript. It communicates directly with your headset through the browser. No ADB binary, no companion app, no server.

## Self-hosting

It's a single `index.html` with all CSS and JS inlined. Grab the file along with `package_name_lookup.json` and the `thumbnails/` folder for display names and app icons (optional, also works without them). Serve over HTTPS or localhost.
