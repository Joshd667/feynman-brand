# Feynman — brand marks

Images, and nothing else.

This repository is public for one reason: Cloudflare Access takes a **URL** for
the logo on its sign-in page, and the browser fetches that URL while drawing the
page — before anybody has signed in. The Feynman site itself sits behind that
sign-in, so an image hosted there could only be seen by somebody who had already
got past the page it belongs to. It has to be served from somewhere with no
login in front of it, and this is that somewhere.

Nothing else belongs in here. No source, no configuration, no documents.

## The marks

Each Feynman mark comes in versions for a light and a dark ground, because one
that reads on one disappears on the other. **The plain filename is the light
version**, which is what Cloudflare draws its sign-in card on.

| File | Ground | Use |
| --- | --- | --- |
| `feynman-name-gc.png` | light | The word in Godalming College's master blue `#0F2C60`. |
| `feynman-name.png` | light | The word in the product's own navy `#1e3664`. |
| `feynman-name-on-dark.png` | dark | The same word in pale steel. |
| `feynman-wordmark.png` / `-on-dark.png` | light / dark | Both lines locked up, for where the mark is shown large. |
| `gc-masterlogo.png` | light | Godalming College's master logo, unmodified. |
| `gc-shield.png` | light | The college shield, unmodified. |
| `favicon.png` | — | The shield at 256×256, as the site's browser-tab icon. |

Ubuntu Bold with the letter-spacing tightened, over a slight gradient; the
second line is JetBrains Mono, wide-tracked. All have transparent backgrounds.

## The college palette

Taken from the master artwork rather than transcribed from a document, so these
are the values the logos and patterns are actually drawn in.

| | Hex |
| --- | --- |
| Master blue | `#0F2C60` |
| Bright blue | `#066CBF` |
| Light blue | `#0A99E0` |
| Mint | `#39D3A7` |
| Yellow | `#FFC900` |
| Orange | `#FF682C` |
| Magenta | `#9E1685` |
| Pale tint | `#EDF0FC` |

## The address

```
https://raw.githubusercontent.com/Joshd667/feynman-brand/main/<file>
```

Served as `image/png` with `Access-Control-Allow-Origin: *`, cached for five
minutes — so a replacement takes up to five minutes to appear.

The masters live with the product, in the private repository at
`docs/self-hosted-web/brand/`. Change them there first; this is a copy that
exists to be fetched.

The two `gc-` files are Godalming College's own artwork, reproduced here for the
college's own sign-in page.
