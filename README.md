# SpiderPi Documentation

This repository contains the SpiderPi VitePress documentation site. The
documentation source files are Markdown files under `docs/docs/`.

## Local development

Install dependencies and start the local documentation server:

```bash
npm ci
npm run docs:dev
```

Build the production site:

```bash
npm run docs:build
```

The production files are generated in `docs/.vitepress/dist/`.

## GitHub Pages deployment

Build and stage the static site before pushing:

```bash
npm run docs:build
npm run docs:stage-main
```

Commit the generated `projects/` directory to `main`. For a repository named
`SpiderPi-vite`, the GitHub Pages URL is:

```text
https://GITHUB-USERNAME.github.io/SpiderPi-vite/projects/SpiderPi/en/latest/
```

Open **Settings > Pages**, select **Deploy from a branch**, and choose
**main** and **/(root)**.

When a custom domain is configured later, the same site path becomes:

```text
https://wiki.hiwonder.com/projects/SpiderPi/en/latest/
```
