# mysite.github.io

Personal portfolio site — hand-written HTML and CSS, served by GitHub Pages.
No framework, no build step.

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

`docs/` is the Pages source directory — every commit to `main` goes live within a
minute or so.

## Working on it locally

The site is fully static, so you can open the file directly:

```bash
open docs/index.html
```

Or serve it the way Pages does:

```bash
python3 -m http.server 8000 --directory docs
```
