# Feynman — brand marks

Four images, and nothing else.

This repository is public for one reason: Cloudflare Access takes a **URL** for
the logo on its sign-in page, and the browser fetches that URL while drawing the
page — before anybody has signed in. The Feynman site itself sits behind that
sign-in, so an image hosted there could only be seen by somebody who had already
got past the page it belongs to. It has to be served from somewhere with no
login in front of it, and this is that somewhere.

Nothing else belongs in here. No source, no configuration, no documents.

## The files

Each mark comes in two versions, because a mark that reads on one ground
disappears on the other. The plain name is the one for a **light** ground, which
is what Cloudflare draws its sign-in card on.

| File | Ground | Size | Use |
| --- | --- | --- | --- |
| `feynman-name.png` | light | 2800×840 | **The sign-in page uses this one.** The word alone, in the brand navy. That slot renders small, so a second line inside the image would be unreadable — it goes in Cloudflare's Header text field instead. |
| `feynman-name-on-dark.png` | dark | 2800×840 | The same word in pale steel, for a dark ground. |
| `feynman-wordmark.png` | light | 2800×920 | Both lines locked up, navy, for anywhere the mark is shown large. |
| `feynman-wordmark-on-dark.png` | dark | 2800×920 | The same lockup in pale steel. |

Ubuntu Bold with the letter-spacing tightened, over a slight gradient; the
second line is JetBrains Mono, wide-tracked. The light versions are the brand
navy `#1e3664`, the dark versions a steel `#dfe6ee` made against `#0b0e12`. All
four have transparent backgrounds.

## The address

```
https://raw.githubusercontent.com/Joshd667/feynman-brand/main/feynman-name.png
```

Served as `image/png` with `Access-Control-Allow-Origin: *`, cached for five
minutes — so a replacement takes up to five minutes to appear.

The masters live with the product, in the private repository at
`docs/self-hosted-web/brand/`. Change them there first; this is a copy that
exists to be fetched.
