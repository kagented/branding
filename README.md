# branding

| Dark Mode | Light Mode |
| :---: | :---: |
| <img src="assets/logo/via-logo-dark.svg" alt="VIA logo — dark mode" width="240"> | <img src="assets/logo/via-logo-light.svg" alt="VIA logo — light mode" width="240"> |
| Momentum,<br>toward The Essence | The Essence —<br>made Vivid |

Experimental brand development for **VIA**.

## Concept

Three concentric layers narrowing to an insight:

- **EXTERNAL** — dashed outer arc → phenomena
- **INTERNAL** — solid inner arc → analysis
- **IDEA** — triangle core → insight

## Structure

```
branding/
├── assets/
│   ├── logo/
│   │   ├── via-logo.svg        Full mark (triangle + both arcs), uses currentColor
│   │   ├── via-logo-mark.svg   Triangle only, for favicons / small sizes
│   │   ├── via-logo-dark.svg   Pre-colored preview (white on #0a0a0a) for README / GitHub
│   │   └── via-logo-light.svg  Pre-colored preview (black on #f8f8f8) for README / GitHub
│   └── tokens/
│       └── colors.css          --via-dark-bg / --via-dark-fg / --via-light-bg / --via-light-fg
├── examples/
│   └── usage.html              Drop-in usage across dark / light / accent backgrounds
└── via_logo.html               Original dual-pane preview (reference)
```

## Usage

The SVGs use `stroke="currentColor"`, so they inherit their parent's `color`:

```html
<link rel="stylesheet" href="branding/assets/tokens/colors.css">
<div style="color: var(--via-dark-fg); background: var(--via-dark-bg);">
  <img src="branding/assets/logo/via-logo.svg" alt="VIA" width="120">
</div>
```

Inline SVG also works and lets CSS retarget the color per context.
