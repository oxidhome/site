# oxidhome.info

[![Publish](https://github.com/oxidhome/site/actions/workflows/publish.yml/badge.svg)](https://github.com/oxidhome/site/actions/workflows/publish.yml)

Source for [oxidhome.info](https://oxidhome.info), the project site for **OxidHome** — an open home-automation platform
built around a Rust core and WebAssembly plugins.

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

This repository contains both written content and code samples, licensed differently.

**Written content** — articles, documentation, design notes, and diagrams — is licensed
under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE-CC-BY-4.0).

You are free to share and adapt this content for any purpose, including commercially, as long as you give appropriate
credit. A suggested attribution is:

> *"Article Title"* by OxidHome Contributors, from the OxidHome documentation, licensed
> under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

**Code samples** — code blocks within articles, example projects, and any scripts or tooling — are dual-licensed under
either of:

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
  http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or
  http://opensource.org/licenses/MIT)

at your option. This matches the licensing of the [main OxidHome codebase](https://github.com/oxidhome/oxidhome).

## Contribution

Contributions are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in this repository shall
be:

- Licensed under **CC BY 4.0** if it is written content (articles, prose, diagrams)
- Dual-licensed under **MIT and Apache-2.0** if it is code (samples, examples, scripts), as defined in the Apache-2.0
  license

without any additional terms or conditions.
