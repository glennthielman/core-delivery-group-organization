# Scale-up talk — Taylorism and Druckerism

## Goal of this talk

Give working software developers the vocabulary and the diagnostic tools to recognise which of two management systems their team is actually running — and then hand them a concrete structure for the case where a Druckerian group has to work alongside a delivery group that operates on Taylorist lines, as happens in offshore and nearshore arrangements.

Three things the audience should leave with:

1. **Recognition.** Agile adopted Drucker's vocabulary; most organisations kept Taylor's structure. Story points are time study, the backlog is a queue of instruction cards, and five "authorities" with no outcome accountability is Taylor's functional foremanship rebuilt by accident. Developers should be able to name what is happening to them.
2. **A diagnostic that resists faking.** Four questions: who defines the task, where the method lives, which direction measurement flows, and what happens when someone says the work should not be done. Any organisation can adopt the Drucker vocabulary in a quarter; none of these survives a quarter of pretending.
3. **A structure, in depth.** Not "do agile properly". A specific operating model: definition completeness as the interface, work classification with a no-exceptions routing rule, acceptance expressed as pre-written failing tests, architectural rules as executable fitness functions rather than prose, protected capacity for landscape evolution, and a bilateral working agreement whose decisive element is the explicit *not accountable for* list.

The underlying move the talk argues for: **stop trying to make a delivery group exceed the envelope, and make the envelope equal the correct outcome.** If the minimum is sufficient, minimum-effort behaviour stops being a problem.

Context: 50-minute conference-style talk (45 speaking + 5 Q&A) for a developer audience. Setting is a **large enterprise with a long history** — do not name an industry; "big enterprise" is the agreed public framing. Code examples are Java/Spring.

## The sharpened thesis — use this framing

Large enterprises did not choose Taylorism; they grew into it. They now describe themselves in Drucker's vocabulary, genuinely believe it, and continue to ask for innovation that the structure has no path to produce.

And what they run is not Taylorism properly. Taylor's system rested on a claim about knowledge: how long a task takes is a measurable fact, discoverable by investigation. Enterprises kept the **control** half and dropped the **knowledge** half:

- **Input is measured precisely** — headcount, day rates, hours booked, utilisation, budget consumed. It arrives on invoices, so finance needs it.
- **Output is not measured at all.** Nobody establishes what the money bought.
- **What looks like output measurement is self-referential.** Velocity is the team's estimate of its own work compared against itself; the line can rise while nothing outside changes.

So the organisation pays all of Taylorism's costs and collects none of its benefit. **Taylor is a critic of these organisations, not their patron** — his 1900 diagnosis applies unchanged. This is the talk's best turn; it rescues the Taylor history section from being a villain origin story.

The drift is gradient, not malice: input cost is trivially countable and output is genuinely hard, so measurement descends to the easy half. Second-order effect: with no output measure there is no early signal, so problems stay invisible until they are catastrophic — and a manager raising a concern with no metric behind it is simply the person bringing bad news, so silence is rational until the problem is undeniable.

## Register — important

**Structural, never cultural.** A cultural explanation for offshore behaviour was discussed during research and deliberately excluded. Do not reintroduce it. It is unfalsifiable, it forecloses design, and it is a liability on stage.

**Both profiles get strengths and costs.** This is a hard requirement, not a stylistic preference. If the Taylorist profile reads as a disease and the Druckerian one as a brochure, the talk produces finger-pointing between the two populations in the room — which is the exact dynamic it is trying to dissolve. The Taylorist profile's decisive strength, stated plainly: **it does not depend on exceptional people**, which is why organisations at scale converge on it.

**Disposition is preference, not type.** People genuinely differ in which profile they thrive in. Bounded problems with clear paths suit some people and are where they do their best work. Frame this as working preference and strength, never as capability or grade of engineer. The supporting evidence is the speaker's own observation: the person who never volunteers an opinion in an open forum gives a precise, considered answer when asked directly — the thought was there, the forum was wrong. Separate the structural half (forum, incentive — changeable) from the preference half (design around it, do not correct it).

**Neutral voice.** No first person, no "I watched this happen", despite the material being drawn from direct experience.

The talk is also explicitly not anti-agile, not a methodology pitch, and not a position for or against offshoring.

## Premises from the speaker's experience

Provenance: roughly twelve years of development work across several large enterprises. These are premises from direct experience, not findings to re-argue.

