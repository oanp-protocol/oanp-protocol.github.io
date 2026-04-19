# oanp.dev

Documentation site for the Open Agent Negotiation Protocol, served via GitHub Pages at [oanp.dev](https://oanp.dev).

Single-file HTML with inlined CSS + hash-based routing between pages. No build step.

## Structure

`index.html` contains all pages as `<article class="page" data-page-id="...">` sections. Client-side JS (end of file) swaps the active page on sidebar clicks and updates the URL hash. Theme toggle (light / dark) persists via `localStorage`.

Sections with full content: intro, three-role-model, commitments, fairness-invariants, message-format, coexistence. Remaining sections render "Coming soon" cards. When a section graduates to full content, edit its `<article>` block.

## Deploy

Pushes to `main` publish automatically via GitHub Pages.

## Custom domain

`CNAME` file points the site at `oanp.dev`. DNS configuration lives at the registrar (GoDaddy).

Required DNS records:

```
Type   Host   Value
A      @      185.199.108.153
A      @      185.199.109.153
A      @      185.199.110.153
A      @      185.199.111.153
CNAME  www    oanp-protocol.github.io
```

## License

Apache 2.0.
