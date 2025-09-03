# Web Novel Starter (GitHub Pages + Jekyll)

This starter turns your `chapters/chapter_{n}.md` files into a clean reader site with a Table of Contents.
- Uses the first `# Heading` in each file as the page title
- Pretty URLs like `/chapters/chapter_1/`
- Hides a trailing `END OF THE CHAPTER` heading automatically on the live page

## Quick Start

1. **Create a repository** named `yourname.github.io` on GitHub (replace *yourname* with your GitHub username).
2. Download this folder, unzip, and **upload all files** to that repository (drag & drop works in the GitHub web UI).
3. Go to the repo **Settings → Pages** and ensure the source is the default branch.
4. Add your chapters to the `chapters/` folder (keep filenames like `chapter_1.md`, `chapter_2.md`, ...).
5. After you commit, your site will be at `https://yourname.github.io/`.

## Add Chapters

Each chapter file should start with a single `#` heading, e.g.

```md
# Chapter 1 — The Beginning
Your translated text here...

## END OF THE CHAPTER
```

The trailing `END OF THE CHAPTER` heading will be removed on the live page.

## Multiple Novels

- Option A (simple): make a separate repo per novel (e.g., `yourname.github.io-mynovel`) and publish as a **Project Page** under Settings → Pages. The URL will be `https://yourname.github.io/mynovel/`.
- Option B (single site): keep all novels here, create a folder per novel (`novel-a/`, `novel-b/`) each with its own `index.md` and `chapters/` folder, then link them from the root `index.md`.

## Submitting to NovelUpdates

- Use your site’s **index page** as the series URL.
- For each new release, submit the **per-chapter URL** (e.g., `https://yourname.github.io/chapters/chapter_23/`).

## Notes

- This site uses the GitHub Pages default theme (`jekyll-theme-minimal`). You can change it in `_config.yml`.
- If the order ever looks off, consider renaming files to use zero-padding (`chapter_001.md`) or keep `sort_natural` in `index.md`.
