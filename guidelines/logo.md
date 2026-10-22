# The logo

**There is one logo, and it is always the same drawing in the same colours.** It is the porter's head and shoulders under his top hat (the symbol) beside the drawn wordmark, `napwake`. A small set of approved files covers every place it goes; nothing else is the logo. Never redraw it, re-colour it, re-pose it or retype it. The porter's poses are illustrations, never the logo.

## The approved versions

Every file is in [`../logo/`](../logo/). A `-dark` file is for dark grounds.

| Version | On light | On dark | Use it for |
|---|---|---|---|
| **Primary lockup**, horizontal | `lockup-horizontal.svg` | `lockup-horizontal-dark.svg` | The default, wherever the logo goes: page headers, posts, slides, footers. |
| Stacked lockup | `lockup-stacked.svg` | `lockup-stacked-dark.svg` | Where the space is closer to square than wide. |
| **The mark alone** (symbol) | `symbol.svg` | `symbol-dark.svg` | Small spaces and places that already say the name: icons from 32 px, the avatar. |
| **One colour** | `lockup-horizontal-mono-ink.svg`, `lockup-stacked-mono-ink.svg`, `symbol-mono-ink.svg` (Night) | the same names in `-mono-paper` (Paper) | Wherever full colour can't print or would clash: photos, coloured grounds, one-colour print, embossing. |
| One colour on Coat | | `symbol-on-coat.svg` | On the brand's teal, Coat: Paper, with the eyes cut in Coat. |
| Wordmark alone | `wordmark.svg` | `wordmark-dark.svg` | Only where the porter is already in the picture: the README header, the social preview, the launch card. |
| Avatar | `avatar-500.png` (on Lamp) | `avatar-500-dark.png` (on Night) | The GitHub organization avatar and other circle crops. Everything that matters sits inside the inscribed circle. SVG sources beside them. |
| Favicon | `favicon-16.svg` | `favicon-16-dark.svg` | Browser tabs: the 16-pixel cut, drawn on whole pixels, not scaled. `favicon.svg` holds both halves and switches with `prefers-color-scheme`. `favicon-32.svg` is the symbol for 32 px. |
| One-colour small mark | `mark-24.svg` | | 24 px and below in one colour: the waking page's footer, the scan report and status page. |

## Which ground

- The colour lockup goes on Paper, white or Lamp.
- The dark lockup goes on Night.
- On anything else, one colour: Night or Paper, whichever reads. On Coat, use `symbol-on-coat.svg`.

## Clear space

Keep clear, on every side of a lockup, the height of the porter's hat at that size: about a third of the symbol's height. Nothing else, text included, goes inside it. [`logo-rules/clear-space.svg`](logo-rules/clear-space.svg) shows it.

## Minimum sizes

| Version | Smallest |
|---|---|
| Horizontal lockup | 100 px wide |
| Stacked lockup | 64 px wide |
| Symbol | 24 px |
| Below 24 px | the 16-pixel cut (`favicon-16.svg`, `favicon-16-dark.svg`); never a scaled-down symbol |

At 16 px the brim, 12 units wider than the face on each side, still reads as a hat, not the lid of a jar or a bin.

## Construction

[`logo-rules/symbol-construction.svg`](logo-rules/symbol-construction.svg) and [`wordmark-construction.svg`](logo-rules/wordmark-construction.svg) show it.

- **Symbol:** a 96 grid. The hat tilts −5°; its brim is 68 wide, 12 past each side of the face. The face is 44 wide, the collar 50, the shoulders 72, cut by the bottom edge. Eyes: radius 7.5, centres 19.4 apart (0.17 and 0.44 of the face's width, as on the full figure). Two brass buttons and a braid tab on the shoulders.
- **Wordmark:** filled outlines, drawn to sit with Big Shoulders Display, not typed in it. x-height 60, stems 12, ascender 22, descender 20. Every counter is a door arch (round top, flat bottom); the n is the open door. The a's bowl meets its stem below the top so the stem reads when small; the k's arm and leg end flat on the x-height and the baseline.
- **Lockups:** in the horizontal lockup the symbol runs from the ascender's top to the baseline; in the stacked one it sits centred over the wordmark at 1.5 times the size.

## Misuses

Never:

- Give him a mouth, a smile, blush or eyebrows. He's calm, not cute. (`misuse-cute.svg`)
- Give him a pillbox hat or a bow tie: that's another open-source project's cat, CNCF Porter's. (`misuse-pillbox.svg`)
- Stretch, squash or re-colour the lockup outside the palette; never a gradient, never purple-to-blue. (`misuse-stretch.svg`)
- Use a pose, a different expression or a different hat as the logo.
- Set "napwake" in a font in place of the drawn wordmark.
- Put the colour lockup on Coat, a photo or a busy picture: use one colour there.
- Rotate it, outline it, add a shadow, or give it the illustrations' print finish.
- Use a lone arch as the mark (Notary Project's mark is an n-shaped arch in a square) or add a lantern (Headlamp's mark is one).

The misuse files in [`logo-rules/`](logo-rules/) show what not to do. Never use them as logos.

## Marks and licences

"Napwake", the logo and wordmark, and the porter's head as used in the logo are the project's marks, owned by Tobi Okedeji and governed by [TRADEMARKS.md](../TRADEMARKS.md): use them unchanged to refer to Napwake, never as the name or logo of something else. The porter's illustrations (poses, door scenes, stickers) are licensed [CC BY 4.0](../illustrations/LICENSE), as the Go gopher is, so anyone can use them with the credit "Night porter illustrations by Napwake, CC BY 4.0".
