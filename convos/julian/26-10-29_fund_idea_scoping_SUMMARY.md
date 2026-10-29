# SUMMARY: Scoping a project idea for the Corrigibility Research Fund

**Last updated:** 26-10-29 (sources saved locally; Idea 1 premise checked in the paper; four candidate ideas ranked; waiting on the humans' answers to the open questions)

Julian wants to find out whether there is a fundable project idea for the Corrigibility Research Fund (corrigibilityresearch.org; manager Max Harms; run through Lightcone Infrastructure). Julian gave three references: Hudson's "Corrigibility Transformation" (arXiv 2510.15395), Byrnes's "Empowerment, corrigibility, etc. are simple abstractions (of a messed-up ontology)", and Saudek's "Why Should Corrigible Agents Favor the Present?". The LOG has a full digest with quotes. All sources were read through web-fetch subagents, not checked line by line by the main agent. Local copies of the three references (full text, including all post comments) are in the gitignored `references/` folder. The README explains how to recreate it.

## Key facts

- [verified: fund homepage and two LW posts, 26-10-29, via subagent] **Round 2 deadline: October 31, 2026.** Apply on Lightcone Commons, mention corrigibility, and disclose AI use. Typical grants are $5k–$35k, and low asks are favoured. Mid-December prizes reward corrigibility work done in 2026 and need no application.
- Max wants: philosophy write-ups, formalism that pressure-tests intuitions, the ethics of corrigibility and model welfare, and the risks of corrigibility. Empirical work only if it studies "something more interesting than 'are they corrigible.'"
- Red flags: LLM-written applications; superficial CAST citations without "receipts"; testing current LLMs for incorrigibility ("easy and not very interesting"); numbers over insight; proposals that sit in a crowded cluster. Who the applicant is weighs heavily: the ideal is prior demonstrated interest in corrigibility.
- Overlap: Hudson and Saudek (authors of two of the three references) are both Round 1 grantees. Saudek is already writing on the self-binding-command question. LLM evals and benchmarks are a crowded cluster (one funded, several honorable mentions).

## Candidate ideas (ranked) — all [concluded], none ratified

1. **Self-binding commands and revocability.** What should a corrigible agent do with "ignore my future corrections"?
   - [verified: local PDF text, 26-10-29, partial read] Hudson's transformation rewards accepting an update to *any* goal equally, including an incorrigible one. The paper leaves "which updates they are allowed to make" to governance.
   - The bare observation is not a contribution. The research content is the space of weaker policies (expiring commitments, commitments that can only be undone with a delay or confirmations, the principal treated as a temporally extended person), plus whether Hudson's no-performance-cost result survives restricting updates to corrigibility-preserving goals.
   - Real-world analogue: psychiatric advance directives (Ulysses clauses).
   - Overlap: Saudek (writing on self-binding); Hudson (reversibility); Carroll et al. 2024 (arXiv 2405.17713, which preference timestamp to use), not yet read.
   - Strongest fit, but needs formal skills.
2. **Ethics of corrigibility / effects of corrigibility training on the model.** Explicitly wanted by Max, unclaimed in Round 1, but unrelated to the given references.
3. **Counsel vs manipulation as a test of Hudson's transformation.** Possibly not a real gap. The myopic construction may already remove the obvious incentive.
4. **Empirical study of temporal command conflicts in LLMs.** Weakest: it falls in the cluster Max calls uninteresting.

[concluded] An agent should not draft the application text. Max treats AI-written applications as a red flag, and one of the patterns he lists is "agent trying to shoehorn their setup into something corrigibility related".

## Open questions for Julian and Ankush

1. Backgrounds and prior engagement with corrigibility.
2. Round 2, the December prizes, or a later round (none is announced yet).
3. Can either of you do formal proofs?
4. Are you willing to contact Saudek and/or Hudson?

## See also

- `convos/julian/26-10-29_project_setup_SUMMARY.md` — the repository's setup decisions (team, git workflow)
