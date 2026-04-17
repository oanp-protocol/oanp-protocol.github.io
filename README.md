# oanp.dev

Static landing page for the Open Agent Negotiation Protocol, served via GitHub Pages at [oanp.dev](https://oanp.dev).

Single-file HTML with inlined CSS. No build step.

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
