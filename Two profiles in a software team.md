## How to read this

The two notes before this one describe [[Taylorism]] and [[Druckerism]] as bodies of thought. This one describes what each looks like when it is already running inside a software team — not as a philosophy anybody signed up to, but as a set of things a visitor could observe in a week without being told anything.

That is the perspective throughout: an outsider sitting in the room for five days, allowed to watch the board, the meetings, the chat and the way people talk about each other, but not allowed to ask what the team believes about management. Nobody in either team describes themselves in these terms. Neither profile is a job title or a methodology; both can wear the same process framework, the same ceremonies and the same tooling.

The headings are deliberately mirrored so the two can be read in parallel.

---

# Profile one: the Taylorist team

## The shape of the team

The first thing visible is that the team is a **stage in a pipeline**, not a unit that owns something. Work enters from somewhere upstream and leaves to somewhere downstream. Ask who the customer is and the answer names an internal party: the business analyst, the product owner, the client's project manager, the integration team. Ask what the team is responsible for and the answer is a *phase* or a *layer* — the API team, the front-end team, the build squad.

Boundaries are drawn around **activity types** rather than around outcomes. There is often a separate analysis function, a separate test function and a separate operations function, each with its own queue and its own manager.

## How work arrives

Work arrives **pre-decomposed**. By the time it reaches the person who will do it, the problem has already been turned into a solution by someone else, and the ticket describes the solution. Tickets contain acceptance criteria that read like instructions rather than like outcomes: "add field X to endpoint Y", not "the customer needs to be able to see Z".

There is a visible **refinement step whose purpose is to make work ready for execution** — specified tightly enough that whoever picks it up does not need to understand the surrounding context. "Ready" is a status, and there are rules for it.

A revealing detail: the ticket is usually written by one person and executed by another, and the writer is more senior.

## How the work is defined

The question "what is the task?" has already been answered off-stage. What remains on the team's side is "how long will it take?"

The method is held in artefacts that live outside the people: templates, definitions of done, coding standards documents, architecture decision records written by an architecture function, a reference implementation that new work is expected to copy. When something is unclear the team's move is to find the document or escalate, not to decide.

Deviation from the written approach requires permission, and the permission is granted by someone outside the team.

## Estimation and measurement

Estimation is where the Taylorist team is most recognisable. Estimates are produced per ticket, aggregated, compared against actuals, and the gap is treated as a **problem of estimation accuracy** rather than as information about the work.

Counting is of **units produced per period**: story points, tickets closed, pull requests merged, lines changed, commits. Trends are tracked over time and shown upward. Somewhere there is a chart with a line going up and to the right that has nothing to do with anything outside the team.

**Utilisation is a tracked quantity.** The proportion of a person's time that is on a ticket, billable, or assigned to a project is visible to someone, and gaps in it require explanation. Idle time is read as waste rather than as capacity.

Where there is an external supplier, time is booked against codes and the codes are reconciled monthly.

## The vocabulary

The words give it away faster than anything else. An outsider hears:

- **resource**, **FTE**, **capacity**, **headcount**, **ramp-up**, **allocation**
- **throughput**, **velocity**, **burn-down**, **utilisation**, **productivity**
- **hand-over**, **hand-off**, **sign-off**, **gate**, **ready**, **done-done**
- **scope**, **in scope**, **out of scope**, **change request**
- "**the business**" as a single actor somewhere else
- "**just** implement the ticket", "that is not **my** ticket", "who is **assigned**?"

People are referred to by count and skill class — "we need two more mediors", "we are one QA short" — more often than by name and strength.

## Meetings and rituals

Meetings are mostly **reporting and allocation** events. Standup is a status round addressed to whoever is leading, in which each person says what they did and what they will do, and the information does not change anyone else's behaviour. Planning is a filling exercise: how many points fit in the box.

Retrospectives exist and produce actions, and the actions are mostly things the team cannot do without someone else's agreement, so they recur.

Decisions appear in the team's world **already made**. There is a forum somewhere that made them; the team is informed in a meeting whose purpose is alignment.

## Who holds the method

