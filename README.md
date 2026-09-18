# Zia

**Zen Browser, with Dia's face.**

A [Sine](https://github.com/CosmoCreeper/Sine) mod that reworks Zen's frame into something close to [Dia](https://www.diabrowser.com): the page in a rounded card, a toolbar that takes the colour of the site under it, and a Dia-style sidebar and address bar.

![Status](https://img.shields.io/badge/status-alpha-orange)
![Platform](https://img.shields.io/badge/tested%20on-macOS%20%C2%B7%20dark%20mode-informational)
![Licence](https://img.shields.io/badge/licence-MIT-blue)

> **Alpha.** Built and tested on macOS, dark mode, **Sidebar and Top Toolbar** layout. Light mode, the other layouts, Windows and Linux are untested and will likely need work. Feedback on those is exactly what's wanted.

---

## Install

Zia is a JavaScript mod, so Sine needs permission to load scripts from outside its marketplace.

1. Install [Sine](https://github.com/CosmoCreeper/Sine).
2. In Zen: **Settings → Sine Mods**, open Sine's settings, turn on **installing JS from unofficial sources**.
3. Paste this into the box under the marketplace:

   ```
   z1n-k/zia
   ```

4. Restart Zen when Sine asks. If the mod doesn't load, open `about:support` and click **Clear startup cache**.

**Set Look and Feel → Sidebar and Top Toolbar**, and use dark mode.

Other mods may conflict, and Zia won't be adjusted to accommodate them. If something looks wrong, turn your other mods off and add them back one at a time.

## Workspace icons

The workspace and folder icons carry a lot of the Dia look, and they're worth setting up.

▶ **[Zia: setting up workspace icons](https://vimeo.com/1228144298)**

---

## What it does

### The page and the toolbar

The page and toolbar sit together in one rounded card. The toolbar takes the colour of the site under it and follows that colour as you scroll, switching to dark text on light sites. Colours are remembered per host, so a page opens in the right colour rather than fading into it. A glow travels along the address bar while a page loads, and the address itself reads as `domain / title`, showing the full URL when you hover it.

### The address bar

Opened, it's Dia's panel: short rows with air around them, one size and weight of text throughout, and none of Firefox's chips, row menus or one-off engine bars. What you type stays lined up with the results underneath it.

### The sidebar

Essentials sit as tiles, four to a row and six when the sidebar is wide. Folders get hover boxes, a bounce when they open, and emoji or icon covers. Downloads live next to the space name with a progress ring around them. Closing a tab by accident is undone with Cmd/Ctrl+Z for ten seconds afterwards.

There's an icon picker too — a third tab beside Zen's own, holding 1,512 Phosphor icons with its own search.

### Media and split view

Playing music gives you a card with the track's artwork and a glow in its colours. Sound bars in those same colours appear on essentials and tabs, turning to dots when muted, and clicking them toggles the sound. Split view gives each pane its own toolbar, and dragging a tab over the page brings up drop cards for either side.

---

## Options

**Settings → Sine Mods → Zia**

| Option | Default |
| --- | --- |
| New tabs open your default search engine's page | on |
| Use Zen's accent colour for the loading bar | off |
| Small bounce when folders open or close | on |

<details>
<summary><b>Zen settings Zia changes</b></summary>

Changed at the default level only. If you've set either yourself in `about:config`, your choice is kept.

- `zen.widget.mac.mono-window-controls` → off, for native macOS window buttons
- `zen.urlbar.replace-newtab` → off, so **+ New Tab** and Cmd+T open a real new tab

</details>

<details>
<summary><b>Known gaps</b></summary>

- Compact mode has no transparency or backdrop blur yet
- Light mode is untested and will very likely need work
- Other sidebar layouts, Windows and Linux are untested

</details>

---

## Credits

Icons are [Phosphor](https://phosphoricons.com), MIT licensed and bundled unmodified; their licence is in `icons/phosphor/LICENSE`.

The bleeding corners technique was inspired by [Bleeding Corners Fix](https://github.com/rsiebertdev/zen-themes/tree/main/bleeding-corners-fix) by rsiebertdev. Zia uses its own implementation, matched to its card shape.

## Licence

[MIT](LICENSE).
