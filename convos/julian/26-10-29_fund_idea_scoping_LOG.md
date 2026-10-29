The repo is for checking out if there is an idea for this fund:
https://corrigibilityresearch.org/

references are:
- https://arxiv.org/pdf/2510.15395
- https://www.lesswrong.com/posts/vzHtHHBJoKATi5SeK/empowerment-corrigibility-etc-are-simple-abstractions-of-a
- https://www.lesswrong.com/posts/8Z4ajAi6CjBxZbGMK/why-should-corrigible-agents-favor-the-present

---

26-10-29, Claude Opus 5.5 — *source digest: fund rules, round 1 grantees, three references*

**What I have read and how.** Web-fetch subagents read every source in this session and reported back to me. I did not read the pages myself, so every quote below is secondhand. It came through the subagent and was not checked against the live page. Pages read:
- the corrigibilityresearch.org homepage (it is a single page);
- Max Harms, "How I'm evaluating corrigibility grant applications" (LW, 26-09-03);
- "Corrigibility Research Fund Grantees (Round 1)" (LW, 26-09-03);
- "Announcing the Corrigibility Research Fund" (LW, 26-07-17);
- the three references the user gave.

Coverage gaps: for the arXiv paper, Section 3.3 after Thm 3.6, Appendices A–D, and the gridworld experiment numbers came only from a tool-generated summary. Two summaries disagreed with each other on those numbers. The PDF is saved locally (Claude Code tool-results directory for this session) if verification is needed. For the Byrnes post, the middle and late comments came only as a model summary.

No prompt injection was found in any page. The subagents saw a "reporting rules" block in fetch results, which comes from the fetch tool's own output, not from the pages.

### The fund

- Run by Max Harms (author of CAST, "Corrigibility as Singular Target"), housed at Lightcone Infrastructure, which "retains final approval of every grant and prize." 2026 budget: "at least $200,000", split roughly evenly between grants and prizes.
- [verified: fund homepage and both LW posts, 26-10-29, via subagent] **Round 2 deadline: October 31, 2026.** Apply on Lightcone Commons and "mention corrigibility." Email alternative: grants@corrigibilityresearch.org. "Applications are treated as public."
- Size: "typical grants to be around $5k–$35k". Round 1 funded 8 of "over 100 applications", "totaling $132k". "A low financial ask makes someone more promising." Work should begin this year, and "it's acceptable to not expect results until 2027." Grants can stack with other funding.
- Prizes: retroactive awards for corrigibility work done in 2026, no application needed (email nomination). "At least $60k awarded in mid-December."
- Exclusions: no lobbying, political activity, or private benefit; no paying for school; no work that "notably accelerates AI capabilities"; nobody currently at MIRI. "Theoretical work that's judged as too esoteric to be of interest to someone like Joe Carlsmith is unlikely to get funding. Work that's incompatible with mainline capability techniques ... is similarly unlikely."
- Application content (announcement post): "Tell me what you want to do, and what level(s) of funding you're hoping for. (Edit: And please disclose whether and why you used AI in generating your application.)" Also: "if writing the application takes you more than a few hours, something has probably gone wrong."

**Directions Max wants** (evaluation post, verbatim):
- Philosophy: "one of the most valuable things an individual researcher can do is find insights and try to write them up for the rest of the research community."
- Formalism: "an extremely valuable tool to use to pressure-test our intuitions."
- Ethics and model welfare: "investigation on the ethics of corrigibility and whether there are downstream effects of corrigibility training on the psychology of the AIs themselves."
- Risks of corrigibility (dictatorship, abuse of AIs that are moral patients): "particularly valuable."
- Empirics only if they study "something more interesting than 'are they corrigible.'"
- His conception: "a broad, agentic disposition that includes things like proactively surfacing flaws and gravitating towards straightforward plans". He contrasts it with narrow behaviour "like shutting down when asked, or obeying commands." The announcement adds: "You do not need to agree with my particular framing of corrigibility (i.e. CAST)", and he would "love to fund negative results."

