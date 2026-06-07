# Krimler

A [Quarto](https://quarto.org) website on math, CS, AI/ML, and security.
Hosted free on GitHub Pages.

## Daily workflow

```bash
quarto preview          # live local preview at http://localhost:xxxx
quarto publish gh-pages # build + push the live site
```

## Add a blog post

```bash
mkdir posts/my-post
$EDITOR posts/my-post/index.qmd   # copy the front matter from posts/welcome/
```

Use `$math$` for math, fenced ```` ```python ```` blocks for code, and
`[@bibkey]` for citations (add the entry to `references.bib`).

## Add a paper (PDF)

1. Put the PDF in `papers/files/`.
2. Copy `papers/_template.qmd` → `papers/my-paper.qmd` and edit the front matter.

## Cite an arXiv paper

Open the arXiv page → **Export BibTeX citation** → paste into `references.bib`,
then cite with `[@thatkey]`.
