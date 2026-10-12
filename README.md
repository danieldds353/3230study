# ITEC 3230 — Recall Studio

A study website based on Professor Andriy Pavlovych’s Weeks 1–4 lecture materials.

## What is included

- 100 lecture multiple-choice questions and 48 lecture short-answer prompts.
- 20 optional multiple-choice questions and 10 optional short answers covering the project brief, another professor’s sample midterm, and background slides marked “Not on test.”
- Separate multiple-choice and short-answer tabs, with two-line model answers.
- Week filters, shuffled rounds, bookmarks, missed-question review and a searchable library.
- Timed 8- or 10-question practice sets; the 90-minute default is the student’s estimate, not a confirmed exam duration.
- Browser-local progress and JSON export/import.

## Put it on GitHub

1. Extract this ZIP.
2. Create or open your GitHub repository.
3. Upload the extracted files into the repository’s top level. `index.html`, `styles.css`, `app.js`, and `questions.js` must be beside one another. Upload the contents, rather than the ZIP itself or an extra enclosing folder.
4. Commit the files to your publishing branch (usually `main`).
5. Open **Settings → Pages**.
6. Set **Source** to **Deploy from a branch**.
7. Select your publishing branch and **/(root)**, then click **Save**.
8. Open the website link GitHub displays after deployment finishes.

GitHub Pages is available for public repositories on GitHub Free; availability for private repositories depends on your plan.

Official setup guide: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Editing and running

No installation or build is required to deploy. This package uses relative asset paths, so it also works as a GitHub Pages project site.

To preview locally, run `python3 -m http.server 8000` from this folder and open `http://localhost:8000`.

The question bank is in `questions.js`. To edit the maintained source, update `tools/build_bank.py`, then run `python3 tools/build_bank.py` to regenerate `questions.js`. Python’s standard library is sufficient.

Progress is saved on the current browser/device. It does not sync to GitHub or another device. Use Export/Import on the progress page to transfer it. Clearing browser data can remove it.

## Source scope

Questions are original practice applications of the four supplied lecture PDFs and project materials. References use PDF page numbers. The other professor’s midterm is explicitly supplemental. Default lecture rounds and timed practice omit slides marked “Not on test.” Week 5 and later lectures have not been provided.

This is a revision resource, not an official exam or an instructor grading tool. Equivalent accurate wording can count when self-marking short answers.