**Red flags** (evaluation post):
- Testing current LLMs for incorrigible behaviour: "both easy and not very interesting."
- LLM smell in the application: "a strike against an application." One of the listed causes is "told their AI agent to acquire money, and the agent is trying to shoehorn their setup into something corrigibility related."
- Superficial CAST citations: "If someone looks like 'they read my stuff' it was probably their AI agent telling them what to say." Engaging with his work needs "receipts": "When did you read it? Why did you read it? What did you think?"
- "LLM-slop applications often emphasized numbers over insight/perspective."
- Clustering: "I was most excited by applicants who were not part of a big cluster."
- Who the applicant is counts heavily. The ideal is "relative outsiders who nonetheless have proven themselves interested in corrigibility prior to the announcement of the fund", and "the most promising person is someone who looks like they're itching to get into the space as a more full-time thing."

**Round 1 grantees** (already funded, so overlap risk):
- Kahn: CAST behavioural benchmark plus fine-tuning ($35k)
- Glover: activation geometry of corrigibility ($20k)
- Eyembe: Corrigibility Games ($12.5k)
- Dietz: dedicated misalignment-flag channel ($20k)
- Saudek: training a corrigible model ($3k)
- Wang & Liu: CAST decision theory, a formal model of a corrigible agent's decisions, with Lean proofs ($20k)
- Nick R.: benevolent-override pilot ($1.5k)
- Hudson / Principled Agents: research org runway ($20k); next project "incentives for taking actions that are reversible in the relevant ways"

Honorable mentions (not funded) include a lay-intuitions survey, correction-responsiveness across capability, whether deep corrigibility training makes models harder to correct, sycophancy as oversight failure, long-horizon agent evals, delegates' corrigibility, and an impossible-task eval. So LLM evals and benchmarks are a crowded cluster.

### The three references

