# Kono-007.github.io

Interactive Windows 7 style web experience built with plain HTML, CSS, and JavaScript.

## Overview

This project includes:

- A lock-style landing page (`index.html`) with a folder rename/password interaction.
- A desktop page (`windows.html`) with:
	- Windows-like taskbar
	- Desktop app icons
	- Draggable in-page app popups
	- Live 24h clock
	- Start menu style Windows popup with open/close animations

## How It Works

### Login flow

On `index.html`, you type text in the input and press Enter:

- First entry stores the value.
- If the next entry matches the previous one, it redirects to `windows.html`.

### Desktop behavior

On `windows.html`:

- Clicking taskbar or desktop app icons opens popups.
- Multiple different app popups can be open at the same time.
- Clicking the same app focuses its existing popup.
- Windows button toggles the Start menu popup.
- Popups are draggable by their title bars.

## App Popups

- Windows: Start menu style popup anchored at bottom-left.
- Chrome: Browser-style popup with design links (from `web_demo/design.html`) and site logos.
- Spotify: Popup with profile link and album embeds.
- Letterboxd: Popup with profile info and dynamically loaded recent poster feed.

## Project Structure

- `index.html`: Entry/login page.
- `windows.html`: Desktop UI and popup/window logic.
- `styles.css`: Shared styling used by pages.
- `Source/`: Icons, wallpaper, and profile image assets.

## Run Locally

1. Open the folder in VS Code.
2. Open `index.html` in your browser (or with Live Server).
3. Enter the same text twice to access the desktop page.

## Notes

- The Letterboxd section uses an RSS-to-JSON endpoint and may fail if the service is unavailable.
- External embeds (Spotify/links) require internet access.