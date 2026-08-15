# secha.dev

Landing page for [secha](https://github.com/Thran34/secha), a security chaos engineering tool for
Kubernetes.

A single static page. No build step, no dependencies, no JavaScript — open `index.html` in a browser
and it renders exactly as it will in production.

## Files

| file | purpose |
|---|---|
| `index.html` | the page: markup, styles, and the shield mark inline |
| `CNAME` | tells GitHub Pages to serve the site at `secha.dev` |
| `logo.png` | favicon, and the source artwork the inline mark is drawn from |

## Editing

Colours and spacing come from CSS custom properties defined at the top of `index.html`. Every token is
declared three times so the page holds in all three viewer states: the bare `:root` block covers light,
a `prefers-color-scheme: dark` block covers a dark OS with no explicit choice, and a `[data-theme="dark"]`
block covers an explicit toggle. Change a colour once in each of those three places, never inside a
component rule.

To preview the dark theme without changing your OS setting, add `data-theme="dark"` to the `<html>` tag.

## Numbers on this page

The measurements shown in the demo readout are real output from `secha demo`, not illustrations. If the
tool's behaviour changes, update them here too.
