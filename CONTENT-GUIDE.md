# How to Update This Website

This guide is for updating the *content* of the site — the words, people, and publications — without needing to know anything about web design or code. You don't need to install anything; everything below can be done in a web browser on the GitHub website.

If you ever get stuck or something looks broken after a change, don't worry — GitHub keeps a complete history of every change ever made, so nothing is ever permanently lost. Just ask a developer to help you undo it.

---

## Quick reference: what to edit for what

| To change...                          | Edit this file |
|----------------------------------------|-----------------|
| The **About** section text             | `_includes/content/about.md` |
| The **Research** section text          | `_includes/content/research.md` |
| The **"How to join?"** section text    | `_includes/content/joining.md` |
| **People** (add, remove, or edit a profile) | `_data/people.yml` |
| **Publications** (add, remove, or edit a paper) | `_bibliography/selected_publications.md` |
| The **Resources** section text (links for students) | `_includes/content/resources.md` |
| The **Research Skills** orientation page | the files in `_includes/content/research-skills/` (one file per section of the page) |

Don't edit any file not listed above (or in the "content" folders described here) — everything else controls the site's layout, colors, and behavior, and is much easier to accidentally break.

---

## How to edit a file on GitHub

1. Go to the website's repository on GitHub (the `nuomi-lab.github.io` project page).
2. Click on the file you want to change (use the table above to find its name, and click through the folders shown before the file name — e.g. for `_data/people.yml`, click the `_data` folder first, then click `people.yml`).
3. Click the **pencil icon** (✏️) near the top-right of the file, usually labeled "Edit this file."
4. Make your change directly in the text box.
5. Scroll down to the bottom of the page. Under "Commit changes," you can leave the default message or write a short note like "update about text."
6. Click the green **Commit changes** button.
7. Wait 1–2 minutes for the website to rebuild, then refresh the live site to see your change.

That's the entire workflow for every file described below.

---

## The text sections: About, Research, How to join?, Resources

These four files each contain the paragraph text for one section of the homepage. They're plain text with a little light formatting — no HTML, no code.

**Example** — this is what `_includes/content/about.md` looks like:

```
# About

NUOMI Lab is an artificial intelligence research group at London South Bank University. Our name is short for **Normative and User-Oriented Machine Intelligence**.

We study what machine learning systems *should* do, and build them around the people who use them and are affected by them.
```

Formatting rules (all optional — plain text works fine too):

