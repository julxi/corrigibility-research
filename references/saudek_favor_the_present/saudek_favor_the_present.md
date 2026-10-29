# Why Should Corrigible Agents Favor the Present?

**Ben Saudek** · 27 Aug 2026 · [LessWrong](https://www.lesswrong.com/posts/8Z4ajAi6CjBxZbGMK/why-should-corrigible-agents-favor-the-present)

> Markdown conversion of the post as saved from GreaterWrong (comments omitted). Formatting changes only.

A corrigible agent understands that it is flawed and seeks to empower its principal to correct those flaws. Many of the intuitive examples of corrigibility happen over a short period of time: the principal gives a command, and then the agent follows it. When there are contradictory commands given at different times, it seems like the agent should follow the most recent command, but it’s unclear exactly why corrigible agents favor the present over the past.

In this post, I will explore this [open question](https://www.lesswrong.com/posts/wZjGLYp5WQwF8Y8Kk/5-open-corrigibility-questions) from Max Harms’ CAST sequence, reproduced verbatim:

- Corrigibility clearly involves respecting commands given by the principal yesterday, or more generally, some arbitrary time in the past. But when the principal of today gives a contradictory command, we want the agent to respect the updated instruction. What gives the priority of the present over the past?

As a simple example, which I will return to throughout the post, consider the following case. On Monday, the principal tells the agent to buy apples every week. On Tuesday, the principal tells the agent to buy oranges instead of apples. A corrigible agent should respect the newer command, but why? Is it just a preference that we have—that is, a corrigible agent *could* respect Monday’s command, but it’s more desirable to have an agent that gives priority to the present? Or is giving priority to newer commands an intrinsic part of what it means to be corrigible?

I will argue that the answer is somewhere in between. Corrigibility doesn’t seem to uniquely privilege the present: a corrigible agent can respond with some delay. However, corrigibility requires that the principal retain the ability to correct the agent. It is incorrigible for an agent to latch onto a command from the past principal and ignore attempts at correction. The present principal’s authority might be best understood as a consequence of the ability to correct the agent rather than an independent feature of corrigibility.

# Can agents just be corrigible to the present principal?

My first instinct is that agents are just corrigible to the present principal, since this at least explains what’s going on in the fruit-buying example. However, an agent that’s solely corrigible to the present principal would do nothing! All commands take some time to communicate, so agents only ever hear commands from the past. An agent that only cared about commands given by the present principal wouldn’t respect any commands.

Even if a time slice is slightly broader than one instant, so that being corrigible to the “present principal” includes the time it takes for a command to be communicated, such an agent would still be useless. It wouldn’t follow the command even 30 seconds after it was given, since then it was given by the past principal.

It’s tempting to say that the agent can just *assume* the present principal still endorses their command because they haven’t repealed it or issued a contradictory command. This starts to feel like incorrigible behavior, though. A corrigible agent doesn’t try to guess what the principal wants and act accordingly, since estimating the principal’s will leads to the [problem of fully updated deference](https://www.lesswrong.com/w/problem-of-fully-updated-deference). Listening to commands isn’t the best way to learn what the principal truly wants, so the agent might instead deconstruct the principal’s brain to figure out precisely what they want. Solutions that rely on guessing whether the principal endorses a particular command, or more broadly, guessing what the principal wants, lead to incorrigible behavior.

# Differences between the past and present principal 

Each difference between the past and present principal is a possible way to answer the original question, since the answer must be grounded in *some* difference between the past and present principal. If they were literally indistinguishable, there would be no basis for prioritizing one over the other.

## Existence

The most straightforward difference is that the present principal exists and the past principal doesn’t, but there are two problems. First, it might not be true! It relies on a controversial view about the nature of time. [B-theorists](https://en.wikipedia.org/wiki/B-theory_of_time), for example, would disagree with the assertion that the past principal doesn’t exist. It would be strange if resolving the mundane fruit-buying case depended on disproving B-theory.

Second, it implies that past commands don’t have authority. If the past principal doesn’t exist and existence is required to have authority, then no past command could have authority. The agent can’t assume that the principal still endorses those commands for reasons explained above.

## Information

Usually, the present principal knows more than the past principal. They’ve observed everything that the past principal has, plus whatever happened in the meantime. Perhaps newer commands deserve priority because they’re more informed. For example, we might imagine that the command to buy oranges is because the principal was made aware of a sale that they didn’t know about when they asked for apples.

There are several issues. It’s not always true that the present principal is more informed. People forget information all the time. A student on summer break might be less informed than they were during the school year, but that doesn’t mean the agent should stop listening to the student over the summer.

This explanation also could favor the future principal over the present principal. For the same reason that the present principal is generally more informed than the past principal, the future principal will probably be more informed than the present principal. But it would be incorrigible if the agent refused a request from the present principal on the grounds that the future principal might want something else.

## Knowledge of past commands

The present principal can remember the past principal’s thoughts, but the past principal can only speculate about what the present principal will think. If the present principal knows why the past principal issued a particular command but realizes the circumstances have changed, then it can issue a new command. This is a more specific type of information that might get around the problems outlined in the previous section.

First, it is true that the present principal isn’t *always* more informed about the relevant past commands. However, the past principal can’t ever know about future commands, so the information asymmetry only goes in one direction. For example, the Tuesday principal knows that the Monday principal asked for apples and might know why, but the Monday principal cannot know with certainty that the Tuesday principal asked for oranges. So it could be that the present is authoritative because it’s the only time slice that can in principle know about the relevant past commands and why they were made.

This doesn’t completely answer the question, though. What happens if the Tuesday principal forgets the Monday principal’s reasoning? On Tuesday, a corrigible agent should still follow the Tuesday command, so there must be something else going on.

## Interaction

Another possible explanation is that only the present principal can interact with the agent. However, this isn’t entirely true—the past principal could leave notes for the agent. This doesn’t seem like a promising answer.

## Responsiveness

Although it’s true that the past principal can interact with the agent, there are some limitations. The content of notes that the past principal might leave is fixed, so it’s always possible that the agent has a question the past principal didn’t anticipate. Even if the past principal successfully predicts the questions that the agent will ask, there are some questions that can’t be answered in a note.[^1] However, the present principal can always correct the agent’s behavior.

I don’t think this completely answers the question. It can’t explain why the agent should follow past commands, but it does raise an interesting point. Corrigibility might give special attention to revisionary commands—commands that correct, revoke, or update earlier instructions. Then, responsiveness matters because revisions are temporally asymmetric in a way that prioritizes the present principal.

# Can empowerment help?

Empowerment might help us answer the question. A corrigible agent seeks to empower its principal.[^2] Returning to the fruit-buying example, if the Monday principal asks for apples and the Tuesday principal asks for oranges instead, then continuing to buy apples disempowers the principal—they can no longer correct the agent.

One could argue this smuggles in the premise that the agent should empower the Tuesday principal over the Monday principal. Someone who thought that the agent should favor the past over the present might argue that the agent should buy apples in order to empower the Monday principal. If there’s no conceptual basis for empowering the present principal over the past principal, then corrigibility might be a less natural concept than previously thought.

Is there anything that can be said here? First, it’s worth clarifying what exactly it means to empower the principal. There are a few senses of “principal” that could be relevant:

- P1: The principal as a temporally extended person

- P2: The principal at a relative temporal location (e.g. the principal from 24 hours ago)

- P3: The principal at a fixed temporal location (e.g. the principal at noon on January 1, 2026)

What would it mean to empower each of these? Very loosely, the agent empowers the principal by helping the principal get what it wants.[^3]

Empowering P1 means helping the principal, a person who persists through time, realize their values. This alone doesn’t answer the original question since temporally extended people can change their values over time. We still need a way to determine what counts as empowering the principal when different time slices of the principal disagree. We could aggregate the principal’s preferences across time, use the present principal’s values, etc. In other words, understanding the principal as a temporally extended person gives us a range of options for which values to choose from, but doesn’t tell us which specific values to choose.

Empowering P2 means helping whatever time slice of the principal that’s currently at the specified time (t^(\*)) realize its values. This could be the Monday-at-noon principal at t₁, the Tuesday-at-noon principal at t₂, and the Wednesday-at-noon principal at t₃. Unlike P3, the time slice the agent is corrigible to changes over time. At some point, the agent will empower every time slice of the principal. This is one possible arrangement, but does little to answer the question because it’s unclear which temporal location the agent *ought* to empower.

Empowering P3 is clearly incorrigible. An agent that was empowering a fixed temporal location wouldn’t be open to correction, couldn’t be shut down unless specified by the principal at t^(\*), and would resist value changes.

Corrigibility seems to entail that the agent empower P1, rather than P2 or P3.[^4] However, this is only a partial answer, since there are multiple ways that the agent could empower P1, and none of them jump out from the definition of empowerment.

# Principal identity

In previous sections, I’ve treated different time slices as competing sources of authority. In the fruit-buying example, a past-favoring agent favors the Monday principal and a standardly corrigible agent favors the Tuesday principal. However, I understand corrigibility as being about a *relationship* between the principal and agent rather than a formula for assigning weight to each time slice. If we say an agent is corrigible to Joe, we don’t mean it’s corrigible to Joe-at-1:37:04 PM, then Joe-at-1:37:05 PM, then..., we mean it’s corrigible to *Joe*!

This isn’t necessarily incompatible with the intuition that more recent commands always take precedence over earlier commands. It’s perfectly comprehensible for the agent to say “I know that’s what Joe-at-1:37-04 PM wants, but is that really what *Joe* wants?” In other words, this view can’t accommodate the agent *always* updating on more recent commands, even if it’s true that the agent normally does. I worry that this view might rely on the agent estimating the principal’s will, which leads to the problem of fully updated deference.

# Commands as exercises of continuing authority 

Another possible answer is that commands are exercises of continuing authority. Rather than calculating the authority of a command by looking at the decision policy and the time the command was given, a corrigible agent might instead understand commands as continuous reflections of the principal’s authority.

In order to illustrate the point, I’ll briefly shift focus to a related concept from the legal system: *lex posterior derogat priori* (LPDP), the principle that a later law repeals an earlier one if the two are inconsistent. This is a helpful analogy for thinking about corrigibility. One thing we can initially note is that the authority of a law doesn’t diminish over time.[^5] Murder won’t be any less illegal in 50 years just because the law making it illegal got older.

There are several justifications in the literature for LPDP. One comes from [Eugenio Bulygin](https://albayanres.com/books/1695726509.pdf):[^6]

> \[T\]he principle aims at ensuring respect for the intentions of the legislature and has similar pre-requisites.62 By prioritizing the more recent norm, the assumption is that the legislature is aware of the earlier law and intends to overrule it.63 Applying the more recent norm also ensures that the views of the current legislature (or framer of the constitution) prevails over those of previous legislatures.

In corrigibility terms, because later principals have more context, the agent figures that the principal is aware of the earlier command and wishes to revoke it. Earlier in the piece, I examined a similar justification—that the present principal knows their reasons for issuing past commands and can evaluate if those reasons still hold—but concluded that it was incomplete because the present principal could forget why they issued a command. However, this justification for LPDP is slightly different: it only relies on the legislature knowing *that* they passed the law, not *why* they passed it.

I’m unsure of this solution. One could also argue that the past principal is always aware of the possibility of a conflicting command, which should give them similar authority. For example, if the past principal tells the agent to do X, it’s because the agent isn’t doing X. So at one point in the past, the principal corrected the action “¬X” by telling the agent to do “X”. If in the future, the principal corrects the action “X” by telling it to do ¬X, why is the later correction privileged?

This objection has been raised by [Peter Suber](https://dash.harvard.edu/server/api/core/bitstreams/7312037d-b1de-6bd4-e053-0100007fdf3b/content):

> Second, statutes may amend or repeal other statutes, and the newer is more likely an amendment of the older than vice versa.\[Note 1\] Why this should be so is unclear. If the newer statute is taken to be the amending, not the amended, statute, then it may be by appeal to “legislative intent”, which collapses into the first reason \[that recent laws are the most recent voice of the people\], or by some appeal to the nature of statutes as a rule of change for statutes. Statutes unquestionably are rules of change for statutes, but this fact alone cannot explain why only newer statutes possess the power of implied repeal, or why it is so difficult for a statute to amend or repeal inconsistent future statutes through self-entrenchment.

It feels more natural to assume that newer commands replace older commands than to assume that older commands supersede newer ones, and to some extent this assumption is right. At some point in time, any given command must have authority over the commands that came before it. Otherwise, the agent is being incorrigible by resisting correction. However, it’s not clear that corrigibility specifies exactly how this must happen (e.g. it seems like past-favoring agents are permissible). Many of the existing justifications for LPDP, while helpful to consider, don’t quite explain what’s going on with corrigible agents.

# Different decision policies 

In this section, I’ll evaluate different types of agents to see if they are corrigible. As I mentioned in a previous post on corrigibility over time, corrigible agents need a way to aggregate commands given over time. There are many possible rules that an agent could use:

- **Standard Agent**: each command takes priority over the commands that came before.

- **Past-Favoring Agent**: the agent gives the highest priority to commands from some time t^(\*) in the past, but also considers past commands that were given after t^(\*).

- **Delayed Agent**: the agent behaves like a standard agent, but commands take time to kick-in.

- **Time-Neutral Agent**: the agent gives equal weight to every command, no matter when it was given.

- **Reverse Agent**: the opposite of a standard agent. Each command takes priority over the commands that come after.

## Past-Favoring Agents

Past-favoring agents are corrigible, with some minor exceptions. It doesn’t seem like there’s something that *uniquely* privileges the present. It’s conceivable that an agent could give the most weight to commands from a past time slice of the principal. However, if the agents favor a time too far in the past, the resulting relationship might be incorrigible. As an extreme case, consider an agent that prioritized commands from 100 billion years ago. It would be extremely difficult to work with this agent! Corrections would take billions of years to take effect. Because one of the central components of corrigibility is empowering the principal to correct the agent’s flaws, such an extreme past-favoring agent strikes me as incorrigible.

## Delayed Agents

Most delayed agents are corrigible, but agents with extreme delays are incorrigible. As a proof of concept, consider that no agent responds to commands immediately. Even standard agents have a small delay: the speed of sound is finite, and it takes the agent some time to process the command.

Perhaps the fact that a delayed agent *chooses* to ignore commands for some period of time makes it incorrigible (as opposed to standard agents, which have a built-in delay as a matter of physical necessity, not due to an active choice). But consider an agent with a one millisecond delay. This agent’s behavior is indistinguishable from a standard agent’s, so it seems wrong to call this agent incorrigible. It’s true that as the delay grows, the agent’s behavior will eventually differ from a standard agent’s. However, it feels possible for a delayed agent to maintain the right kind of relationship to the principal, even if the principal can’t immediately correct the agent. Like past-favoring agents, I suspect that a delayed agent with an extremely long delay is incorrigible.

## Time-Neutral Agents

Time-neutral agents are incorrigible. If all commands are timeless—that is, they always have the same weight—the agent will be extremely difficult to correct. We can think of a time-neutral agent as tallying votes for each action. The tally of votes can never decrease, so if the principal wants to correct the agent, they will have to vote for the other side by issuing commands. Depending on the current tally, the principal may have to command the same thing multiple times in order to change the agent’s behavior.

Let’s return to the fruit-buying example, but imagine that the principal is uncertain about the decision, so they tell the agent to ask them every day for the next year before buying anything. For the first 364 days, the principal told the agent to buy apples. However, on the 365th day, the price of apples skyrockets so the principal tells the agent to buy oranges instead. Now, there are 364 votes in favor of buying apples and only one vote for oranges. The principal would have to tell the agent to buy oranges 364 more times in order for the agent to actually listen.

This kind of agent again strikes me as incorrigible. It resists correction, and the problems only grow worse as more commands are issued.

## Reverse Agents

Reverse agents are clearly incorrigible. The first command they receive has authority over all commands. The second command they receive has authority over all commands, minus the first one. And so on. This leads to extremely uncorrectable behavior. Once a command is given, the principal can’t get the agent to change course later. It could try telling the agent to change its behavior but this new command would get less weight than the original command, so the agent wouldn’t listen. In the fruit-buying case, the agent would buy apples. Even though the Tuesday principal asked for oranges, that command matters less than the earlier command to buy apples so the agent would ignore it.

# Conclusion

I started by asking why corrigibility seems to privilege the present principal over the past principal. Tentatively, this doesn’t seem like a strict requirement for corrigible agents. The past principal clearly has *some* authority, even though the agent should be open to correction. An agent can give priority to some past time slice, or take some time to respond to new commands, while remaining corrigible.

However, corrigibility does impose at least one relevant constraint: the principal must retain the ability to correct the agent. This entails that when two commands contradict, the later one must eventually be given priority. It also rules out agents with sufficiently long delays (e.g. billions of years) and agents that give unwavering authority to the past (e.g. by always giving newer commands less weight than older ones).

There are still several confusions that I have:

- Which types of past-favoring and delayed agents are corrigible? Where is the cutoff between “corrigible but takes time to correct” and “incorrigible because it takes too long to correct?”

- Can a command bind the agent to ignore future commands? Is it corrigible behavior to follow such a command, or does the agent need to modify itself to be incorrigible?

- Should the agent care at all about the future principal? Do expected future commands carry any weight?

- Does any part of this argument implicitly rely on a controversial view about the nature of time?

*Thanks to Max Harms for reviewing a draft of this piece, and to Ian Kahn for helpful thoughts on principal identity.*

[^1]: For example, “did you write this note?” Even if the note says “I, the past principal, wrote these instructions,” this doesn’t answer the question, because the agent can ask if the past principal wrote that clarification.

[^2]: At least in a limited sense. A corrigible agent might not empower the principal in the broadest possible sense, but certainly empowers the principal by at least proactively bringing up problems, allowing the principal to make corrections, etc.

[^3]: I will assume a narrow sense of empowerment here: empowerment over a subset of the principal’s values (such as being able to correct and shut down the agent).

[^4]: This *isn’t* because P2 and P3 favor the past. It’s because an agent can’t be solely corrigible to any particular time slice of the principal, including the present principal.

[^5]: Of course, this isn’t always true. There are some archaic laws that no longer have authority, but I don’t think this edge case is relevant.

[^6]: I wasn’t able to track down the original source, but the quote I included is on page 136 of the attached PDF.
