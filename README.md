# Alternative Frontends

Simpler, distraction-free start pages for everyday sites. Each frontend is a single static HTML file with no build step, no dependencies, and no tracking. Custom links and settings are saved in your browser's `localStorage`.

**Live:** https://philipdodson2017.github.io/alternative-frontends/

| Frontend | Live page | Description |
|---|---|---|
| Google | [/google/](https://philipdodson2017.github.io/alternative-frontends/google/) | Search box with a plain web-results mode (`udm=14`, no AI overview), a YouTube search mode, and an editable grid of shortcut tiles with light and dark themes. |

## Use it as your browser homepage

Set your browser's homepage or new-tab page to the live URL for the frontend you want. The Google frontend has a **Set as homepage** button in its footer that copies the address and shows the steps for your browser; browsers no longer let a page change the homepage itself (only Internet Explorer does).

## Focus mode (Google frontend)

The Google start page can hide the parts you don't need while you search. Hidden parts are removed from the page, not just faded out, so the keyboard and screen readers skip them too.

| Control | What it does |
|---|---|
| **Hide all** / **Show all** (top right) | Hides the three rows below in one action, and brings them all back. |
| **Hide favourites** / **Show favourites** (above the tiles) | The shortcut tiles. |
| **Hide instructions** / **Show instructions** (at the end of the hint line) | The hint lines under the search box. |
| **Hide page buttons** / **Show page buttons** (left of the footer buttons) | The row of page buttons. |
| **Peek** (top left) | Off by default. When it is on and everything is hidden, resting the pointer near the top or bottom edge brings that row back until the pointer leaves. It is switched off automatically when the browser asks for reduced motion. |

Each control says the action it performs, and the setting is remembered in the browser.

Other ways to hide everything:

- **Ctrl+Shift+F** (or Cmd+Shift+F on a Mac): works even while the search box has focus.
- **F**: when the search box does not have focus. Press **Escape** to leave the search box first.
- **Double-click or double-tap** on empty background.
- **`#focus`** at the end of the page address, so a homepage or bookmark opens straight into the calm view (`#focus=0` forces the full view).

### Choosing the search mode by voice

The Google frontend can switch between Google, Gemini, All and YouTube by voice, using the browser's built-in speech recognition **on the device only**. No audio leaves the device and no cloud recognition is used.

- The **Voice** button appears only when the browser reports on-device English recognition as available (`SpeechRecognition.available({langs:["en-US"], processLocally:true})` returns `"available"`). In Firefox, and in browsers that only offer cloud recognition, the button is not in the page at all.
- If the browser supports on-device recognition but the speech pack is not downloaded yet, the page offers a **Download voice pack** button. Nothing is downloaded until you click it: your browser then downloads its English speech pack, and the audio itself still stays on the device.
- Commands: Google, Gemini, All, YouTube, hide everything, show all.

## Adding a frontend

Create a folder named after the site (e.g. `youtube/`) containing an `index.html`, then add a card to the root `index.html` and a row to the table above.

Not affiliated with Google or any other site linked from these pages.
