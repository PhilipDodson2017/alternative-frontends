# Alternative Frontends

Simpler, distraction-free start pages for everyday sites. Each frontend is a single static HTML file with no build step, no dependencies, and no tracking. Custom links and settings are saved in your browser's `localStorage`.

**Live:** https://philipdodson2017.github.io/alternative-frontends/

| Frontend | Live page | Description |
|---|---|---|
| Google | [/google/](https://philipdodson2017.github.io/alternative-frontends/google/) | Search box with a plain web-results mode (`udm=14`, no AI overview), a YouTube search mode, and an editable grid of shortcut tiles with light and dark themes. |

## Use it as your browser homepage

Set your browser's homepage or new-tab page to the live URL for the frontend you want. The Google frontend has a **Set as homepage** button in its footer that copies the address and shows the steps for your browser; browsers no longer let a page change the homepage itself (only Internet Explorer does).

### Choosing what appears on the Google page

The round button at the top right opens a view panel with three switches (favourites, instructions, footer) and three presets: **Everything**, **Calm** (favourites and instructions hidden) and **Search only** (only the search box and mode selector remain). The choice is remembered in the browser.

- Keyboard: `1`, `2`, `3` when the search box is not focused, or `Ctrl+Shift+1/2/3` at any time.
- Touch: swipe left on the empty background for less, right for more.
- Link: add `?view=all`, `?view=calm` or `?view=search` to the address to open straight into a preset (for example as a browser homepage); the address wins over the saved choice for that visit.

## Adding a frontend

Create a folder named after the site (e.g. `youtube/`) containing an `index.html`, then add a card to the root `index.html` and a row to the table above.

Not affiliated with Google or any other site linked from these pages.
