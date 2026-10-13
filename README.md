# ITEC 3230 — Recall Studio: Slides + Matching Readings

An updated GitHub-ready study website. Professor Andriy Pavlovych’s supplied Weeks 1–4 slides define the scope. Selected matching sections from both supplied books deepen those topics.

## Question bank

- 164 slide-aligned MCQs and 80 slide-aligned short-answer prompts.
- This includes the original 100 MCQs and 48 short answers plus 64 MCQs and 32 short answers connected to readings.
- 20 optional MCQs and 10 optional short answers remain in separate project, other-professor and “Not on test” sections.
- Total: **184 MCQs + 90 short answers = 274 questions**.

Every reading-linked question cites a book section/chapter and relevant slide pages. These questions are original applications, not copied textbook exercises. Complete book files and extracted book text are not in this ZIP.

## What changed

- Default timed practice is **60 minutes**, reflecting the latest expectation of **8–10 exam questions**.
- Choose 8 or 10 questions and mixed, short-answer-only, or MCQ-only practice. The mixed ratio is a practice choice, not a confirmed exam split.
- Material filters: slides + matching readings, original slide questions, or reading-linked questions.
- An application-question filter supports scenario reasoning instead of recognition alone.
- New reading map and expandable key-point checklists for reading-linked short answers.
- Every short-answer model stays at two concise lines, with at most 40 words.
- Original question IDs remain stable, preserving existing progress when replacing files on the same website/browser. New practice defaults migrate to one hour. An already running older session retains its original deadline.

## Upload and publish on GitHub Pages

1. Extract this ZIP.
2. Upload its contents into your repository’s top level, replacing the previous site files. Keep `index.html`, `styles.css`, `app.js`, and `questions.js` together.
3. Commit to your publishing branch, usually `main`.
4. In **Settings → Pages**, choose **Deploy from a branch**, select your branch and **/(root)**, and Save.
5. Open the Pages link after deployment completes. If the old version remains visible, refresh the page to load the updated assets.

No installation or build is needed for deployment. Relative asset paths support a GitHub Pages project site.

Official setup guide: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Reading alignment

See **Reading map** in the website and `STUDY_GUIDE.md` in this package. Book sections were selected to match slide topics; this is not a claim that entire chapters have been assigned or will appear on the exam. Week 5 and later slides have not been supplied.

Books used:

- Rogers, Sharp & Preece, *Interaction Design: Beyond Human–Computer Interaction*, 6th edition (2023).
- Norman, *The Design of Everyday Things*, revised and expanded edition (2013).

Norman’s more precise affordance/signifier distinction and error analysis are clearly connected to the slides’ perceived-affordance, human-error and action-cycle material.

## Editing and local use

Serve this folder with `python3 -m http.server 8000`, then open `http://localhost:8000`.

Edit the original questions in `tools/build_bank.py` and the reading-linked additions in `tools/reading_bank.py`. Run `python3 tools/build_bank.py` to regenerate `questions.js`. Only Python’s standard library is needed.

Progress stays in the browser on the current device. Use Export/Import on the progress page to transfer it. Changing the website origin or clearing browser data can remove access to existing local progress.

This is a practice resource. Short answers are self-marked, and equivalent accurate wording can count. The models and checklists do not promise an instructor’s mark or an extra grade for brevity.