Method sits above and outside. There is an architect, a lead, a technical authority or a central standards group that specifies how, and a layer of people who implement. The split is visible in the seating, in the invite lists and in who reviews whom — review flows one direction.

The functional split Taylor described as functional foremanship shows up in a modern form: a person doing a piece of work answers to a scrum master for process, a tech lead for method, a line manager for performance, a delivery manager for schedule and a client-side manager for scope. Each is authoritative in their own narrow domain. None of them is accountable for the whole outcome.

## Quality

Quality is a **stage**, performed by a function that receives work after it is built. Defects are counted, categorised and attributed to the stage where they were introduced. There is a notion of work being "thrown over the wall", and people use that phrase without irony.

Testing effort is estimated separately and is the first thing compressed when the schedule slips.

## How improvement happens

Improvement is a **programme**. It is initiated centrally, has a name, arrives as a rollout with training, and applies uniformly across teams. Its success is measured by adoption — how many teams are using it — rather than by effect.

Local improvements that the team makes for itself tend to be invisible to the organisation and do not survive a reorganisation.

## What a good day looks like

A good day is a day in which the planned work was completed and nothing unplanned intervened. Finishing early creates a minor problem: the person needs new work assigned. Questions are a cost, because a question means someone is not producing.

## What an outsider notices first

- Nobody in the room can say what the end user is actually trying to do, and nobody finds that strange.
- A large proportion of the conversation is about who is responsible rather than about what is true.
- The people closest to the code have the least say in what gets built, and have usually stopped offering.
- There is a lot of documentation about process and very little about the domain.
- The team's own estimates of their work are consistently wrong in the same direction, and the response each time is to estimate more carefully.
- When a person leaves, the organisation's response is to request a replacement of the same grade.

---

# Profile two: the Druckerian team

## The shape of the team

The team is organised around **an outcome that someone outside the organisation experiences**. Asked what they are responsible for, people name a part of the business, a customer journey or a service — not a layer and not a phase.

The team contains the disciplines it needs to go from a problem to something running, which usually means it is mixed and small. Nobody's job title fully predicts what they will do this week.

Asked who the customer is, people can name them, and some of them have spoken to one recently.

## How work arrives

Work arrives as a **problem or a desired outcome**, not as a specification. Items on the board are phrased as what should become true, and the question of how is open at the moment work is picked up.

The team is expected to come back and say "this is not worth doing" or "the real problem is somewhere else", and this happens often enough that an outsider will see it at least once in a week.

There is a visible step where the team **defines the task** before doing it, and that step involves the people who will do the work. Drucker's first question — *what is the task?* — is asked out loud, by the team, about their own work.

## How the work is defined

Method sits with the people doing the work. Standards exist, but they are written by the team and changed by the team, and an outsider will see them changed during the week.

Disagreements about approach are resolved inside the room, usually by someone building the smaller version and looking at it. There is an evident bias toward getting information rather than getting agreement.

The architecture is discussed by everyone, including the newest person, and the newest person's objections get answered rather than deflected.

## Estimation and measurement

The team measures **what happened outside the team**. The numbers on the wall are about users, errors in production, latency, adoption, revenue, support load, time from idea to live — things that exist whether or not the team is looking.

Measurement is pointed at the people doing the work, for their own correction, and arrives fast enough to act on. The team is the first to know when something is going wrong, not the last. This is Drucker's self-control element in its most literal form: the feedback goes to the person who can do something about it.

Forecasting exists where a date genuinely matters, and is treated as a forecast — revised when reality moves, without anyone needing to be blamed for the revision.

Nobody tracks individual utilisation. Slack in the week is not an anomaly requiring explanation.

## The vocabulary

An outsider hears:

- **outcome**, **customer**, **user**, **value**, **the problem we are solving**
- "**what are we actually trying to do here?**"
- "**what would we need to see to know we were wrong?**"
- **contribution**, **ownership**, **we decided**, **we were wrong about**
- **stop doing**, **drop it**, "**would we start this today?**"
- people by name and by strength: "ask Sara, she has been through this with the payment flow"

