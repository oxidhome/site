# oxidhome.info

[![Publish](https://github.com/oxidhome/site/actions/workflows/publish.yml/badge.svg)](https://github.com/oxidhome/site/actions/workflows/publish.yml)

Source for [oxidhome.info](https://oxidhome.info), the project site for **OxidHome** — an open home-automation platform built around a Rust core and WebAssembly plugins.

The site is a static [Zola](https://www.getzola.org/) build deployed to GitHub Pages on every push to `main`.

## Local development

```sh
zola serve
```

Then open http://127.0.0.1:1111.

## Layout

- `content/` — markdown for each page and section
- `templates/` — Tera templates (`base.html`, `index.html`, `section.html`, `404.html`)
- `static/` — assets copied verbatim into the published site (`site.css`, logos, favicon)
- `zola.toml` — site configuration

## License

Code is dual-licensed under [MIT](LICENSE-MIT) **or** [Apache 2.0](LICENSE-APACHE) at your option. Site content is licensed under [CC BY 4.0](LICENSE-content).
