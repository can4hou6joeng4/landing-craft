# Landing Craft

A [Claude Code](https://claude.ai/claude-code) skill that generates **visually striking landing pages** with 57 city-inspired design systems.

> Not your typical card-grid template. Every output is a design artifact — clip-path dividers, GSAP scroll animations, SVG textures, real depth and layering.

## What It Does

Tell the skill about your product. It opens an interactive browser preview of **57 city-inspired visual styles** — from Kyoto to Lagos to Palm Springs — and lets you click to select. Then it generates a complete multi-file site with real product copy.

```
your-product-landing/
├── index.html      # Full page with nav, sections, footer
├── style.css       # Design tokens, textures, clip-paths
├── main.js         # GSAP ScrollTrigger animations
└── assets/
    └── icons.svg   # SVG sprite matching the city aesthetic
```

## Features

- **57 city aesthetics** — each with unique fonts, colors, textures, motion, and icon style
- **Interactive preview** — browser-based card picker (no CLI menu)
- **7 hero variants** — full-screen, split, minimal, product demo, typography-led, magazine, pop card
- **6 feature layouts** — big numbers, alternating showcase, timeline, bento grid, horizontal scroll, FAQ
- **6 testimonial styles** — compact grid, magazine, masonry, horizontal scroll, chat bubbles, avatar wall
- **4 nav archetypes** — full-screen blast, magnetic pill, vertical side rail, split centered
- **3 color tones** — original city, dark luxe, bright modern
- **Multi-page support** — optional About, Contact, Blog sub-pages sharing the same design system
- **3 form sections** — newsletter subscribe, waitlist signup, inline contact form
- **Transition picker** — geometric / organic / blend / minimal section dividers
- **One-click deploy** — optional Netlify deployment with preview URL, then production
- **Python 3.6+ compatible** — works on macOS default Python (3.9)
- **Cross-platform** — Python launcher + PowerShell fallback for Windows

## Quick Start

This is a Claude Code skill. Install it globally:

```bash
npx skills add can4hou6joeng4/landing-craft -a claude-code -g -y
```

Then just say:

> "帮我做一个落地页"

or

> "Build me a landing page for my product"

## Trigger Phrases

The skill activates on: `帮我做一个落地页`, `做个首页`, `产品展示页`, `活动页`, `营销页`, `官网首页`, `landing page`, `product page`, `promo page`, `make me a homepage`, `build a product showcase`, `create a campaign page`.

## Workflow

1. **Describe your product** — name + one-line intro
2. **Pick a city style** — 57 cards rendered live in your browser
3. **Choose options** — typography, nav, color tone, transitions, hero/features variants
4. **Get your site** — complete `index.html` + `style.css` + `main.js` + `icons.svg`
5. **Preview** — auto-opens in your browser
6. **Deploy** — optional one-click publish to Netlify with preview URL

## Project Structure

```
├── SKILL.md                              # Skill definition (Claude Code reads this)
├── assets/
│   ├── style-preview-template.html       # 57-city interactive picker
│   ├── options-preview-template.html     # Layout/nav/color/transition chooser
│   ├── clip-paths.css                    # Section divider library
│   ├── gsap-snippets.js                  # Proven GSAP animation patterns
│   ├── textures.css                      # CSS-only background textures
│   ├── sections/                         # Pre-built section HTML variants
│   │   ├── hero-variants.html            # 7 hero templates (A-G)
│   │   ├── features-variants.html        # 6 feature templates (A-F)
│   │   ├── testimonial-variants.html     # 6 testimonial templates (A-F)
│   │   └── conversion-variants.html      # Pricing, FAQ, CTA, Brand Wall
│   └── scripts/
│       ├── run_preview.py                # Cross-platform preview launcher
│       ├── run_preview.ps1               # Windows PowerShell equivalent
│       ├── get_city_tokens.py            # Extract city color tokens
│       └── extract_variant.py            # Extract section variant by ID
├── references/
│   ├── city-styles.md                    # 57 city design parameters
│   ├── nav-catalog.md                    # 4 nav style implementations
│   ├── imagery-derivation.md             # Non-city description → tokens
│   └── product-demo-hero.md              # Product demo hero guide
└── evals/
    └── evals.json                        # Skill evaluation test cases
```

## Design Philosophy

- **No `#ffffff` backgrounds** — warm neutrals, cool tints, or deep darks
- **Two typefaces minimum** — display/serif headlines + clean sans body
- **SVG as design core** — not decorative sprinkles
- **GSAP depth** — parallax layers, sticky panels, staggered reveals
- **No clone grids** — every repeating section has visual hierarchy, not identical rows

## License

[MIT](LICENSE)
