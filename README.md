# Corrigibility Research

This repository is for finding out whether Julian and Ankush have a fundable research idea for the [Corrigibility Research Fund](https://corrigibilityresearch.org/). The fund is managed by Max Harms through Lightcone Infrastructure; it gives grants (typically $5k–$35k) and retroactive prizes for corrigibility research. Starting references: Hudson, "Corrigibility Transformation" ([arXiv 2510.15395](https://arxiv.org/abs/2510.15395)); Byrnes, ["Empowerment, corrigibility, etc. are simple abstractions (of a messed-up ontology)"](https://www.lesswrong.com/posts/vzHtHHBJoKATi5SeK/empowerment-corrigibility-etc-are-simple-abstractions-of-a); Saudek, ["Why Should Corrigible Agents Favor the Present?"](https://www.lesswrong.com/posts/8Z4ajAi6CjBxZbGMK/why-should-corrigible-agents-favor-the-present). A new reader should start with the fund-idea scoping topic below. Note that the fund manager treats AI-written applications as a red flag, so application text must be written by the humans.

This project uses the [Epistemic Memory](https://github.com/FlorianDietz/EpistemicMemory) conventions: all project memory lives in LOG/SUMMARY file pairs under `convos/`, governed by [CLAUDE.md](CLAUDE.md). Human guide: [docs/HOW_TO_USE.md](docs/HOW_TO_USE.md). Open ideas and deferred items: [FUTURE_WORK.md](FUTURE_WORK.md). Workflow problems and lessons: [FEEDBACK.md](FEEDBACK.md).

**Reference copies** live in `references/`, one subfolder per source, each with a markdown version tracked in git: `hudson_2510.15395/hudson_corrigibility_transformation_v2.md` (converted with pandoc from the arXiv LaTeX source; numbering matches the PDF) and, for the LessWrong posts, `byrnes_empowerment_abstractions/byrnes_empowerment_abstractions.md` and `saudek_favor_the_present/saudek_favor_the_present.md` (post only, comments omitted). Images are in each subfolder's `figures/`. The originals (PDF; the GreaterWrong HTML pages, which also contain all comments) are gitignored. To re-download them:

```
mkdir -p references/hudson_2510.15395 references/byrnes_empowerment_abstractions references/saudek_favor_the_present
curl -sSL -o references/hudson_2510.15395/hudson_corrigibility_transformation_v2.pdf https://arxiv.org/pdf/2510.15395v2
curl -sSL -o references/byrnes_empowerment_abstractions/post_with_comments.html https://www.greaterwrong.com/posts/vzHtHHBJoKATi5SeK/empowerment-corrigibility-etc-are-simple-abstractions-of-a
curl -sSL -o references/saudek_favor_the_present/post_with_comments.html https://www.greaterwrong.com/posts/8Z4ajAi6CjBxZbGMK/why-should-corrigible-agents-favor-the-present
```

## Team

- Julian Bitterlich — `convos/julian/`
- Ankush — `convos/ankush/`

**Identifying the current user:** run `git config user.name` and match it against this list. `Julian Bitterlich` → julian; any name containing `Ankush` → ankush. If the name matches neither or both, ask the user before proceeding.

## Current status and goals

Scoping a grant idea (topic `fund_idea_scoping`). Four candidate ideas are ranked; waiting on Julian and Ankush to answer the topic's open questions (backgrounds, whether to target Round 2).

## Maintenance

Recurring tasks:

| Task | Last run | Due when | Notes |
|------|----------|----------|-------|
| Sync (LOG/SUMMARY drift) | — | After many LOG changes, or ~monthly | `!sync`; procedure: `docs/procedures/sync.md` |
| LLM-ism checklist refresh | — | ~Monthly while you publish regularly; otherwise before any high-stakes submission | Update the checklist and Known-screening sections of `docs/procedures/outward_text.md` from full primary sources (see the file's refresh rule); bump its refresh date |

One-time deadlines (delete a row when done):

| Due | Item | Source (authoritative) |
|-----|------|------------------------|
| 26-10-31 | Corrigibility Research Fund Round 2 applications close (Lightcone Commons) | `convos/julian/26-10-29_fund_idea_scoping_LOG.md` |
| 26-12 (mid) | Fund awards at least $60k in prizes for 2026 work; nominate by email, no application | same |

## Conversation Index

All discussions live in `convos/{user}/`. **When starting a new topic, add a row here.** Read the SUMMARY first; open the LOG only if the SUMMARY is insufficient. Status cells describe current state only — rewrite them on update, don't append.

| Date | User | Topic | Status | SUMMARY | LOG |
|------|------|-------|--------|---------|-----|
| 26-10-29 | julian | Project setup (team, git workflow, privacy choice) | Done | [SUMMARY](convos/julian/26-10-29_project_setup_SUMMARY.md) | [LOG](convos/julian/26-10-29_project_setup_LOG.md) |
| 26-10-29 | julian | Scoping a Corrigibility Research Fund project idea | Sources digested, 4 ideas ranked; awaiting answers on backgrounds and Round 2 | [SUMMARY](convos/julian/26-10-29_fund_idea_scoping_SUMMARY.md) | [LOG](convos/julian/26-10-29_fund_idea_scoping_LOG.md) |
