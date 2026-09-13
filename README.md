# Feynman — brand marks

Two images, and nothing else.

This repository is public for one reason: Cloudflare Access takes a **URL** for
the logo on its sign-in page, and the browser fetches that URL while drawing the
page — before anybody has signed in. The Feynman site itself sits behind that
sign-in, so an image hosted there could only be seen by somebody who had already
got past the page it belongs to. It has to be served from somewhere with no
login in front of it, and this is that somewhere.

Nothing else belongs in here. No source, no configuration, no documents.

## The files

| File | Size | Use |
| --- | --- | --- |
| `feynman-name.png` | 2800×840 | The word on its own, transparent ground. **This is the one the sign-in page uses** — that slot renders small, so a second line inside the image would be unreadable. |
| `feynman-wordmark.png` | 2800×920 | Both lines locked up together, for anywhere the mark is shown large. |

Ubuntu Bold, letter-spacing tightened, with a steel gradient through the
letterforms. Intended for a dark ground — `#0b0e12` is the one they were made
against.

## The address

```
https://raw.githubusercontent.com/Joshd667/feynman-brand/main/feynman-name.png
```

Served as `image/png` with `Access-Control-Allow-Origin: *`, cached for five
minutes — so a replacement takes up to five minutes to show up.

The masters live with the product, in the private repository at
`docs/self-hosted-web/brand/`. Change them there first; this is a copy that
exists to be fetched.
