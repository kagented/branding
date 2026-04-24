# branding

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
│   │   └── via-logo-mark.svg   Triangle only, for favicons / small sizes
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

## Taglines

- Dark: 어둠 속에서 발견한 명확한 통찰의 에너지
- Light: 정밀한 분석이 설계한 압도적 신뢰의 가치