- The delivery group delivers what is explicitly defined, and nothing that is not. Work routed to them with room for investigation produces no usable result.
- This will not change within the planning horizon; opportunities to grow into broader responsibility were offered over several years and not taken up.
- **Opinions appear only on direct solicitation.** Ask the person what they think and you get a considered answer; do not ask and you get silence, including in meetings convened to collect opinions.
- **It is disengagement, not disenfranchisement.** Developers there have real say over craftsmanship, and the division of labour with design or analysis is often perfectly reasonable. What is absent is any wish to participate beyond the ticket — "I am here, I am doing my hours."
- **The time difference is one hour, not a time zone.** Questions can be asked and answered the same morning, and are not asked; the stated reason is not wanting to bother anyone. The barrier is social, not temporal. This rules out the easy fixes — more overlap hours and better tooling do not address it — and is the strongest argument for a structure that does not depend on anyone asking.
- **Failure produces attribution, not investigation.** Nobody sits down to establish why something failed, and nobody says they were wrong. Structural, not moral: with no shared record of what was supposed to happen, there is nothing to compare against except each other.
- **Documentation is extensive and unusable** — a maze accumulated over years. Finding the right page is harder than asking, and asking is also not done. This is the strongest practical argument for putting rules in the pipeline instead.
- **Remaining story points carry over sprint after sprint.** The product owner and scrum master record it as normal practice and never ask the team what it means. The data is not hidden; it is never looked at.
- The Druckerian team is real and the speaker leads one. Its distinctive feature: people operate well beyond their role titles — technically-titled people doing the communication, reporting or planning that nobody assigned them.

**The core team is a proposal, not the current state.** There is no core team today. It is the solution being designed in `Working structure - core and delivery group.md`.

## Files

- `Taylorism.md` — scientific management explained. Neutral and historical. Includes the contested historiography (Wrege & Perroni 1974, Wrege & Hodgetts 2000 on the pig iron story; Levitt & List 2011 on Hawthorne) and an objections section.
- `Druckerism.md` — Drucker explained. Neutral and historical. Includes an objections section (method, forecasting, Deming's point 11 on MBO) and a section on commonly misattributed quotes.
- `Two profiles in a software team.md` — a **practitioner account**, not a neutral field guide. Both profiles with strengths and costs, the degraded-Taylorism framing, split diagnostic/characterisation tables, and a closing section on what happens when both exist in one organisation.
- `Working structure - core and delivery group.md` — the operating model. Twelve sections, ten Mermaid diagrams. Current and consistent with everything above.
- `References.md` — framings considered during this work and the reason each was or was not adopted. The test applied is not whether a framing is true but whether it acts on the problems in the working structure. Currently: Forest and Desert (Andres-Beck / Beck), lean. Each entry carries what it describes, why it does not act on these problems, what is worth keeping, a conclusion and sources.
- `Cases.md` — enterprises outside tech running nearshore arrangements, Belgium-anchored where possible. The test applied is **what is verifiable**: each entry separates published fact from recruitment copy and vendor material. Headline finding: nobody publishes a method, and every organisation reports input (headcount, cities, targets) with no output measure at all — the degraded-Taylorism reading appearing in the public record. Currently: KBC, Euroclear, Ahold Delhaize, Barry Callebaut, Cegeka/Fluvius, ING, Colruyt as counter-example.
- `Talk deck - Taylorism and Druckerism.md` — 59 slides, Marp front matter, speaker notes as HTML comments, timing anchors in the header.

## Key design decisions

Three structural choices in `Working structure - core and delivery group.md` that are easy to undo by accident. They were each argued for specifically.

**Information is pulled, not pushed.** The interface does not rely on anyone raising a blocker. An open channel with a response SLA is the obvious design and it fails on the "nothing is volunteered" premise — the question is not asked even when the answer is thirty seconds away, because asking has a social cost and guessing does not. The first interface rule is therefore a **scheduled direct solicitation**: a named person asking specific people specific questions on a fixed cadence. Blocking is still encouraged, but the design does not depend on it and is expected to take months to establish. What is being optimised is not round-trip time — the loop is already short — but **silent assumptions**.

**The boundary is dispositional, not geographic.** The design sorts by work class, never by location or employer. Both populations typically sit onshore, sometimes in the same room. Do not let "Class A" become shorthand for "work we send over there" — at that point classification stops being about the work and the conflict the structure prevents returns by another door. Corollary: the structure is worth adopting even if the offshore arrangement ends.

**The core team does not exist and has to be formed.** Section 11 covers it: drawn from the team already working that way, four to six people, and three things needed on day one — authority to refuse a package, access to production signal, and a named owner for classification. The management conversation about what the core team will *not* be measured on happens before the team starts, not at its first review.

## Outstanding — deferred

**The deck is out of date and the speaker has deprioritised it.** Do not rewrite it unprompted. When it is picked up, four things need fixing:

- It still argues from a **24-hour round trip**. Wrong for this setting — see the one-hour premise above. The argument moves from latency to social reluctance, which makes the framework more necessary rather than less.
- It still carries **financial-institution / regulated-industry** framing. Should become an illustrative example rather than the speaker's context.
- It does not carry the **degraded-Taylorism turn**, which is a better pivot into the offshore section than what is there now.
- Part 3 presents Taylorism **without strengths**, which conflicts with the register requirement above.

## Conventions

- Obsidian markdown, no frontmatter on notes, `[[wikilinks]]` between them
- `Taylorism.md` and `Druckerism.md` stay neutral, historical and conclusion-free, and apply the **same evidentiary standard to both figures** — this symmetry was a deliberate correction and should not be undone. Lived experience belongs in the profiles document, not in these two.
- Mermaid for diagrams (renders in Obsidian; does **not** render in Marp without extra setup — export as images before `marp-cli`, or present from Obsidian Slides)
- Deck exports: `npx @marp-team/marp-cli@latest "<deck>.md" --pdf` or `--pptx`
