# QIn — Klingon-Themed Roundcube Skin

A dark, green-based Roundcube email skin with a Klingon military/sci-fi aesthetic. **QIn** (tlhIngan Hol: "message" / "torpedo") — every email is a photon torpedo.

Based on the [Elastic](https://github.com/roundcube/roundcubemail/tree/master/skins/elastic) skin.

## Features

- Dark green palette with tactical green (`#00cc6a`) accent
- Angular clip-path buttons with uppercase lettering
- HUD glow lines on headers and footers
- Scan-line CRT overlay (disabled on mobile)
- Glowing login page with angular form
- Green focus rings on inputs
- Dark mode "deeper black" variant
- Fully responsive (desktop, tablet, phone)

## Installation

1. Copy the `QIn` directory into your Roundcube `skins/` folder:
   ```bash
   cp -r QIn /path/to/roundcubemail/skins/
   ```

2. Set the skin in your Roundcube config (`config/config.inc.php`):
   ```php
   $config['skin'] = 'QIn';
   $config['skin_logo'] = 'skins/QIn/images/logo.svg';
   ```

3. If you modify the LESS files, rebuild CSS:
   ```bash
   cd skins/QIn && make css
   ```

## Files Changed from Elastic

| File | Change |
|------|--------|
| `meta.json` | Name + theme-color |
| `styles/colors.less` | Full rewrite — all color variables |
| `styles/_styles.less` | New — Klingon aesthetic CSS |
| `images/logo.svg` | New — angular blade emblem |
| `images/contactgroup.svg` | Green palette |
| `images/contactpic.svg` | Green palette |
| `images/corner-handle.svg` | Green palette |
| `images/download.svg` | Green palette |

All templates, layout, JS, and fonts are unchanged from Elastic.

## License

Creative Commons Attribution-ShareAlike — same as the Elastic skin.

Qapla'!
