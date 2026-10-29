# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project overview

A static website about horses, written in plain HTML and CSS. There is no build step, package manager, framework, linter, or test suite, and the directory is not a git repository.

- `index.html` is the only page. It is laid out as `header` > `main` (made of `section`s) > `footer`.
- `styles.css` is the single stylesheet, linked from `index.html`. It is currently empty.
- `.vscode/settings.json` holds only editor colour customisations and has no effect on the site.

## Running

Open `index.html` directly in a browser, or serve the directory with any static server, for example:

```sh
python3 -m http.server 8000
```

## Conventions

- HTML is indented with tabs and uses self-closing void tags (`<meta ... />`, `<link ... />`).
- Use semantic elements (`header`, `main`, `section`, `footer`) to match the existing structure.
- New pages should copy the `<head>` from `index.html`: charset, viewport, a meta description, a title, and the `styles.css` link.
