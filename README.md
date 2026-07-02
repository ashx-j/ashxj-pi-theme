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

## License

MIT
