# NUOMI Lab Website

Adapted from the following template:
* [Demo](https://YoussefRaafatNasry.github.io/portfolYOU/)
* [Documentation](https://YoussefRaafatNasry.github.io/portfolYOU/docs/)

## Editing content

These are the only files you should need to edit to update the site's content. Each is plain text/markdown or simple data fields - no HTML or layout code to worry about breaking.

| To change... | Edit this file |
|---|---|
| The About text | `_includes/content/about.md` |
| The Research text | `_includes/content/research.md` |
| The "How to join?" text | `_includes/content/joining.md` |
| People (add/remove/edit a profile) | `_data/people.yml` |
| The Resources text | `_includes/content/resources.md` |
| The Research Skills orientation page | `_includes/content/research-skills/*.md` (one file per section) |
| Publications (add/remove/edit a paper) | `_bibliography/selected_publications.md` (plain BibTeX; edited by hand, nothing regenerates it) |

For the three `content/*.md` files: write plain prose, using `**bold**`, `[link text](url)`, and blank lines between paragraphs, the same way you'd write a markdown document. Don't add HTML tags (`<div>`, `<section>`, etc.) - those live elsewhere and control the page's structure/styling, not its content.

See `CONTENT-GUIDE.md` for a fuller, non-technical walkthrough (including the BibTeX format and which optional fields control the Abs/Bib/arXiv/HTML buttons under each publication).

Everything else in this repo (`_layouts/`, `_includes/` outside of `content/`, `_sass/`, `pages/index.md` itself, `_config.yml`) controls structure, navigation, and visual design rather than content - changes there are more likely to break something, so treat those as off-limits for routine content updates.
