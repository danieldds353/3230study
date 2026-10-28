# ITEC 3230 — Recall Studio: all six supplied lectures

This GitHub-ready package adds the missing **Lecture 05: Prototyping & walkthroughs** to the latest version, retaining Lecture 06, Weeks 1–4, matching readings and optional sections.

## New Lecture 05 material

- **40 original MCQs** with explanations and exact PDF page references.
- **24 short-answer questions**, each with two concise model lines and key-point checklists.
- Topics: conceptual models/metaphors, interaction types/styles, fidelity and coverage, prototype lifecycles, storyboards/PICTIVE, interface builders/Wizard of Oz, principles/visual design, participatory design, heuristic evaluation, cognitive walkthroughs, GOMS, KLM and Fitts’ Law.
- Downloadable `lecture-05-study-guide.pdf`; the Lecture 06 PDF is retained.
- Lecture 05 appears before Lecture 06 in the lecture cards and selectors. The existing 338 question objects and their order are unchanged; 64 new questions are appended with IDs beginning `l5-`.
- Practice and timed rounds can select Lecture 05 alone or all supplied lectures. No additional textbook assignment or later assessment format is inferred.

## Bank totals

| Scope | MCQ | Short answer | Total |
| --- | ---: | ---: | ---: |
| Weeks 1–4 + existing matching readings | 164 | 80 | 244 |
| Lecture 05 | 40 | 24 | 64 |
| Lecture 06 | 40 | 24 | 64 |
| All supplied lectures | **244** | **128** | **372** |
| Optional project / other-professor / excluded background | 20 | 10 | 30 |
| Complete bank | **264** | **138** | **402** |

## Update GitHub Pages

1. Extract the ZIP.
2. Upload its contents to the same repository folder as the previous version, replacing files with matching names.
3. Keep `index.html`, `styles.css`, `app.js`, `questions.js`, `lecture-05-study-guide.pdf` and `lecture-06-study-guide.pdf` together.
4. Commit to your existing publishing branch/folder and refresh the published page. No install or build is required.

The package does not publish to a GitHub account automatically. Progress uses the same browser-storage key and stable existing question IDs. Replacing files at the same website origin preserves compatible progress; Export/Import provides a backup. Moving to a different website address or browser does not automatically transfer local progress.

## Editing and local use

Run `python3 tools/build_bank.py` to regenerate `questions.js`. Edit Lecture 05 content in `tools/prototyping_bank.py`, Lecture 06 in `tools/evaluation_bank.py`, original questions in `tools/build_bank.py` and reading-linked questions in `tools/reading_bank.py`. Python’s standard library is sufficient.

For local use, serve the folder with `python3 -m http.server 8000`. `LECTURE_05_QUESTIONS.md` and `LECTURE_06_QUESTIONS.md` provide source-order copies of the new sets. See `STUDY_GUIDE.md` for scope and revision advice.

The 8–10 question, 60-minute format remains a study preset from earlier exam preparation. It is not a confirmed format for later assessments. Answers are self-marked; brevity is not a substitute for completeness. The source labels now correctly distinguish primary Lecture 05 coverage of analytical/predictive models from the optional other-professor photos.