Absences are as telling as presences: no "resource", no "the business" as a distant actor, little talk of scope boundaries.

## Meetings and rituals

Meetings are mostly **working sessions and decisions**, not reporting. Standup, if it exists, is people coordinating with each other — the information changes what someone does next. A person can say "I am stuck" without preamble.

Decisions get made in the room, by the people present, and recorded briefly. An outsider will see someone write down what they expect to happen as a result of a decision — Drucker's feedback analysis, usually without the name — and will see an older such note being checked against what actually happened.

Retrospectives produce changes the team implements itself, and the previous round's changes are still in place.

## Who holds the method

The person doing the work knows most about it, and the organisation behaves as if this were true. Seniority shows up as more context and better questions, not as the right to specify.

Leads spend their time on obstacles, on information flow and on getting the right problems in front of the team. An outsider watching a lead for a day sees them removing things, not assigning things.

Each person can say what they are responsible for, and the answers do not overlap confusingly or leave gaps. Somewhere there is the equivalent of Drucker's manager's letter — an explicit, mutually agreed statement of what each person is accountable for — even if it takes the form of a one-page document or a recurring conversation rather than a letter.

## Quality

Quality is a property of the work as it is produced, not an inspection afterwards. The people who build something are the people who are called when it breaks, and they know this when they are building it.

There is no wall to throw anything over. The phrase does not come up.

## How improvement happens

Improvement is **continuous, local and unannounced**. The team changes its own working method from one week to another, without a programme, a name or a rollout.

Learning is visible as teaching: people explain things to each other, in pairs, in review, in writing. Drucker's point that knowledge workers learn most by teaching is observable rather than stated.

Abandonment happens. An outsider will see something deliberately stopped — a feature retired, a report no longer produced, a meeting deleted — because somebody asked whether it would be started today.

## What a good day looks like

A good day is a day where something got clearer or something real changed for a user. Finishing early is not a problem; the person goes and finds the next most useful thing, and is trusted to judge what that is.

Questions are productive, not a cost. Someone interrupting to ask "why are we doing this?" is answered rather than managed.

## What an outsider notices first

- People argue about the problem, not about responsibility.
- The quietest person in the room gets asked directly for their view, and it changes the decision.
- Someone says "I was wrong about that" early in the week, in public, with no visible cost.
- The team knows things about the customer that nobody above them knows.
- When a person leaves, the organisation's response is a conversation about what that person was actually doing and whether it still needs doing.
- A surprising amount of work is visibly **not** being done, on purpose, and the team can say why.

---

# Side-by-side signals

| Observable | Taylorist team | Druckerian team |
|---|---|---|
| Organised around | an activity or layer | an outcome someone outside experiences |
| Work arrives as | a specified solution | a problem or desired outcome |
| "What is the task?" | answered elsewhere, before arrival | answered by the team, out loud |
| Method lives in | documents and roles above the team | the people doing the work |
| Measurement counts | units produced per period | what changed outside the team |
| Measurement flows | upward, for control | to the doer, for self-correction |
| Idle time | waste to be explained | capacity, unremarkable |
| Standup is | a status report to a lead | coordination between peers |
| Quality is | a stage performed downstream | a property of the work as made |
| Improvement is | a programme, rolled out | continuous, local, unannounced |
| People are | resources of a grade | named individuals with strengths |
| Review flows | one direction, downward | both directions |
| Stopping work | requires a change request | is a normal weekly act |
| When someone leaves | request a replacement of the same grade | reconsider what the work is |
| Phrase in use | "that is not my ticket" | "what are we actually trying to do?" |

## A note on mixtures

Almost no team an outsider walks into is purely one profile. The common pattern is a team that holds Druckerian assumptions internally while sitting inside a Taylorist frame — planning its own work in the room and then reporting it upward in units of production — or the reverse, a team that uses the whole Druckerian vocabulary in its ceremonies while every observable signal belongs to the first profile.

The signals that resist being faked are the structural ones: who defines the task, where the method lives, which direction measurement flows, and what happens when somebody says the work should not be done at all.
