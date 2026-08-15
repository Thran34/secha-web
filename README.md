# secha.dev

Landing page for [secha](https://github.com/Thran34/secha), a security chaos engineering tool for
Kubernetes.

A single static page. No build step, no dependencies, no JavaScript — open `index.html` in a browser
and it renders exactly as it will in production.

## Files

| file | purpose |
|---|---|
| `index.html` | the page: markup and styles, no build step |
| `CNAME` | tells GitHub Pages to serve the site at `secha.dev` |
| `logo.svg` | the canonical mark — favicon and nav |
| `logo.png` | raster fallback, rendered from `logo.svg` |

## Design

The page commits to one look rather than following the viewer's theme: a dark instrument panel, because
the subject is a signal that goes missing. `color-scheme: dark` is declared and every colour is painted
explicitly, so the page holds whatever ground the browser puts behind it.

Three roles carry the type. A heavy uppercase sans does the talking, monospace does the measuring — it
appears only where real data does, in the readout and the commands — and the amber accent marks one
thing per screen. Red and green are reserved for measured outcomes and never used as decoration.

All colours and both fonts are CSS custom properties at the top of `index.html`. Change them there,
never inside a component rule.

Layout note: `.wrap` owns the horizontal padding. A child that also sets the `padding` shorthand will
silently cancel it — use `padding-block` instead.

## Numbers on this page

The measurements shown in the demo readout are real output from `secha demo`, not illustrations. If the
tool's behaviour changes, update them here too.

## Logo

`logo.svg` is the canonical mark and is byte-identical to the copy in the
[secha](https://github.com/Thran34/secha) repository. It carries no background, so it sits on a light
or dark ground unchanged. `logo.png` is rendered from it for places that will not take an SVG.

Change the mark in one repository and copy it to the other — never edit one copy alone.
