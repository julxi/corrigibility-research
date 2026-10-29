# SUMMARY: Project setup

**Last updated:** 26-10-29 (all references converted to markdown and tracked; PDF/HTML originals ignored; post files renamed after their source)

Julian asked me to set up the Epistemic Memory template for this repository. I interviewed Julian and configured the repository accordingly. The verbatim interview answers are in the LOG.

## Decisions

- [decided] Team of two: Julian (git user.name `Julian Bitterlich`, folder `convos/julian/`) and Ankush (folder `convos/ankush/`).
- [decided] Agents identify the current user by matching `git config user.name` against the README team list, and ask when the match is ambiguous.
- [assumed] Ankush's git user.name contains "Ankush". The exact value is unknown.
- [concluded] Folder slugs `julian` and `ankush`. These are my choice, not yet confirmed by Julian.
- [decided] Default git workflow: agents never commit or push. The human reviews every change in the diff before committing it.
- [decided] Private records are not set up for now. They can be added later per CLAUDE.md §Privacy.
- The README project description is based on Julian's chat description of the project (see `convos/julian/26-10-29_fund_idea_scoping_LOG.md`).

## What changed

The demo user `convos/jamie/`, `CORE.md`, the CLAUDE.md template note, and the example entries in FUTURE_WORK.md and FEEDBACK.md were removed. README.md is now the working index, built from `docs/README_SKELETON.md`.

`references/` is tracked in git except the originals (`*.pdf`, `*.html`), at Julian's request. Each source has a markdown version: the Hudson paper converted from the arXiv LaTeX source (numbering matches the PDF), and each LessWrong post as a markdown file named after its folder, e.g. `references/byrnes_empowerment_abstractions/byrnes_empowerment_abstractions.md` (post only; comments omitted at Julian's request). The LessWrong posts' license was not checked, which matters only if the repo goes public.

## Open items

1. Confirm or change the slugs.
2. Give Ankush's exact git user.name.
3. Review the diff and commit.

## See also

- `convos/julian/26-10-29_fund_idea_scoping_SUMMARY.md` — the first research topic
