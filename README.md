# Yongxue Xu · Academic Homepage

A minimal, bilingual academic homepage with publications, news, honors and education. This repository is maintained independently from [the original homepage](https://jerrysnow.me/).

## Update the homepage

- Edit `content.json` for biography, news, papers and awards.
- Run `python3 build.py` to regenerate the page.
- Edit `dist/style.css` for appearance and `dist/site.js` for interactions.
- Keep figures, the transparent portrait and downloadable CVs in `dist/assets/`.

Preview locally:

```sh
python3 build.py
python3 -m http.server 8765 --directory dist
```

Every push to `main` automatically rebuilds and publishes the homepage with GitHub Pages. All asset paths are relative, so it also works under a project subdirectory.

## Design references

The typography, profile sidebar, oval portrait frame and News styling follow [Maolin Wang](https://morin.wang/). The original reference stylesheet is retained as `dist/morin-base.css`. Compact publication rows and thumbnail shadows are inspired by [Yue Ma](https://mayuelala.github.io/). Biographical information and paper content belong to Yongxue Xu.

The CV PDFs are copies from the original homepage and are maintained separately from `content.json`.
