# zhaorui-bi.github.io

[![Deploy GitHub Pages](https://github.com/zhaorui-bi/zhaorui-bi.github.io/actions/workflows/pages.yml/badge.svg)](https://github.com/zhaorui-bi/zhaorui-bi.github.io/actions/workflows/pages.yml)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-2ea44f?logo=github)](https://zhaorui-bi.github.io)
[![Jekyll](https://img.shields.io/badge/Built%20with-Jekyll-cc0000?logo=jekyll)](https://jekyllrb.com/)

Personal academic homepage of **Zhaorui (Elijah) JIANG**, hosted with GitHub Pages and built as a lightweight Jekyll site.

The site highlights research interests, publications, academic updates, education, research experience, industry experience, and acknowledgements.

**Live site:** [https://zhaorui-bi.github.io](https://zhaorui-bi.github.io)

## Overview

This repository contains the source code for a single-page academic portfolio. The design is intentionally lightweight: static HTML, one Jekyll layout, one global stylesheet, and image assets stored directly in the repository.

The homepage currently includes:

- A profile header with contact links
- Recent academic and research news
- Selected publications and project links
- Education history
- Research and internship experience
- Industry experience
- Mentor and collaborator acknowledgements

## Tech Stack

| Layer | Tooling |
| --- | --- |
| Site generator | Jekyll |
| Hosting | GitHub Pages |
| Styling | Custom CSS |
| Icons | Lucide |
| Deployment | GitHub Actions |

## Repository Structure

```text
.
|-- index.html                  # Homepage content with Jekyll front matter
|-- _layouts/
|   `-- default.html            # Base layout, navigation, metadata, and footer
|-- css/
|   `-- main.css                # Global styles and responsive layout rules
|-- img/                        # Portraits, logos, paper figures, and static assets
|-- _config.yml                 # Jekyll configuration
`-- .github/workflows/pages.yml # GitHub Pages build and deployment workflow
```

## Local Development

Install Jekyll if it is not already available:

```bash
gem install jekyll bundler
```

Run the site locally:

```bash
jekyll serve --livereload
```

Open the local preview:

```text
http://127.0.0.1:4000
```

Opening `index.html` directly in a browser is not recommended because the browser will not process Jekyll layouts or front matter.

## Editing Guide

Most routine updates can be made in a small number of files:

| Task | File |
| --- | --- |
| Update profile, news, publications, education, or experience | `index.html` |
| Update navigation, metadata, footer, or external scripts | `_layouts/default.html` |
| Update colors, spacing, typography, or responsive behavior | `css/main.css` |
| Add portraits, logos, or paper figures | `img/` |
| Adjust GitHub Pages build behavior | `.github/workflows/pages.yml` |

When adding new image assets, reference them from HTML with an absolute path such as:

```html
<img src="/img/example.png" alt="Descriptive alt text">
```

## Deployment

The site is deployed automatically through GitHub Actions.

1. Commit changes locally.
2. Push to the `master` branch.
3. The `Deploy GitHub Pages` workflow builds the Jekyll site.
4. GitHub Pages publishes the generated output.

The workflow can also be triggered manually from the repository's GitHub Actions page.

## Maintenance Checklist

- Keep news items in reverse chronological order.
- Keep navigation anchors aligned with section `id` values.
- Use descriptive `alt` text for all meaningful images.
- Compress large portraits, logos, and paper figures before committing.
- Check external links after publication and profile updates.
- Review `_layouts/default.html` when updating personal metadata, contact links, or copyright year.

## Contact

- Website: [https://zhaorui-bi.github.io](https://zhaorui-bi.github.io)
- GitHub: [zhaorui-bi](https://github.com/zhaorui-bi)
- LinkedIn: [Zhaorui Jiang](https://www.linkedin.com/in/zhaorui-jiang-a91201341/)