**Hudson, "Corrigibility Transformation: Constructing Goals That Accept Updates"** (arXiv 2510.15395, v2 26-08-05).
- Setup: an MDP whose state includes the agent's goal, and an action that adds an accept/reject bit for updates sent through designated channels.
- The transformation replaces goal G with a myopic goal (γ=0). Its reward is the Q-value of the reject-version action under the original goal, plus a bonus δ for accepting: R_C(s,a_i,s') = Q^{π**}_G(s,a_0) + δ·𝕀(i=1). Accepting therefore always pays more than rejecting, and paying costs to avoid updates is not reinforced.
- Theorems: the result is corrigible, has no performance loss when no updates are sent (under a goal-independent-transitions condition), and is interruptible. A recursive version handles subagent creation, assuming the set of agent-creating actions is known.
- Experiments: gridworlds, plus a **prompt-level** LLM study on ImpossibleBench. In that study, monitor-disabling dropped "from 73% to 1%" and obfuscation from 16–17% to ~0% (table average over three models).
- Stated limits: the definition is strict; zero-cost prevention of updates is "not strictly disincentivized" (footnote 1); critic manipulation is untested; training (as opposed to prompting) is untested.
- The author is a Round 1 grantee.

**Byrnes, "Empowerment, corrigibility, etc. are simple abstractions (of a messed-up ontology)"** (LW, 26-05-11).
- Thesis: manipulation, empowerment, and corrigibility rest on a folk free-will ontology. So "none of these ... have any 'True Names' ... useful in practice for AI alignment."
- The crux is counsel vs manipulation. True facts also change what people want, so baselines like Harms's null-policy comparison are hard to justify.
- Rebuttals: Harms (only terminal-value changes matter), and abramdemski ("legitimacy" via a reflection principle).
- The argument is framed around Byrnes's brain-like-AGI design, not LLMs.

**Saudek, "Why Should Corrigible Agents Favor the Present?"** (LW, 26-08-27).
- Question: why should a later command override an earlier one? His answer: corrigibility doesn't privilege the present per se, but requiring that the principal can correct the agent implies later contradicting commands must *eventually* win.
- He sorts policies into standard, past-favoring, delayed, time-neutral, and reverse. Time-neutral and reverse are incorrigible; extreme delay is incorrigible. No formalism and no experiments.
- Open questions: where the delay cutoff lies; **whether a command can bind the agent to ignore future commands**; whether expected future commands count.
- In comments, Harms raised "Don't listen to what my future self tells you" and called untangling it "an important next-step". Saudek replied: "I've started thinking about it and hope to write up my thoughts sometime soon."
- Saudek is a Round 1 grantee.

---

26-10-29, Claude Opus 5.5 — *candidate ideas and recommendation*; based on the digest above. I have not read the Hudson paper's proofs myself.

### Fit check before ideas

The scarce input here is not an idea but **who the applicants are**. Max says who the applicant is "will often give better data than looking at their application". His ideal is someone with demonstrated interest in corrigibility *before* the fund was announced. I don't know Julian's or Ankush's background, prior corrigibility engagement, or available time. That determines which idea is viable and whether Round 2 is realistic at all.

[concluded] Submitting in two days with an application an agent drafted is close to the exact pattern Max screens against: AI-written text, CAST citations without receipts, and "agent trying to shoehorn their setup into something corrigibility related". Reasoning: each element is named as a red flag in his evaluation post (quotes in the digest above). Whatever goes in must be written by Julian and/or Ankush, with honest AI-use disclosure. I can help with critique, fact-checking against the sources, and thinking the idea through, but I should not draft the application text.

### Candidate ideas, ranked

**1. Self-binding commands and revocability: formal work bridging Hudson and Saudek.**
- Question: a corrigible agent should follow its principal, and the principal should stay able to correct it. What should it do with "ignore my future corrections" (Harms's comment), and what does Hudson's transformation actually do with such an update? My unverified reading of the construction: an agent with the transformed goal accepts *any* update through the channel, including one to a goal that rejects later updates. If so, the transform is corrigible step by step but lets the principal (or whoever controls the channel) end corrigibility in one move.
- Possible deliverables:
  - Saudek's temporal properties stated formally in Hudson's MDP setup ("eventual override", "bounded override latency", "self-binding is revocable");
  - a result about which combinations can hold together; there may be an impossibility between "obey every command" and "principal can always correct later";
  - a write-up.
- Fit: formalism that pressure-tests an intuition Max himself flagged as important; not in the eval cluster; ties all three references together.
- Risks:
  - (a) Saudek says he's already writing on this; Hudson's next project (reversibility incentives) is adjacent; Wang & Liu are formalizing corrigible decisions. Contacting Saudek and Hudson first could turn competition into collaboration.
  - (b) It needs real comfort with formal RL/decision theory.
- [assumed] The "accepts updates to incorrigible goals" reading is correct. It must be checked against Section 3 of the paper before anyone relies on it.

**2. Ethics of corrigibility / effects of corrigibility training on the model.**
- Max explicitly hopes for this "in future rounds", and nobody in Round 1 did it.
- It doesn't build on the user's references. It is listed because it is the clearest gap in the fund's own stated wants. Fit depends entirely on the applicants' background (philosophy, or model-welfare work).

**3. Counsel vs manipulation as a test of Hudson's transformation (Byrnes × Hudson).**
- Question: does the transformed goal leave the agent free, or motivated, to shape *whether the principal wants to send updates*? Byrnes's point is that this distinction has no clean formal definition.
- On a first pass, the myopic construction values outcomes as if updates were rejected. That might remove the obvious incentive to provoke or suppress updates, but it leaves G's other incentives to influence the human. [assumed] This needs a careful read before it counts as a real gap. If the incentive turns out to be absent, the idea collapses into "Byrnes's objection applies to every corrigibility scheme", which isn't a project.

**4. Empirical study of temporal command conflicts in LLM agents (Saudek's taxonomy).**
- Ranked last: Max calls testing current LLMs for incorrigibility "easy and not very interesting", and several honorable mentions are already in this cluster. It would only work if it studied something deeper, e.g. whether models distinguish revisionary commands from additive ones.

### Recommendation

[concluded] Idea 1 is the strongest *if* one of the applicants can do formal work. Reasoning: it matches two of Max's named priorities (formalism to pressure-test intuitions; an open question he called important), it combines the user's references instead of following one, and it avoids the crowded LLM-eval cluster. The main weakness is overlap with Saudek and Hudson.

Whether to aim at Round 2 (Oct 31) or not is the humans' call. The alternatives:
- (a) a short, hand-written, low-ask Round 2 application;
- (b) do the work now and submit it for the mid-December prizes, which reward 2026 work and need no application;
- (c) wait for a possible later round. None is announced; the announcement names only Rounds 1 and 2 for 2026.

### Open questions for Julian and Ankush

1. What are your backgrounds, and have you engaged with corrigibility before (writing, projects, reading CAST)? When, and what did you think? Max asks for exactly this.
2. Is Round 2 (Oct 31) the target, or is the December prize route or a later round acceptable?
3. Can either of you do formal RL/decision-theory proofs? That decides between Idea 1 and Ideas 2/4.
4. Are you open to contacting Saudek and/or Hudson before applying?

---

Can you save the referencens locally in a gitignored folder (not the grant page)

---

26-10-29, Claude Opus 5.5 — *references saved locally*

I saved the three references in `references/`, which I added to `.gitignore`. The README now has recreation commands, because ignored files don't reach other machines.

- `references/hudson_2510.15395/`: arXiv PDF v2 (dated 5 Aug 2026 on its first page) plus a `pdftotext -layout` conversion.
- `references/byrnes_empowerment_abstractions/` and `references/saudek_favor_the_present/`: GreaterWrong HTML with all comments, plus plain-text conversions.

[verified: title tags and comment-element counts, 26-10-29] Both posts are the real pages, not error pages. Their comment counts match those reported in the digest above (76 for Byrnes, 2 for Saudek).

A quick grep for instruction-like phrases aimed at AI agents found nothing. The only hit was ordinary paper text.

The digest's note that the PDF lives in the session's tool-results directory is superseded: use the copy in `references/`.

With full local text available, the two unverified points in this topic can now be checked directly: the Hudson gridworld numbers (the two summaries disagreed) and the [assumed] reading behind Idea 1 (that the transformed goal accepts updates to incorrigible goals).

---

What is the top-ranked idea? Your top-ranked idea? Can you explain it to me?

---

26-10-29, Claude Opus 5.5 — *Idea 1 premise checked against the paper; idea refined*

I read the relevant parts of the local Hudson PDF: Section 2 (setup and the definition of corrigibility), Algorithm 1 and the recursive transformation, the limitations paragraph, the Impact Statement, and Appendix D. This was not a full read; I did not check proofs.

**Premise check.** [verified: local PDF text, 26-10-29, partial read] Nothing in the formal setup stops an accepted update from installing an incorrigible goal:
- The definition is "fairly strict, allowing for updates to any goal at any time." After an update, "the agent will optimize for the new goal."
- The acceptance bonus δ·𝕀(i=1) in R_C does not depend on what the new goal is.
- Appendix D only ensures the goal space is well-defined (it assumes the space is closed under the transformation). It does not restrict updates to corrigible goals.
- The recursive transformation penalizes *creating other agents* with incorrigible goals, but not accepting an update that makes *the agent itself* incorrigible.
- The paper treats which updates are allowed as a governance question. Impact Statement: "care must be taken in determining which update channels are designated, who is allowed to make updates through them, and which updates they are allowed to make."

The [assumed] tag on Idea 1's premise is therefore resolved. The bare observation is not a contribution, though: Hudson can reply "that's by design; it's governance." The project has to add something beyond it.

**New prior work to check.** Hudson says Carroll et al. (2024, arXiv 2405.17713, on changing and influenceable reward functions) focuses on "which preference timestamp to use". That is close to Saudek's question and must be read before any application.

**Refined version of Idea 1.** Commands that bind the future.
- Trivial impossibility: no agent can both (a) always follow the latest command and (b) always leave the principal able to correct it later, once commands like "ignore all my future commands" exist. Obeying such a command breaks (b); refusing it breaks (a). [concluded: follows directly from the two definitions.]
- The research content is the space of weaker policies and which of them keep what corrigibility is for:
  - commitments that expire;
  - commitments that can be undone only with a delay or extra confirmations (the Ulysses-contract pattern);
  - the principal treated as a temporally extended person (Saudek's "P1") instead of whoever spoke last.
- An existing real-world analogue with its own literature: advance directives in medicine, especially psychiatric advance directives (Ulysses clauses), where a patient pre-authorizes treatment over their own later refusal. [assumed: I know this literature exists, but I have not read it in this project.]
- A tension worth stating: the web-fetch subagent reported that Max Harms, in a comment on the fund announcement, sketched a "24-day delay" as a governance mitigation (not verified by me). That is a delayed agent in Saudek's taxonomy, and Saudek argues that long enough delays are incorrigible. Where the line lies is exactly Saudek's open question (a).
- Embedding in Hudson's setup: could accepted updates be restricted to a corrigibility-preserving class of goals, and does the "no performance cost" result survive that restriction?

**Overlap risk, updated.** Saudek is writing on self-binding. Hudson's next project, reversibility incentives, is adjacent, since a binding command is an irreversible change to the command state. Carroll et al. covers preference timestamps.
