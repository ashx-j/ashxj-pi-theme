# ashxj

A muted sage dark theme for the [pi coding agent](https://github.com/earendil-works/pi).

Low-saturation, earthy, calm. The accent is a dusty sage green; the surface
hierarchy is built from very dark warm grays. Semantic colors (success, error,
warning) are tuned to harmonize with the sage instead of clashing with it.

## Palette

| Role | Hex |
|---|---|
| Accent | `#a9b8a8` (logo, selected items, cursor, spinner) |
| Border | `#5c6e59` (dark sage) |
| Border accent | `#9fbc9a` (light sage, for focused borders) |
| Muted | `#808080` (secondary text, quotes, hrs) |
| Success | `#79a776` (dusty green) |
| Error | `#c35555` (warm red) |
| Warning | `#dfc958` (warm gold) |
| Heading | `#f0c674` (kept warm gold for visual hierarchy) |

Dark surface hierarchy (top → bottom of the stack):
`#1a1a1a` custom message bg → `#1f1f1f` selected/tool pending → `#171717`
user message bg → `#242924` tool success (slight green tint) → `#2c2626`
tool error (slight red tint).

`text`, `userMessageText`, and `customMessageText` are intentionally empty
(`""`) so they fall back to the terminal's default foreground — lets your
terminal config decide what reads best.

## Install

Add this repo's directory to your pi themes path in
`~/.pi/agent/settings.json`:

```json
{
  "themes": [
    "C:/path/to/ashxj-pi-theme"
  ]
}
```

Then either edit `"theme": "ashxj"` in the same file, or use `/theme ashxj`
inside pi. `/reload` to pick it up.

## Design notes

- **Sage over purple.** Most "muted dark" themes use a desaturated purple as
  the accent. This one uses sage green — same low-saturation philosophy,
  different hue, more organic.
- **VS Code-style syntax.** Most syntax colors are kept as-is from the built-in
  `dark` theme (`#DCDCAA` functions, `#9CDCFE` variables, `#CE9178` strings,
  etc.) so code reads familiar. Only `syntaxComment` and `syntaxKeyword` are
  retuned to the sage family.
- **Flat thinking levels.** All six `thinkingOff` → `thinkingXhigh` borders
  use the same `#6b6b6b` gray. pi switches between them as you change
  thinking level, so a single color keeps the visual change quiet.

## License

MIT
