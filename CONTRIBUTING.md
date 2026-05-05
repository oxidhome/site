# Contributing to OxidHome Docs

Thanks for your interest in contributing to OxidHome's documentation. This repo holds articles, design notes, tutorials, architecture documentation, and other written content for the project.

For changes to the core platform code, see [`oxidhome/oxidhome`](https://github.com/oxidhome/oxidhome). For plugins, see [`oxidhome/plugins`](https://github.com/oxidhome/plugins).

## What belongs here

- **Articles** — tutorials, deep dives, design rationales, how-tos
- **Architecture documentation** — design decisions, ADRs, technical specs
- **API reference material** — generated where possible, hand-written where useful
- **Diagrams and visual content** — architecture diagrams, flow charts, illustrations
- **Translations** — of any of the above

What does **not** belong here:

- Code that's part of the platform (goes in [`oxidhome/oxidhome`](https://github.com/oxidhome/oxidhome))
- Plugin source code (goes in [`oxidhome/plugins`](https://github.com/oxidhome/plugins))
- Reference documentation that should live next to the code it describes (rustdoc)

Code samples *embedded in articles* are fine and expected — they're part of the article.

## How to contribute

### Reporting issues

Open an issue if you find:

- Mistakes (factual errors, broken examples, outdated information)
- Missing documentation for things that should be documented
- Confusing explanations
- Broken links

### Suggesting articles

Open an issue with:

- The topic you'd like to write about
- Roughly what it would cover
- The intended audience (new users, plugin authors, contributors)

This helps avoid duplicate work and lets us flag any topics that overlap with planned content.

### Submitting written content

1. **Fork and branch** from `main`. Use a descriptive branch name.
2. **Write the content.** See the style guide below.
3. **Verify code samples actually work.** Articles with broken examples are worse than no article.
4. **Open a pull request** with a brief description of the article and who it's for.

PR reviews focus on accuracy, clarity, and consistency with the rest of the documentation.

## Style guide

OxidHome docs aim to be **accurate, direct, and respectful of the reader's time**.

### Tone

- Write to a developer who's smart but new to OxidHome (or to the topic). Don't talk down.
- Explain *why*, not just *what*. The reasoning behind a design decision is often more useful than the decision itself.
- Be honest about limitations. "OxidHome can't do X yet" is better than vague hedging.
- Avoid hype. Don't oversell features or call things "blazing fast" without numbers to back it up.

### Structure

- Lead with the conclusion or the main idea, then unpack it.
- Use headings to make articles scannable.
- Keep paragraphs short. Long walls of text are hard to read on phones.
- Code samples should be runnable when possible. If a sample is illustrative only, say so.

### Accuracy

- Verify every claim. If you're not sure something is correct, either check or remove it.
- Link to authoritative sources for non-obvious facts (specs, RFCs, vendor documentation).
- If something might change (a Wasmtime API, a Cargo feature flag), note the version it applies to.
- When you reference architectural decisions, link to [`ARCHITECTURE.md`](https://github.com/oxidhome/oxidhome/blob/main/ARCHITECTURE.md) in the main repo.

### Code samples

- Use proper syntax highlighting (` ```rust`, ` ```toml`, ` ```wit`, etc.).
- Keep samples minimal — show the relevant lines, not a hundred lines of boilerplate.
- If a sample needs context (imports, surrounding code), include it once and reference it.
- Don't paste code without explaining what it does.

### Diagrams

- SVG preferred (text-searchable, scales well, works on dark mode).
- Source files for diagrams (e.g., `.excalidraw`, `.drawio`) should be committed alongside the rendered version when practical, so others can edit them.
- Keep diagrams simple. A diagram with 30 boxes and 50 arrows is usually better as two diagrams.

### Per-article footers

Each standalone article should end with an attribution footer so it can be republished cleanly:

```markdown
---

*Part of the OxidHome documentation. © {year} OxidHome Contributors. Articles licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); code samples dual-licensed under [MIT](https://github.com/oxidhome/docs/blob/main/LICENSE-MIT) and [Apache-2.0](https://github.com/oxidhome/docs/blob/main/LICENSE-APACHE).*
```

## Licensing of contributions

This repository contains content under two different licenses. By contributing, you agree to both:

### Written content

Articles, prose, design notes, diagrams, and other written or visual content are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE-CC-BY-4.0).

Unless you explicitly state otherwise, written content you contribute is licensed under CC BY 4.0.

### Code samples

Code blocks within articles, example projects, and any scripts or tooling are dual-licensed under [MIT](LICENSE-MIT) and [Apache-2.0](LICENSE-APACHE), matching the main OxidHome codebase.

Unless you explicitly state otherwise, code you contribute is dual-licensed under MIT and Apache-2.0, without any additional terms or conditions.

If your contribution includes content that you cannot license under these terms (for example, third-party diagrams used with permission, or screenshots from copyrighted sources), declare it in the contribution and ensure the source is attributed and the use is legitimate.

## Code of conduct

Be respectful, be patient, assume good faith. The maintainers reserve the right to remove comments, close issues, or restrict participation if needed to keep the project healthy.

## Questions

For questions about an article you're considering writing, or about how the docs are organized, open an issue or a GitHub Discussion.
