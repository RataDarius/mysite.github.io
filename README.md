# mysite.github.io

Personal portfolio site — hand-written HTML and CSS, served by GitHub Pages.
No framework, no build step, nothing to break at deploy time.

**Live:** https://ratadarius.github.io/mysite.github.io/

---

## Layout

```
docs/
  index.html        the whole site
  rata.png          portrait
  3-wheel-car.jpg   project photo
  certificates/     certificate PDFs
```

`docs/` is the Pages source branch — every commit to `main` goes live within a
minute or so.

## Sections

One page, five sections: hero, focus areas, projects, certificates, about,
contact. All navigation is in-page anchors; there is no routing.

## Working on it locally

The site is fully static, so you can just open the file:

```bash
open docs/index.html
```

To preview it exactly as Pages serves it, run a server from inside `docs/`:

```bash
python3 -m http.server 8000 --directory docs
```

## Notes

- Certificate links are relative (`certificates/…`) so they keep working if the
  repository is renamed or Pages is ever moved to a root-level site.
- The certificate filenames are plain ASCII on purpose — an earlier version used
  a Romanian `ț` that was stored decomposed (as `t` plus a combining character)
  and silently 404'd.
- Fonts come from Google Fonts via a `<link>`, so the page needs a network
  connection to render with Inter; the fallback stack still looks fine.