- A line starting with `#` is a big heading; a line starting with `##` is a smaller sub-heading.
- Wrapping text in `**two asterisks**` makes it **bold**.
- Wrapping text in `[brackets](and-a-url-in-parentheses)` makes it a clickable link — e.g. `[LSBU](https://www.lsbu.ac.uk)` becomes [LSBU](https://www.lsbu.ac.uk).
- Leave a completely blank line between paragraphs. Without a blank line, two lines of text will run together into one paragraph.
- Don't add anything that looks like `<div>` or `<section>` (angle brackets) — that's code, not text, and belongs to a different part of the site.

To edit: open the file, change the words, keep the same `**bold**` and `[link](url)` style if you want that formatting preserved, leave blank lines between paragraphs, and commit your change as described above.

The **Resources** section (`_includes/content/resources.md`) and the **Research Skills** page (the files in `_includes/content/research-skills/`) follow exactly the same rules. A few extras appear in those files:

- A line starting with `- ` is a bullet point, and a line starting with `1. ` is a numbered item. Indent a bullet by two spaces to nest it under the one above.
- A paragraph starting with `> ` becomes a shaded callout box (used for the "What we expect" notes).
- To add a resource, copy an existing bullet and change its text and link, e.g. `- **[Link text](https://example.com)**: a short description.`

---

## People

`_data/people.yml` controls the "People" section. It uses a format called YAML — it looks like a list of index cards, one per person.

**Example** — one person's entry looks like this:

```yaml
    - name: Weiwei Pan
      pronouns: they/them
      title: Principal Investigator
      affiliation: London South Bank University
      site: https://onefishy.github.io/
      image: /assets/img/people/weiwei-pan.png
```

A few important rules for this format:

- **Indentation (the spaces at the start of each line) matters.** Every line for one person must line up exactly like the example above. The easiest way to avoid mistakes is to **copy an existing person's entry and edit the copy**, rather than typing a new one from scratch.
- Each person's entry starts with `- name:` (a dash, then a space, then `name:`).
- Available fields for each person:
  - `name` — required.
  - `title` — their role (e.g. "PhD Student").
  - `affiliation` — their institution.
  - `site` — a link to their personal website or LinkedIn. Leave this out if they don't have one.
  - `pronouns` — optional, e.g. `she/her`.
  - `image` — a photo (see below). Leave this out entirely if you don't have one yet — the site will just show the profile without a photo.
  - `coadvisor` — optional, the name of a student's co-advisor.

### Adding a new person

Copy an entire existing entry (from the `- name:` line down to the line before the next `- name:`), paste it as a new block in the same list, and edit the details. Make sure the new block starts with `- name:` and every other line lines up with the other entries.

### Removing a person

Delete their entire block, from their `- name:` line down to (but not including) the next person's `- name:` line.

### Adding a photo

1. Get the photo file (a `.png` or `.jpg` works).
2. In the repository, go to the `assets/img/people/` folder and use GitHub's "Add file → Upload files" button to upload it.
3. In that person's entry in `_data/people.yml`, set `image:` to `/assets/img/people/` followed by the exact filename you uploaded, e.g. `image: /assets/img/people/jane-smith.jpg`.

---

## Publications

**Note:** the Publications section and its tab are currently hidden, because the lab doesn't have papers yet. Once real papers are in the file below, ask a developer to set `show_publications: true` in `_config.yml` to show them.

`_bibliography/selected_publications.md` controls the "Selected Publications" section. Each paper is one block in a citation format called BibTeX — the same format Google Scholar, Zotero, and most reference managers can export directly.

**Example** — one paper's entry looks like this:

```
@article{pan2026example,
  title     = {An Example Paper Title},
  author    = {Weiwei Pan and A. Coauthor},
  year      = {2026},
  journal   = {Some Journal or Conference Name},
  abbr      = {Some Journal or Conference Name},
  abstract  = {A short summary of the paper, shown when someone clicks "Abs."},
  arxiv     = {2401.12345},
  bibtex_show = {true}
}
```

A few important rules for this format:

- Every entry starts with `@` followed by a type (usually `@article` or `@inproceedings`), then `{`, then a short unique ID with no spaces (e.g. `pan2026example` — any consistent naming works, it's just an internal label), then a comma.
- Every field follows the pattern `name = {value},` — don't forget the curly braces and the comma at the end of each line except the last one before the closing `}`.
- The whole entry must end with its own closing `}` on its own line.
- **Getting the BibTeX for a paper**: on Google Scholar, click "Cite" under the paper, then "BibTeX" — copy everything it gives you and paste it in as a new block. You can add the extra fields below afterward.
- Useful optional fields, each controlling one button under the entry:
  - `abstract` — shown when a reader clicks "Abs."
  - `bibtex_show = {true}` — shows a "Bib" button with the raw citation.
  - `arxiv` — just the arXiv ID (e.g. `2401.12345`, not the full URL) — shows an "arXiv" button.
  - `html` — a full URL — shows an "HTML" button linking there.
  - `abbr` — shows a small badge with the venue name in the left margin.
- The page automatically groups and sorts papers by year — you don't need to keep the file in any particular order.

### Adding a paper

Paste its BibTeX as a new block anywhere in the file (with a blank line before and after), then add whichever optional fields above you'd like.

### Removing a paper

Delete its whole block, from its opening `@article{` (or similar) line down to its closing `}`.

This file is edited by hand only — nothing regenerates it automatically, so it will only ever show exactly what's written in it.

---

## What not to touch

Everything else in the repository — folders like `_layouts`, `_sass`, `_includes` (other than `_includes/content/`), and files like `_config.yml` or `pages/index.md` — controls the site's design, colors, and page structure rather than its words. These are more delicate: a small mistake there can visibly break the site's layout. Leave those to a developer.
