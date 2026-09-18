# Zia

A [Sine](https://github.com/CosmoCreeper/Sine) mod that makes [Zen Browser](https://zen-browser.app)'s frame look and work like [Dia](https://www.diabrowser.com).

**Status: alpha.** Built and tested on macOS in dark mode with the **Sidebar and Top Toolbar** layout. Light mode, the other sidebar layouts, Windows and Linux are untested.

## Install

Zia is a JavaScript mod, so Sine needs permission to load scripts from outside its marketplace.

1. Install [Sine](https://github.com/CosmoCreeper/Sine) if you haven't already.
2. In Zen, go to **Settings → Sine Mods**, open Sine's settings, and turn on **installing JS from unofficial sources**.
3. Paste this repository into the box under the marketplace:

   ```
   z1n-k/zia
   ```

4. Restart Zen when Sine asks. If the mod doesn't load, go to `about:support` and click **Clear startup cache**.

Zia expects **Look and Feel → Sidebar and Top Toolbar**, and dark mode.

Other mods may conflict with it, and Zia won't be adjusted to accommodate them. If something looks wrong, turn your other mods off and add them back one at a time.

## Setting up workspace icons

The workspace and folder icons are a large part of the Dia look. Short guide: **[Zia: setting up workspace icons](https://vimeo.com/1228144298)**

## What it does

**Page and toolbar**

- Page and toolbar sit together in one rounded card
- The toolbar takes the colour of the site under it and follows it as you scroll, switching to dark text on light sites
- Site colours are remembered per host, so the toolbar is right the moment a page opens
- A loading glow travels along the address bar
- The address reads as `domain / title`, and shows the full URL on hover

**Address bar**

- Dia-style opened panel: short rows, one weight of text throughout, no chips or row menus
- What you type stays lined up with the results underneath it

**Sidebar**

- Essentials as tiles, four to a row and six when the sidebar is wide
- Folders with hover boxes, a bounce on open, and emoji or icon covers
- Downloads sit next to the space name with a progress ring
- Cmd/Ctrl+Z undoes a closed tab for ten seconds
- An icon picker holding 1,512 Phosphor icons, as a third tab beside Zen's own

**Media and split view**

- A music player card using the track's artwork, with a glow in its colours
- Sound bars in the artwork's colours on essentials and tabs, dots when muted, click to toggle
- Per-pane toolbars in split view, and drop cards when a tab is dragged over the page

## Options

**Settings → Sine Mods → Zia**

- New tabs open your default search engine's page (on by default)
- Use Zen's accent colour for the loading bar
- A small bounce when folders open or close (on by default)

## Zen settings Zia changes

These are changed at the default level only. If you've set them yourself in `about:config`, your choice is kept.

- `zen.widget.mac.mono-window-controls` → off (native macOS window buttons)
- `zen.urlbar.replace-newtab` → off (so **+ New Tab** and Cmd+T open a real new tab)

## Known gaps

- Compact mode has no transparency or backdrop blur yet
- Light mode is untested and will very likely need work
- Other sidebar layouts, Windows and Linux are untested

## Credits

- Icons from [Phosphor Icons](https://phosphoricons.com), MIT licensed. The bundled set is unmodified; its licence is in `icons/phosphor/LICENSE`.
- The bleeding corners technique was inspired by [Bleeding Corners Fix](https://github.com/rsiebertdev/zen-themes/tree/main/bleeding-corners-fix) by rsiebertdev. Zia uses its own implementation, matched to its card shape.

## Licence

MIT. See [LICENSE](LICENSE).
