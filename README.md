# hosambadawi.github.io

Personal site for **Hosam Mahmoud Ibrahim** — AI Systems Architect & Agentic AI Engineer.

**Live:** https://hosambadawi.github.io/

## What's here

Single-page portfolio, no build step. Everything is a static file — GitHub Pages
serves it as-is.

```
index.html      the entire site (inline CSS + JS, inline SVG diagrams)
images/         profile photo (optimised .jpg used by the page)
fonts/          self-hosted Inter + JetBrains Mono subsets
```

## Notes

- **No dependencies, no build.** Edit `index.html` and push; the change is live.
- **Fonts are self-hosted** rather than loaded from Google Fonts — no third-party
  request, no layout shift, works offline.
- **Architecture diagrams are inline SVG** and inherit the CSS colour variables,
  so re-theming the page re-themes the diagrams.
- **Calendly loads lazily** when the contact section comes into view, and falls
  back to a plain link if the widget fails.
- Accessibility: single `<h1>`, no skipped heading levels, all text meets WCAG AA
  contrast, decorative SVGs are `aria-hidden`, animation respects
  `prefers-reduced-motion`, and content stays visible with JavaScript disabled.

## Editing the common bits

| What | Where |
|---|---|
| Colours, spacing, radii | `:root` block at the top of the `<style>` |
| Booking link | search for `calendly.com/hosam_mahmoud` |
| Repo cards | the `.repos` grid in the *Open source* section |
| Diagrams | the two `<svg>` blocks inside `.case-diagram` |
