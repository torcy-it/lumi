# Website images

Replace any file here **keeping the same filename** — the site will load it automatically.

## App icons (default only — App Icon 1)

**Source in Xcode:** `Final Version/Assets.xcassets/appicon_1.imageset/appicon_1.png`  
**Do not use** `appicon_2` (Red Hood alternate icon).

| File | Use |
|------|-----|
| `app-icon-default.png` | Header brand icon (all pages) |
| `favicon-32.png` | Browser tab |
| `favicon-192.png` | High-res browser icon |
| `apple-touch-icon.png` | Add to Home Screen |

To refresh all icons from the app project:

```bash
SRC="Final Version/Assets.xcassets/appicon_1.imageset/appicon_1.png"
cp "$SRC" website/images/app-icon-default.png
sips -z 32 32 "$SRC" --out website/images/favicon-32.png
sips -z 192 192 "$SRC" --out website/images/favicon-192.png
sips -z 180 180 "$SRC" --out website/images/apple-touch-icon.png
```

## Home (`index.html`)

| File | Where it appears |
|------|------------------|
| `lumi-say-hi.png` | Lumi on the home page (tap to jump) |

## How To Play (`regole.html`)

| File | Step |
|------|------|
| `howto-point1.png` | 1 — Explore the islands |
| `howto-point2.png` | 2 — Complete the chapters |
| `howto-point3.png` | 3 — Put events in order |
| `howto-point4.png` | 4 — Unlock the book |

## About Us (`chi-siamo.html`)

`developers/` folder — one circular photo per developer.

## Tips

- Recommended format: **PNG**. Square team photos work best (they are cropped into circles).
- After replacing icons: hard-refresh (`Cmd+Shift+R`) or close/reopen the browser tab.
