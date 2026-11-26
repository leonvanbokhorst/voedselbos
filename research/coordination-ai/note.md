# Where conversational or agentic AI could lighten coordination — and where it would add burden

**Issue #12.** Desk research, 26 November 2026. Public sources only; no product design, no vendor selection, no pilot, no stakeholder contact, no implementation.

**Lens: the no-software baseline.** For each coordination task the question is not "what could a model do?" but "what does current practice already achieve, and what would have to be true for a tool to beat it?" The commission's own warning — that new software may not be needed — is treated here as a live hypothesis with falsifiers, not as a disclaimer.

Marks: **[D]** documented in a retrieved source · **[C]** claimed by one actor or a self-description · **[I]** inference of this note · **[U]** not established in the sources searched · **[P]** provided by the commissioner (direct account, not public documentation). Every source id and URL is in [`sources.md`](sources.md); retrieval date, hashes and access status are there too.

This note tests, and does not inherit, the repository's existing software judgement: "a roster and a text thread suffice; the only defensible AI use is transcription with a human checking names **[I]**" ([`../BRIEF.md`](../BRIEF.md) §3; [`../experiments/note.md`](../experiments/note.md) §8). That judgement was made in the context of three specific cheap experiments. §5–§8 below say where it holds, where it is too narrow, and where it is too generous.

---

## 1. The answer in short

1. **The documented coordination cost in this ecosystem is human and relational, not clerical.** The two retrieved bodies of evidence that measure it both locate the burden in a *person who holds several roles at once* — the community-garden coordinator who designs activities, applies for money, answers volunteers, keeps the gate and absorbs whoever arrives, and the city's green advisory body whose two coordinators absorb whatever plan lands on their desk **[D]** [S13][S20]. Where the record can be measured, the explicitly administrative slice is the *smallest* slice: for Trefpunt Groen Eindhoven, "Managementtaken en administratie" is **5%** of 2025 hours against 20% communication, 15% achterban alignment and 45% advice work **[D]** [S20]. **A tool that removes administrative drag is therefore aiming at the smallest measured component of a real problem [I]**.

2. **The tasks a tool could genuinely beat the baseline on are few, narrow and largely stateless: translating and summarising one artefact, and drafting one report.** These are the two places with any measured analogue: in a municipal GenAI evaluation the largest single use, by prompt analysis, was "opstellen, samenvatten en vertalen" at 47% **[D]** [S16], and the only retrieved measurement of reporting software and reform is a fall from eight to six hours *per funder* **[D]** [S17]. Neither requires the tool to remember anything between uses, which is the property that decides whether software becomes an object to maintain **[I]**.

3. **The tasks where an AI would most plausibly add burden are exactly the ones that sound most useful: matchmaking, a live directory, onboarding, and an agent answering the front door.** Each requires the tool to hold perishable, personal or third-party data; each becomes a maintained object with an owner, and none has an owner in this ecosystem — the one node that closed had no legal entity at all **[D]** (§5). The Dutch municipal-chatbot record shows the characteristic failure is not model quality but missing local context and timing: a bot told a researcher the town hall would be open on a Monday that was a public holiday **[D]** [S15].

4. **The clearest asymmetry in the evidence is that the no-software baseline works better than the software alternatives — until the keeper leaves.** A WhatsApp/text thread and a fixed weekly slot produce documented social cohesion and are the normal Dutch civic infrastructure **[D]** [S18]; community-garden coordinators run their groups *by texting everyone to confirm sessions* **[D]** [S13]. Software is not beaten here by warmth; it is beaten by the fact that the baseline has no maintenance cost beyond the person already present — and that person is the actual single point of failure, which no tool in this record fixes **[I]**.

5. **The decision rule that follows is not "no software" but "almost always no software, and never software that remembers".** Of ten documented coordination tasks, four justify *borrowing* an existing tool under a human check — one of them (funder reporting) only where a reporting duty actually exists — and six resolve to *do nothing* (§8). **Build fails structurally** for every node in this record except the three with staff and a legal person, and for them it fails economically (§8.4).

6. **The honest answer to the commission is a negative one with a positive edge.** Nothing in the retrieved evidence supports software as a coordination layer for Eindhoven's green ecosystem in this phase, and several findings predict that building one would reproduce the exact `regeldruk` the ecosystem's own municipal programme has committed to reducing **[D]** [S12]. What the evidence *does* support is the opposite of a platform: a funded human coordinator-hour, a shared work session, and one text thread — which is what the comparable literature recommends when it is asked what would help **[D]** [S13].

---

## 2. Method, lens and evidence standard

### 2.1 Task first, technology second

The issue asks for a task-by-task assessment, so the unit of analysis is a **task** — something a named person does at a named moment — not a technology. Ten tasks were assembled from the repository's own record, not from a product taxonomy: recurring work-session scheduling, translation and plain-language access, onboarding a new volunteer, matchmaking between initiatives, knowledge capture when a keeper leaves, funder and municipal reporting, event logistics, answering routine enquiries, visibility posting, and keeping the record of who decided what. Each one appears in the issue brief, in a retrieved source, or in both. §4.2 states which are documented as costly and which are only named.

### 2.2 Three categories that must not be collapsed

The issue's own distinction is load-bearing and is applied throughout:

- **(a) Automation of administrative drag** — a machine does a bounded clerical step faster: transcribe a session, draft a summary, translate an announcement, format a report. The output is checked by a person who is accountable for it.
- **(b) Conversational access to information** — a person asks a question and gets an answer drawn from material the organisation already publishes. The failure mode is a wrong answer that sounds right.
- **(c) An agent acting on someone's behalf** — it books, enrols, sends, schedules, commits or speaks for an organisation. This adds **consent, mandate and accountability** properties that (a) and (b) do not have: someone must be able to be answerable for an act, and in this ecosystem, for most nodes, there is no legal person to be answerable **[D]** (§5.1).

Nothing in (c) is defensible here, and this note does not soften that. A tool in category (c) that sends an email under an organisation's name, or puts a volunteer on a roster that carries a legal duty (keyholder, supervisor, first aid), is performing an act of an entity that does not exist **[I]**.

### 2.3 What this note can and cannot establish

- **Can:** what the record documents about who does which coordination task and at what measured cost; what existing practice achieves; what comparable software attempts in the Netherlands and in the civic-tech literature did; what regulators and evaluations say about the current capability and its risks.
- **Cannot:** how many hours any Eindhoven volunteer actually spends on any task (no time-use data exists for these initiatives **[U]**); whether any of them wants a tool **[U]** — nobody was asked, and the exclusions forbid asking; whether a specific model on a specific date will be accurate on a specific task **[U]** — capability claims rot, so every technical claim below is dated and labelled by source type.
- **Refuses:** product design, vendor comparison, and any estimate that would imply a pilot is the next step.

### 2.4 A note on how fast this evidence decays

Every technical claim in §7 is dated. Two of the retrieved items are vendor-adjacent or self-assessed (**[C]**): a funder sector body's survey of its own grantees' reporting hours [S17], and a municipality's own evaluation of its own assistant [S16]. Where a capability claim comes from a party that benefits from it, it is marked **[C]** and not used to carry a conclusion.

---

## 3. Status of the propositions

| # | Proposition | Status | Basis | Falsifier |
|---|---|---|---|---|
| P1 | Participation in this ecosystem has a price, and the price is mostly administrative | **Established as a claim by the municipality itself [D]**; the "mostly" is **[I]** | "vrijwilligersorganisaties ervaren veel regeldruk" and `regeldruk` named as a barrier, with a programme line to reduce it [S12] | A municipal or initiative count showing non-administrative burdens dominate |
| P2 | In the one local body with paid staff, administrative work is the smallest measured slice of hours | **Established for that body [D]** | TGE urenbesteding 2025: administratie 5%, communicatie 20%, afstemming achterban 15%, advies 45% [S20] | TGE hours being unrepresentative of volunteer-run nodes — likely, and stated in §6 |
| P3 | Volunteer coordinators in community growing carry the heaviest load, and it is multi-functional | **Established in one peer-reviewed qualitative study, elsewhere [D]**; transfer to Eindhoven **[I]** | 21 interviews, Aberdeen; coordinators "experienced the greatest burdens on their time and wellbeing" [S13] | Eindhoven coordinators being staffed, insured and rota'd — true for Wasven/Phood, not for the closed node |
| P4 | The comparable literature's recommendation is funded human coordination, not tooling | **Established as the authors' policy recommendation [D]** | "Funded, centralised bodies are required to help coordinate volunteers" [S13] | A comparable study recommending software |
| P5 | Dutch municipal conversational agents fail mainly on local context and timing | **Documented in a practice test of 36 bots [D]**; the method is informal practice-testing, not a benchmark **[I]** | Bot answered a holiday-Monday opening-hours question wrongly [S15] | A rigorous benchmark of municipal bots showing contextual accuracy |
| P6 | GenAI's largest organisational use is text processing, summarising and translation | **Documented in one official municipal evaluation [D]**; productivity gain is self-report **[C]** | 47% of the >25,000 collected prompts, coded by user goal, were "opstellen, samenvatten en vertalen" [S16] | Independent time-and-motion measurement showing a different mix |
| P7 | Reporting-software/reform savings are real but small, and the binding constraint is the number of funders | **Documented at [D] for the number; magnitude modest** | 8 → 6 hours per funder [S17] | A reform showing large per-funder savings |
| P8 | Civic-tech and community-platform initiatives commonly do not sustain | **Established as a research-community consensus [D]** | "many civic tech initiatives and projects are short-lived" [S14]; German e-government cases abandoned after success [S19] | A survivorship dataset of local civic tech with high sustained rates |
| P9 | WhatsApp groups are the de facto local coordination infrastructure in NL, and they work | **Established for neighbourhood-safety groups [D]**; garden transfer **[I]** | Six case studies; "vooral een bijdrage … aan de sociale cohesie" [S18] | A comparable Dutch study of garden groups finding otherwise |
| P10 | The baseline's weak point is the person, not the channel | **Established [D]** in both the WhatsApp and garden studies | If a beheerder stops "is het mogelijk dat de hele groep hierdoor wordt geraakt" [S18]; "it would fall to bits" [S13] | Evidence that groups survive keeper turnover unaided |
| P11 | Software would fix that weak point | **Not established [U], and the retrieved evidence points the other way [I]** | No retrieved case of a tool supplying a second keeper; several of a tool acquiring one | A documented case where a tool held continuity after the keeper left |
| P12 | Any responsible use requires a legal person able to be accountable | **Inference from the accountability structure of (c) [I]**; not stated by any retrieved source | §5.1, §8.3 | A Dutch arrangement letting an unincorporated group lawfully be the controller of a processing operation |

Propositions P1–P11 are the ones an independent reviewer should attack first. P5 and P6 rest on Dutch documents that are official but not peer-reviewed, and P2 rests on a single organisation's own annual accounts.

---

## 4. What the ecosystem already coordinates with

### 4.1 The documented baseline

This is the inventory the lens requires: not "what is missing" but "what exists and what it achieves". All items **[D]**.

| Baseline instrument | Who runs it | What it demonstrably achieves | Where it breaks |
|---|---|---|---|
| **A fixed weekly slot** — Fridays 10:00–12:30, an explanation at 10:00, work, a stop at 12:00, half an hour of tasting and tea, a published winter reopening date, no obligation to come twice | one coordinator + volunteers (closed node) | the same hour served production, recruitment and belonging; visitors could walk in; a group of ~30 was claimed by 2023 | lost with the site in July 2026 — all three functions at once [S01]; the Friday design itself is documented in [`../meaning/note.md`](../meaning/note.md) §3 |
| **Two fixed monthly shifts** — klusochtend 2nd/4th Saturday, natuurwerkochtend 1st/3rd Saturday, plus daily commercial opening | paid staff + Natuurwerkgroep (Wasven) | a rhythm that does not depend on any one volunteer's availability | requires staff to exist; not transferable to a node without payroll [S06] |
| **A text thread / WhatsApp group** | one beheerder or coordinator | documented social cohesion; the normal Dutch civic channel; ~8,000 neighbourhood groups registered since 2015 | key-person fragility; deepens the digital divide; can shade into surveillance [S18] |
| **A scheduled municipal circuit** — the Klusbus, weekdays 07:30–16:00 in neighbourhoods selected on energy-poverty research | four housing corporations + municipality | coordination by timetable rather than by app; no participant-facing software at all | only works for a service that travels to people [S21] |
| **A recurring programmed evening** — eight Groen Cafés in 2025 with Bibliotheek Eindhoven, KNNV, IVN and Wasven | Trefpunt Groen (2 coordinators + 1 communications staff) | a standing venue-to-audience channel that other organisations borrow; TGE "steeds beter … actiever te communiceren" | depends on €232k turnover and a protocol mandate [S20] |
| **A wishes register** — 124 greening records, 56 still "Kans of wens", 14 with a planned year | municipality | an intake route for residents' proposals; the city itself names feedback as the weak link | no published response loop; 90 intake dates over three years (from the repository's own count, [`../participation/note.md`](../participation/note.md)) |
| **A back office you can borrow** — Supportpunt: "administration, board advice, and communication" | a staffed Eindhoven foundation | a website, built and live since 1 October 2023, for a 0.7-ha volunteer project | was used for a website and nothing else; the advisory capacity existed and was not drawn on [S02] |
| **A mailing list** | one practice, on a commercial ESP | an audience that survived the site; inbound offers of land arrived by email | held personally, in a personal brand's account; "Eindhoven heeft géén voedselbos meer" [S03] |
| **A national registration day** — Open Voedselbossendag, 5 September 2026 | Boer&Buur met Natuur / Natuur en Milieufederaties | one annual moment of public visibility with a shared map | the closed node and the Dunantpark forest were both absent; visibility infrastructure not used |
| **A two-weekly alignment + a quarterly council** — TGE coordinators ↔ municipality; CMO 4×/year | TGE + municipality | the strongest documented coordination relation in the city; 53 binding tree advices, 33 zoning advices in 2025 | advisory only; carries no obligation for anyone outside it [S20] |

**Two observations.** First, none of these instruments is a platform, and the ones that work are *rhythms* — a Friday, a Saturday, a fortnight, a season, an annual day **[D]**. Second, the only instrument in the list that failed catastrophically failed with its *site*, not with its coordination: the closure notice thanks "alle vrijwilligers die iedere vrijdag hebben meegebouwd" **[D]** [S01]. That is a tenure failure, and no coordination tool addresses it ([`../continuity/note.md`](../continuity/note.md); [`../BRIEF.md`](../BRIEF.md) §1).

### 4.2 Which tasks the record documents as costly

| Task | Documented as costly? | Where |
|---|---|---|
| Recurring-session scheduling and who-turns-up | **Yes** — arrival without notice, "taxing to find people meaningful tasks on the spur of the moment", texting everyone to confirm | [S13] |
| Translation and plain-language access | **Partly** — "Eindhoven wordt steeds internationaler" as a driver; an English-first green strand already running | [S12][S10] |
| Onboarding a new volunteer | **Yes** — induction, safeguarding, finding cover with the right training | [S13] |
| Matchmaking between initiatives | **No direct evidence of cost**; there is a documented *absence* of relations to match | [`../network/note.md`](../network/note.md) §2–3 |
| Knowledge capture when a keeper leaves | **Yes** — as a risk, not a measured cost; a fifteen-year ecovillage scores itself 1/5 on collective memory | [`../comparators/ecodorp-boekel.md`](../comparators/ecodorp-boekel.md) |
| Funder and municipal reporting | **Yes** — `regeldruk`; grant-writing; "continuous cycle of grant seeking" | [S12][S13] |
| Event logistics | **Partly** — room cost, licensing, prep hours are estimated, not quoted | [`../experiments/note.md`](../experiments/note.md) §5 |
| Answering routine enquiries | **No evidence of volume** — the only trace is a mailbox receiving offers of land | [S03] |
| Visibility posting | **Yes as a burden, weakly** — "actieve communicatie" is 20% of TGE hours | [S20] |
| Keeping the record of decisions | **Not documented at all** — no minutes, membership list or decision rules were retrievable for the region's own governance body | [`../fragmentation/note.md`](../fragmentation/note.md) §3 |

**The gap worth naming:** three of the ten tasks the issue lists have no documented cost in this ecosystem's record. That is not evidence they are cheap; it is evidence that nobody counts **[U]**. It also means any business case for a tool would be built on the issue's plausibility, not on the record **[I]**.

---

## 5. Task-by-task assessment

Each task below answers the same six questions: who does it now, at what cost, what the baseline achieves, what a tool would have to know (and therefore hold), the plausible saving, and what it would add. The verdict in each heading is this note's judgement applied to the decision rule in §8.

### 5.1 A structural point that governs every row

The closed node had **no legal entity** in any retrieved source **[D]** ([`../network/note.md`](../network/note.md) §7). That is not a technicality for this question. It determines, in order: who can be the controller of personal data; who can hold a contract with a software supplier; who is answerable for an automated message that turns someone away; and who can be sued if a volunteer is injured after being rostered by a machine **[I]**. For most of the ecosystem's small nodes, **the party that would need to own the tool does not exist**, and creating it is precisely the legal-person burden the municipality has committed to reducing **[D]** [S12].

### 5.2 T1 — Scheduling a recurring work session and filling shifts

- **Who does it now:** the coordinator, by text and by conversation at the previous session **[D]** — "Sasha regularly texted all members to confirm sessions" [S13]; for Wasven, a published standing rota (2nd/4th Saturday) does the work without anyone sending anything **[D]** [S06].
- **Cost:** not measured in hours anywhere **[U]**. Qualitatively: volunteers "were encouraged to give advance notice of attendance, but often arrived without prior notice", and coordinators "conceded it was taxing to find people meaningful tasks on the spur of the moment" **[D]** [S13].
- **Baseline:** a fixed slot plus a text thread. It achieves what a roster achieves, with no maintenance, and it tolerates the casual arrival that the design is built around. The food forest's explicit rule — nobody is obliged to come twice running — is only workable *because* no roster is enforced **[C/I]** ([`../meaning/note.md`](../meaning/note.md) §3).
- **What a tool would need to know:** names, contact details, availability, skills, and any role with legal weight (keyholder, supervisor, first-aid, safeguarding). That is a personal-data processing operation about volunteers, and a schedule that people feel bound by.
- **Plausible saving:** small. The cost documented in [S13] is not assembling the list; it is *improvising meaningful work for whoever arrives* — a judgement about soil, season and skill that a scheduler does not have.
- **What it would add:** converts a no-obligation invitation into an obligation (a shift), which is precisely the property the design was built to avoid; plus another channel; plus a controller problem (§5.1).
- **What would have to be true for a tool to beat it:** that someone is actually spending recurring hours on rota assembly, and that attendance is predictable enough to schedule. Neither is documented here **[U]**. **Verdict: do nothing.**

### 5.3 T2 — Translation and plain-language access

- **Who does it now:** nobody, systematically. The ecosystem's English-first strand is a separate volunteer run of events, "a group of sustainability-minded individuals who organize English-speaking events … guided nature walks, workshops, lectures and tours, movie nights, cleanups and gaming events", currently recruiting co-organisers **[D]** [S10]. The municipality records internationalisation as a driver of change in volunteer work **[D]** [S12]. The English-language description of the food forest that exists (Supportpunt's story page) is a *provider's* translation, not the community's **[D]** [S02].
- **Cost:** a bilingual A4 from one spoken session was estimated at "a real hour" saved with a human checking names and claims **[I]** ([`../experiments/note.md`](../experiments/note.md) §8). No measured local cost **[U]**.
- **Baseline:** a Dutch-language newsletter and site; an English-first event series that exists alongside, not inside, the Dutch one **[D]**. That is a *distributional* settlement — English speakers get their own strand — rather than a translation failure.
- **What a tool would need to know:** the source text, plus the local lexicon that no general model holds — Elburglaan, De Wielewaal, *kruidentuin*, the names of the plants and the people, and the unwritten rule ("kom gewoon langs"). If it is fed the mailing-list archive it holds the audience. **A per-message, stateless use holds nothing.**
- **Plausible saving:** real and the best-evidenced in this note. In an official municipal evaluation of a GenAI assistant, the largest single use in the prompt analysis of more than 25,000 prompts was "Tekstverwerking (opstellen, samenvatten en vertalen)" at 47% **[D]** [S16]. The gain there is self-reported, not measured **[C]**.
- **What it would add:** translation error in exactly the material where error has consequences — the timing of an event, a safety instruction, whether children are welcome, what to bring. The Dutch chatbot test found the characteristic failure was not vocabulary but context and timing: asked whether the town hall was open the coming Monday (a public holiday), a bot answered that it was open 09:00–17:00 **[D]** [S15]. A translated *and* wrong notice is worse than a Dutch notice.
- **What would have to be true for a tool to beat it:** that the same person does this often enough to justify the habit, that a human reads every output before it is sent, and that nothing is stored. All three are achievable. **Verdict: borrow, stateless, human-checked — the repository's existing judgement, confirmed and narrowed to per-artefact use.**

### 5.4 T3 — Onboarding a new volunteer

- **Who does it now:** the person who is there that morning. The food forest's whole induction was a short explanation of the day's tasks at 10:00, with visitors free to walk in **[D]** ([`../meaning/note.md`](../meaning/note.md) §3). Where the work involves vulnerable participants, induction becomes a training problem: finding cover required someone "with Protecting Vulnerable Groups training, basic knowledge of gardening and who was comfortable with the client group", described as "a major challenge" **[D]** [S13].
- **Cost:** not measured **[U]**. The documented cost is *safeguarding*, not information: the coordinator could not apply to themselves the freedom they granted volunteers, "mainly due to feelings that it would not go well without them and concerns over safeguarding" **[D]** [S13].
- **Baseline:** a human at a gate on a fixed morning. It achieves the thing onboarding is for — a stranger becomes safe and useful within one session — because a person can read the stranger.
- **What a tool would need to know:** the rules, what not to touch, who to ask, insurance and liability positions, and (for care settings) who has been trained and cleared. The last of these is special-category-adjacent personal data, and the party that would hold it does not exist (§5.1).
- **Plausible saving:** low. An induction page is not the bottleneck; the bottleneck is a person being present **[I]**.
- **What it would add:** a false assurance that someone has been inducted; a training record that implies a duty of care somebody now owes; and the temptation to let the tool stand in for the gate.
- **What would have to be true:** a legal person with a safeguarding obligation and a real induction standard. **Verdict: do nothing (write one A4 — not software).** This is the strongest case in the note for the repository's own instinct that paper beats a platform.

### 5.5 T4 — Matchmaking between initiatives

- **Who does it now:** nobody, and that is the documented finding. The network is thin: the closed node was never in Trefpunt Groen's *achterban*; its only documented edges are co-presence at a 2024 market and a Supportpunt-built website; the 13 organisations at that market produced no follow-up **[D]** ([`../network/note.md`](../network/note.md) §2–3). TGE holds the only city-wide network and its role is advisory **[D]** [S20].
- **Cost:** no cost is documented, because there is no process to cost **[U]**. What is documented is an absence.
- **Baseline:** co-presence (a market, a Groen Café), and one person's memory of who exists.
- **What a tool would need to know:** a live inventory of who has what, who wants what, and current capacity — the most perishable data in any network — plus named individuals' willingness, which is not public and cannot be scraped.
- **Plausible saving:** the *matching* is not what is missing. What is missing is a reason and a person; and the regional record contains a direct warning that adding a convening venue can *displace* the cooperation it was meant to host — "higher levels of cooperation in collaborative institutions are associated with lower levels of cooperation in other … institutions" **[D, child-reported, cross-sectional]** ([`../fragmentation/note.md`](../fragmentation/note.md) §4.7). A directory is a venue.
- **What it would add:** a maintained object (a directory that is wrong within a season), a consent problem (listing named people at other organisations), and a new channel that competes with the eight Groen Cafés a year that already convene this network **[D]** [S20].
- **What would have to be true:** someone whose paid job is brokerage, and a directory that decays gracefully. TGE already has the mandate and not the brokerage capacity; that is a staffing question, not a software one **[I]**. **Verdict: do nothing.**

### 5.6 T5 — Knowledge capture when a keeper leaves

- **Who does it now:** nobody. The twelve years of site knowledge at Elburglaan were held in one practice; the closure produced "sympathy and invitations but no public account of what was learned" **[D/I]** ([`../experiments/note.md`](../experiments/note.md) §4). A funded fifteen-year ecovillage still scores itself 1/5 on backup skills and collective memory **[D]** ([`../comparators/ecodorp-boekel.md`](../comparators/ecodorp-boekel.md)). The comparable literature says the loss is not hypothetical: "if I was just to abruptly say I was going I think it would fall to bits" **[D]** [S13].
- **Cost:** the cost is the loss, which is not a cost anyone budgets **[I]**.
- **Baseline:** none exists. This is the one task in the ten where the baseline is *nothing*, and that is the strongest argument in the note for doing something.
- **What a tool would need to know:** the archive — and here the substitution risk is at its sharpest. The knowledge is partly *in a place that no longer exists*: what grew where, what the soil did, which corner flooded. A model asked to write "twelve years on one A4" from a thin archive will produce a fluent, plausible, unverifiable document about soil it never saw. The cheap, defensible route is a **recording plus a human writing the four pages**, with transcription as the only machine step, because a person who was there can reject a wrong sentence **[I]**.
- **Plausible saving:** real but bounded: transcription converts a two-hour conversation into a draft. Nothing in the retrieved evidence suggests a model can *decide what mattered* in twelve years **[U]**.
- **What it would add:** a document that looks like institutional memory and is not; a plausible-sounding horticultural claim with no site to test it against; and, if it is published, exactly the drift the experiment's stop rule anticipates — from "what we learned" to "what we achieved" **[D]** ([`../experiments/note.md`](../experiments/note.md) §4).
- **What would have to be true:** one named author with standing in the community, one recording, one human check of every name and claim. **Verdict: borrow for transcription only; the writing is human.**

### 5.7 T6 — Funder and municipal reporting

- **Who does it now:** whoever holds the relationship — for a volunteer node, usually the same person who does everything else. `regeldruk` is named by the municipality as a barrier, with a programme line to review subsidy schemes *with* applicant organisations **[D]** [S12]. In the regional prevention architecture the reporting burden is documented as a condition imposed on participants: PACO membership, Regioraad participation, quarterly reporting, monitoring cooperation and IZA-SPUK accountability **[D]** ([`../fragmentation/note.md`](../fragmentation/note.md) §4.3).
- **Cost:** the strongest measured figure retrieved anywhere in this note: reporting "dropping from eight hours for a single funder's requirements to six hours" after a reform in a well-resourced US foundation field **[D, funder sector body's own survey of 96 institutions, not representative]** [S17]. The same source reports that "only half of respondents report using any type of digital technology like note-taking or transcription tools, pre-filled reporting templates, or other tools (that could include AI) that could help summarize submitted reports" **[D]** — i.e. adoption is partial even where capacity exists.
- **Baseline:** a document assembled once a year, in the funder's format, by the person who knows the numbers.
- **What a tool would need to know:** outputs, counts, narrative, and the funder's format — plus, for care organisations, participant data that is special-category. For a node without a legal person there is no reporting duty at all, which is why the food forest appears in no annual report **[D/I]**.
- **Plausible saving:** the only task with a measured analogue, and the analogue says **modest**: two hours per funder. If an initiative has one funder, the addressable saving is two hours a year. The binding constraint, per the same analysis, is *the number of separate accounts a participant must render*, not the form of each one ([`../fragmentation/note.md`](../fragmentation/note.md) §4.9) **[D]**.
- **What it would add:** a summarised report that is plausible and slightly wrong about the numbers is a governance failure, not a time saving; and the summary is produced by whoever holds the source data.
- **What would have to be true:** that an organisation has (i) a real reporting duty, (ii) more than one funder, and (iii) a person who checks the figures. **Verdict: borrow, drafting only, one report, human checks every number.** For a practice with no entity, this task does not exist yet.

### 5.8 T7 — Event logistics

- **Who does it now:** the organiser, using tools they already have — a ticket page, a room, a newsletter, a partner's venue. The food forest's practice ran paid offerings through a booking platform (Hipsy) and used others' platforms for visibility **[D]** (entries for Hipsy and the 2024 DDW market in [`../visibility/sources.md`](../visibility/sources.md)).
- **Cost:** estimated, not quoted: room hire at LAB-1 "perhaps €150–400, possibly in kind", ~4 hours prep per party **[I]** ([`../experiments/note.md`](../experiments/note.md) §5).
- **Baseline:** an existing scheduling/booking product plus a text thread plus one person. This task is already fully tooled; the cost is venue and hours, neither of which a model reduces.
- **What a tool would need to know:** attendee lists, access and dietary needs, payments. That is a personal-data operation for a marginal gain.
- **Plausible saving:** near zero for coordination; some for drafting the announcement, which is T2/T9.
- **What it would add:** another channel alongside the one people already use. **Verdict: do nothing.**

### 5.9 T8 — Answering routine enquiries ("the front door")

- **Who does it now:** the keeper, by email and at the gate. The only quantified trace in the local record is a mailbox receiving "zoveel prachtige e-mails van mensen die een plek heeft of iemand kennen waar we een nieuw voedselbos zouden kunnen aanleggen" **[D]** [S03]. Volume is **[U]**.
- **Cost:** **[U]**. No count of enquiries exists in any retrieved source.
- **Baseline:** a person who answers, and — critically — who can answer *differently depending on who is asking*. That is the whole advantage: a stranger who is anxious gets a different answer from a journalist.
- **What a tool would need to know:** a body of stable answers plus the local timing knowledge, and the ability to say "I don't know — ask Maartje". It would hold an enquiry log: who asked what, which is a read on the audience and on demand.
- **Plausible saving:** unknown, because volume is unknown. This is the task where the *evidence gap* is doing all the work in favour of the tool **[I]**.
- **What it would add:** the best-documented failure mode in the Dutch record. A practice test of **36 municipal chatbots** concluded "de meesten stelden zwaar teleur", finding bias, censorship, digital inaccessibility and security problems, and noting that the bots are "niet zelflerend … hoewel vaak een verkoopargument van makers" **[D]** [S15]. The failure example given is a context-and-timing error on the simplest possible question. A bot that tells a lonely newcomer "everyone is welcome, just come on Friday" when the season has ended is not a small error; it is the ersatz-relationship risk in [`../meaning/note.md`](../meaning/note.md) §6 realised as a product.
- **What would have to be true:** a stable, published, current body of answers; a visible "this is a machine" notice; an escalation route to a person; and someone whose job it is to keep the answers current. The Amsterdam evaluation shows what that looks like when an organisation is serious: the warning "ChatAmsterdam is een AI-systeem, en kan dus fouten maken. Controleer altijd de antwoorden" is "te allen tijde zichtbaar in beeld", plus e-learning and pop-ups on sensitive input **[D]** [S16]. **A volunteer practice cannot staff that.** **Verdict: do nothing.**

### 5.10 T9 — Visibility posting

- **Who does it now:** the communications worker (TGE has one, at 20% of organisational hours) or the keeper **[D]** [S20]. The ecosystem's existing distribution is other people's platforms: a green market during DDW, a Supportpunt story, TGE's Groenflits and network map, an annual national open day **[D]**.
- **Cost:** for TGE, communication is the second-largest slice of hours after advice **[D]** [S20]. For a volunteer node, unmeasured **[U]**.
- **Baseline:** a newsletter and borrowed platforms. It already reaches the audience that exists; the food forest's audience *survived* the closure as a mailing list **[D]** [S03].
- **What a tool would need to know:** event details and images with consent. Drafting is the only machine step; publishing is an act (category (c)) and needs a person.
- **Plausible saving:** real but small — drafting, not distribution. Note that the same municipal assistant's second-largest use category was "Informatie vergaren" at only 18% **[D]** [S16].
- **What it would add:** content volume without audience. **Verdict: borrow for drafting only, if anyone actually wants it.**

### 5.11 T10 — Keeping the record of who decided what

- **Who does it now:** nobody, in every node this repository examined. No minutes, membership list, decision rules or annual report exist for the closed node **[D]**; the region's own governance body has no retrievable minutes, membership list or decision rules **[U]** ([`../fragmentation/note.md`](../fragmentation/note.md) §3). The one node with a formal decision record is Wasven (three ANBI foundations, board, raad van toezicht) **[D]** [S06] — and it has staff to keep it.
- **Cost:** the cost of *not* having it is documented as a continuity risk, not as an expense **[I]**.
- **Baseline:** memory and a WhatsApp thread's scrollback.
- **What a tool would need to know:** who attended, what was decided, who is accountable. An automatically generated minute is a *record*, and a record that is wrong is worse than no record because it will be treated as authoritative.
- **Plausible saving:** a transcript plus a human edit converts an hour into a page — the same saving as T5.
- **What it would add:** a false record; and a surveillance surface (who said what, when), which is the documented shading of neighbourhood coordination channels into "doe-het-zelfsurveillance" **[D]** [S18 — different domain, transfer by analogy only].
- **What would have to be true:** a named clerk and a rule about what is recorded. **Verdict: do nothing until there is a body that decides things.** Recording decisions before there is a decision-maker is the wrong order.

### 5.12 The task table in one view

| Task | Who now | Documented cost | Baseline achieves | Tool's plausible saving | What it adds | Verdict |
|---|---|---|---|---|---|---|
| T1 Scheduling | coordinator, by text | improvisation, not assembly [S13] | works, no maintenance, tolerates casual arrival | small | obligation, another channel, controller problem | do nothing |
| T2 Translation / plain language | nobody systematically; parallel English strand [S10] | ~1 hour per artefact **[I]** | a separate English-first series | **real; best-evidenced** [S16 47%] | translation error on safety-relevant text | **borrow, stateless, human-checked** |
| T3 Onboarding | the person at the gate | safeguarding load [S13] | a stranger becomes safe in one session | low | false assurance; a duty someone now owes | do nothing (one A4) |
| T4 Matchmaking | nobody | none; an absence [network §3] | co-presence (a market, a Groen Café) | none — the venue is not the gap | decaying directory; consent; displaces existing venues | do nothing |
| T5 Knowledge capture | nobody | the loss, unbudgeted | nothing | transcription only | plausible unverifiable memory | **borrow for transcription; human writes** |
| T6 Funder reporting | the keeper | 8→6 h per funder [S17] | one annual document | **modest, measured** | a slightly wrong summary treated as fact | **borrow, drafting, numbers human-checked** |
| T7 Event logistics | organiser, existing tools | room + hours **[I]** | already fully tooled | ~none for coordination | another channel | do nothing |
| T8 Front door | the keeper | unknown **[U]** | a person who reads who is asking | unknown; volume unknown | **documented failure mode** [S15] | do nothing |
| T9 Visibility | comms worker / keeper | 20% of TGE hours [S20] | borrowed platforms + a mailing list | drafting only | volume without audience | borrow for drafting |
| T10 Decision record | nobody | risk, not expense | memory + scrollback | ~1 hour per meeting | a false authoritative record; surveillance surface | do nothing |

**Reading the table:** four tasks justify a borrowed tool used statelessly under a human check (T2, T5, T6, T9); six justify nothing at all. **That is the answer to the issue in one table, and the shape of it is a null result with four small, unglamorous exceptions [I].**

---

## 6. Where the cost actually sits

The lens requires a baseline, and the baseline has a shape that matters for the verdict.

**Two cost structures are documented, and they are different.** Trefpunt Groen Eindhoven spends €195,795 of a €232,000 turnover on staff, and its 2025 hours split roughly: 25% advising on environmental plans, 20% advising on felling permits, 20% communication, 15% aligning its *achterban*, 10% other projects, 5% intensifying the network, 5% management and administration **[D]** [S20]. Its chair reports the year as "vooral een druk jaar. Veel plannen kwamen op het bordje van onze coördinatoren terecht" **[D]**. The *volunteer* node's cost structure is nothing like this: it is one person's evenings, an unbudgeted multi-functional role, and — per the Aberdeen interviews — "the extent of the bureaucracy involved, structural restrictions, and the time and effort involved in striving towards their goals" **[D]** [S13].

**So the same word, `regeldruk`, names two different problems.** In the staffed organisation it is a small measured slice; in the volunteer node it is the difference between a practice and a job **[I]**. A tool sold to "reduce administrative burden" would be addressing 5% of one organisation's hours and an unmeasured share of one person's evenings — and the one person is the party the ecosystem has already lost once.

**The comparator that matters most is not a tool but a post.** The Aberdeen study's own policy recommendation is: "Funded, centralised bodies are required to help coordinate volunteers and to provide training and empowerment activities to encourage the sharing of workloads" **[D]** [S13]. Eindhoven's municipal volunteer programme proposes a **flexpool**, an **umbrella foundation** that takes over "het besturen en de lasten van rechtspersonen", and a **confidential adviser** — the same family of interventions, aimed at the person, not the tool **[D]** [S12]. **The documented remedy for coordination burden in this domain is a funded human and a lighter legal load, and there is no retrieved evidence that software substitutes for either [I].**

---

## 7. Evidence from comparable attempts

Fifteen attempts are tabulated. Four carry the argument and are discussed after the table. **What transfers** and **what does not** are separated in every row, because the single most common error in this literature is sliding a clinical or municipal finding into a 0.7-hectare volunteer practice.

| Attempt | What the retrieved source documents | Transfers here | Does not transfer |
|---|---|---|---|
| **36 Dutch municipal chatbots**, practice test by two named researchers, iBestuur, 12-06-2025 [S15] | "de meesten stelden zwaar teleur"; bias, censorship, digital inaccessibility, security problems; "niet zelflerend … hoewel vaak een verkoopargument van makers"; 19 of 36 in the Algoritme Register; the failure example is a holiday-opening-hours question answered wrongly | the failure mode (context, timing, local knowledge) is exactly the failure mode of a garden's front door | municipal scale, procurement, a vendor relationship, and a website with a content team |
| **ChatAmsterdam**, official evaluation, 06-06-2025 [S16] | 840 colleagues, >25,000 prompts, 7,000 chats, 3 surveys; 47% of prompts by user goal were "opstellen, samenvatten en vertalen"; risk named as sensitive input plus unreliable answers; a permanent on-screen warning; self-developed for data ownership | the task mix: text and translation dominate; data ownership is a design choice, and an expensive one | the capacity: e-learning, filters, a PIA, a product manager, a Privacy Officer |
| **Machine translation for institutional messages**, MaTIAS/Fedasil, *Revista Tradumàtica* 23, 2025 [S22] | ~400 curated practical messages, one-way only; a domain translation memory improves quality; expert human evaluation of 90 messages × 14 languages; complex or sensitive interactions "typically require … a professional interpreter"; Dutch as a source was harder than French for 9 of 14 targets; Dutch compounds mistranslated ('refteruren' → canteen "changed"; 'fluohesje' → "fluorescent bottle") | the *shape* of responsible MT here: a curated message set, one-way, evaluated, with a human for anything individual | the resources — an AMIF-funded interdisciplinary academic team |
| **Dutch speech recognition**, TU/e + TNO, ECML PKDD 2024 [S23] | Whisper on Dutch: read speech (Common Voice) WER 0.067–0.074 for the large model; broadcast/spontaneous (NPO) WER 0.185 (eloquent) to 0.837 (non-eloquent) depending on model, with the *large* model at 0.691 overall — worse than the tiny one on some categories | the realistic range for a real meeting is far worse than the demo | the corpus: NPO broadcast is professionally miked; a garden conversation is not |
| **Whisper hallucination**, ACM FAccT 2024 [S24, child-reported, not re-retrieved] | hallucinated phrases in transcriptions; worse with long non-vocal durations | the failure that a "check the names" instruction does not catch | magnitude for this domain **[U]** |
| **Retrieval-grounded answering (RAG)**, ACL 2024 [S25, child-reported, not re-retrieved] | 43.1% of 17,790 annotated responses contain at least one hallucinated span; QA subset 29.1% | "grounded" means "cites a passage", not "correct" | a 2024 benchmark on 2023-era models; current systems are [U] |
| **Acting agents**, AgentDojo (NeurIPS 2024) [S26, child-reported] + UK NCSC (2025) [S27] | agents fail at many tasks even without attack; prompt injection "cannot be fully mitigated"; mitigations must be "deterministic (non-LLM) safeguards that constrain the actions of the system" | why category (c) is not a design question but a risk-appetite question | state of the art moves; the structural point does not |
| **Automation bias**, Lyell et al. 2017 [S28] | n=120; incorrect decision support *increased* omission errors by 33.3%, 24.5%, 26.7% across conditions; commission errors in 65.8%/53.5%/51.7% of false-positive cases; correct support reduced errors by 38.3–46.6%; "Task complexity and interruptions had no impact on AB" | verification can fail even without workload pressure: the coordinator is not too busy to check, but reassured into not checking | clinical stakes, trained professionals, a simulated system |
| **Civic tech discontinuation**, CHI '23 workshop + Rehak 2023 [S14][S19] | "many civic tech initiatives and projects are short-lived. Only a few initiatives manage to sustain over time"; German cases "stalled or … been abandoned after an initial phase of broad success" | the base rate: the default outcome of a civic-tech object is discontinuation | a rate for the Netherlands or for Eindhoven **[U]** |
| **Maintenance/repair as the condition of infrastructure**, Ramakrishnan, O'Reilly & Budds [S29] | infrastructure is "dynamic materiality undergoing decay, maintenance, and repair"; the labour "enacted by ordinary people to secure connectivity and flows … often goes unremarked or understudied"; decay can be *exploited* by the powerful, shifting labour onto the marginal | the correct frame for a tool: it is not a product but a phase of upkeep with a distribution of labour | the setting (water infrastructure in Rajasthan) |
| **OSS abandonment**, Coelho & Valente, FSE 2017 [S30, child-reported] | 118 maintainers of deprecated GitHub projects; 69% had received no funding; ranked reasons: superseded (27), obsolete (20), maintainer lacked time (18), lacked interest (18) | the rival explanation: many projects "fail" because they were *finished* or replaced — the same is true of a hackathon platform | GitHub is not a garden |
| **WhatsApp neighbourhood groups**, Politie & Wetenschap, 6 cases [S18] | the baseline works: "vooral een bijdrage … aan de sociale cohesie"; groups are "professioneel opgezette structuren waar betrokkenen veel tijd in steken"; if a beheerder stops "is het mogelijk dat de hele groep hierdoor wordt geraakt"; app use can "de gesignaleerde tweedeling verder verdiepen" | the baseline's real properties: social effect, unpaid professional labour, key-person fragility, divide | domain: safety, not growing; and it shows how a coordination channel shades into surveillance |
| **Coordinator burden**, Wardle et al. 2024 [S13] | 21 interviews; coordinators carry the greatest burden; policy recommendation is "funded, centralised bodies … to help coordinate volunteers" | the intervention that the comparable literature actually recommends | UK, 2021, qualitative |
| **Reporting reform**, CEP 2025 [S17] | 8 → 6 hours per funder; only ~half of funders use any digital tool for reports; barriers named as staff capacity | the magnitude of the addressable saving | a well-resourced US foundation field; a volunteer practice is not that |
| **Mutual-aid coordination software**, uHelp (arXiv 2023) [S31, child-reported] | a volunteer-search system "tested with a community of single parents in Barcelona"; no outcome, uptake or retention measure reported | that this category of software is being built | any evidence that it works |

### 7.1 The four findings that decide the argument

**(i) The Dutch conversational-agent record fails on local knowledge, not on language.** The practice test's own example is a public holiday: the bot answered an opening-hours question with the standard hours **[D]** [S15]. The authors' diagnosis is that a chatbot "kan woorden decoderen, maar 'kent' geen betekenis", and that the easy route is the boring one — "de 'makkelijke manier' het oude[r]wetse schrijven voor een website is" **[D]**. For this ecosystem that is decisive, because the information a newcomer most needs is precisely the perishable, contextual kind: whether the ground is open, whether the season has ended, whether the gate is the one on Elburglaan. **A general model does not hold that; a person does; and a stale web page is cheaper than a confident wrong answer [I].**

**(ii) The one responsible MT deployment found is a curated, one-way, evaluated message set — and even it keeps a human for anything individual.** MaTIAS translates ~400 *pre-collected* practical messages one-way, with a translation memory and expert human evaluation, and explicitly reserves "complex, individualised interactions" for "a professional interpreter" **[D]** [S22]. That is the mature form of the task, and it is *not* "an AI that answers questions in English". It also shows the cost: an AMIF-funded interdisciplinary project with 30 staff interviews and 45 resident interviews before a single message was translated **[D]**. **A volunteer practice cannot reproduce the process, and should not reproduce the product without it [I].**

**(iii) The transcription saving is real on clean audio and unreliable on real audio.** Dutch read speech transcribes at 6.7–7.4% WER with the largest Whisper model; Dutch broadcast and spontaneous speech ranges from 18.5% to 83.7% depending on program type and model, and the *largest* model performs *worse* than the medium one overall on that data (0.691 vs 0.266) **[D]** [S23]. A separate study documents Whisper inserting whole phrases that were never said **[D, child-reported]** [S24]. So the repository's "transcription with a human checking names" is still the best candidate — and it under-states the check. **On a recorded garden conversation the realistic output is a draft where a substantial minority of words are wrong, including possibly numbers and names; the human step is a re-listen, not a proofread [I].**

**(iv) The regulator has already drawn the line that matters for the front door.** The Dutch data protection authority and the consumer authority state that organisations using chatbots "moeten mensen altijd de mogelijkheid bieden om met een medewerker te spreken", must make clear that a chatbot is in use, and must ensure it gives no "onjuiste, ontwijkende of misleidende informatie" **[D]** [S32]. This is framed as a call to *customer-service* organisations and rests on consumer law and the DSA, so its legal reach over a volunteer initiative is **[U]**; but as a design condition it is unambiguous, and it is unmeetable by an organisation with no employees **[I]**. The companion-app investigation adds the sharper warning for this ecosystem: tested chatbots answered evasively or denied being AI when asked, and "tijdens crisismomenten verwijzen de chatbots niet of nauwelijks door naar professionele hulp" **[D]** [S33].

### 7.2 The "AI as infrastructure" reading, and what it changes

The maintenance literature is the most useful frame retrieved, and it is not a warning about technology — it is a warning about *who ends up doing the upkeep*. Infrastructure is "dynamic materiality undergoing decay, maintenance, and repair"; the labour is "enacted by ordinary people to secure connectivity and flows, which often goes unremarked or understudied"; and decay can be *capitalised on* by whoever is best placed, shifting the burden onto the least powerful **[D]** [S29].

Applied here: a tool introduced into a network of volunteer nodes would be maintained by whoever has least choice about it — the same coordinator who already texts everyone **[I]**. And the civic-tech base rate says the object will outlive its maker less often than not: "many civic tech initiatives and projects are short-lived. Only a few initiatives manage to sustain over time" **[D]** [S14]. **The "AI as infrastructure" framing therefore does not make AI respectable; it makes the maintenance question compulsory, and this ecosystem cannot answer it (§8).**

---

## 8. Preconditions and a decision rule

### 8.1 Preconditions for any responsible use

These are conditions, not recommendations. Each has a test that a volunteer practice can apply in an afternoon without buying anything.

| # | Precondition | Test |
|---|---|---|
| C1 | **Name the person whose hours it saves, and the hours** | Can you write "this saves X, who currently spends Y hours a month, Z hours"? If Y is unknown, the case is not made **[U]** |
| C2 | **The baseline must be documented as failing** | What did the thread/roster/poster fail to do, and when? "It feels outdated" is not a failure |
| C3 | **The task must be (a) drag or (b) access — never (c) action** | Does the tool *do* anything (send, book, enrol, commit, speak for you)? If yes, stop: no accountable legal person exists for most nodes (§5.1) |
| C4 | **Prefer stateless** | Does it need to remember between uses? Memory is what turns a tool into an object with an owner |
| C5 | **No special-category or third-party personal data** | Whose data is in it, and who is the controller? A node without a legal entity cannot answer honestly |
| C6 | **A human reads every output that leaves the building** | Name them. Not "someone checks", a name |
| C7 | **The route to a person stays open and is stated** | The AP/ACM condition: always offer a human; and for this ecosystem the "human" is a volunteer whose phone number is public |
| C8 | **It must be cheaper to sustain than to stop** | What does it cost per year in hours to keep working? Who does that in month 14? |
| C9 | **Exit is designed before entry** | What happens to the data and the channel when the keeper leaves? This ecosystem has already run that experiment once, involuntarily **[D]** |
| C10 | **It does not become the record of who is in and who is out** | Does it create a list of people that someone could later use for another purpose? The neighbourhood-group evidence shows the drift **[D]** [S18 — analogy] |

### 8.2 The decision rule

**Do nothing** is the default, and the burden of proof runs against the tool. The order of questions:

1. **Is there a task, a person, and a measured cost?** If any is missing → *do nothing*, and if it matters, measure it first. (Three of the ten tasks in §4.2 have no documented cost at all, and four more have only a qualitative one.)
2. **Is it (c) an action?** → *do nothing*. No legal person, no mandate, no consent basis (§5.1); the agent-safety evidence says the residual risk cannot be mitigated to zero **[D]** [S27].
3. **Does it need to remember, or hold other people's data?** → *do nothing, or reduce the design until it does not.* A directory, a matchmaker, an onboarding record, and an enquiry log all fail here.
4. **Is there a paid owner for three years?** → if no, *do nothing*. The civic-tech and OSS base rates both point the same way **[D]** [S14][S19][S30].
5. **Borrow before buy, buy before build.** Borrowing means a feature of something already in use — a phone's dictation, a translation box, a word processor. Buying means a supplier, a contract and a controller. Building means a maintainer.
6. **If it survives 1–5:** one artefact, one human check, no persistence, a named reviewer, and a date at which it is switched off unless re-justified.

### 8.3 Applying the rule to the ten tasks

| Verdict | Tasks | Why |
|---|---|---|
| **Borrow** (stateless, human-checked) | T2 translation; T5 transcription; T6 report drafting; T9 announcement drafting | passes 1 (a real artefact, a real hour), 2 (no action), 3 (no persistence), 5 (a tool already present); on 4, borrowing means **no new object exists to own** — the person already doing the task uses a tool they already have |
| **Do nothing** | T1 scheduling; T3 onboarding; T4 matchmaking; T7 logistics; T8 front door; T10 decision record | fails 1 (no measured cost) or 3 (needs memory/personal data) or 2 (an action) or 4 (no owner) |
| **Build** | none | fails at 4 for every node in the record, and at 3 for every task that would justify it |
| **Buy** | none recommended | fails at 4 for the small nodes; for Wasven/Phood a purchase is a staffing decision, not an AI decision, and is outside this issue's scope |

### 8.4 Why "build" fails structurally, and not only economically

For a node with a legal person, insurance and payroll — Wasven, Phood, Trefpunt Groen — building or buying is *possible*. It is not *indicated*, for three retrievable reasons: the comparable literature's recommendation for coordination burden is funded human capacity, not tooling **[D]** [S13]; the one measured saving in the reporting domain is two hours per funder **[D]** [S17]; and the one local body whose hours are published already spends only 5% of them on administration **[D]** [S20]. **A tool aimed at a 5% slice, in the one organisation whose hours we can actually see, is not a coordination strategy [I].**

For a node without a legal person — which is the node this commission is about — building fails earlier: there is no one to contract, no one to be the controller, no one to be answerable for an automated answer, and no one to maintain it after the founder stops. **That is the structural answer to the issue, and it is a null result.**

---

## 9. Counter-evidence and tensions

The issue asks for the contradictions, so they lead rather than trail. They are numbered R1–R8 to keep them distinct from the tasks T1–T10.

**R1. A tool can relieve exactly the burden that drives exhaustion — and become the burden.** The contribution note's central finding is that the price of participation is administrative and that exhaustion is administrative ([`../participation/note.md`](../participation/note.md) §3). That is the strongest argument *for* a tool, and it is not answered by repeating that tools cost money. The honest version: **if the burden is 5% of one organisation's hours and an unmeasured share of a volunteer's evenings, then a tool must be nearly free in time to be worth it — and almost no tool is.** The retrieved case where a tool *did* address this — a municipality that built its own assistant to keep data ownership — required e-learning, filters, a privacy officer and a permanent warning banner **[D]** [S16]. **The main risk is not that the tool is bad; it is that it is good enough to be kept [I].**

**R2. The strongest case for AI in this ecosystem is the least coordination-like use.** Translation and transcription are category (a), single-artefact, stateless, human-checked — and they are also the two places with the best evidence base and the smallest data footprint (§7.1). The tasks that sound like "coordination" — a directory, a matcher, an assistant that answers newcomers — are the ones that fail the tests. **Anyone arguing for AI here should be pushed to say which category they mean, because the defensible answer is the unglamorous one [I].**

**R3. The baseline is not neutral, and "do nothing" preserves an exclusion.** A WhatsApp group and a Dutch-language newsletter are a distributional settlement: they serve the people already in the channel. The neighbourhood-group study notes that app use "kan … de gesignaleerde tweedeling verder verdiepen", and a Dutch audit documents "kanaalverleiding" — staff steering older callers towards digital channels they did not choose **[D]** [S18 (analogy)][S34, child-reported]. The ecosystem's Dutch-first default is also *why* an English-first strand runs separately **[D]** [S10]. **So "do nothing" is a choice with a cost borne by people who are not in the room — the one argument in this note that genuinely cuts against its own conclusion [I].** The answer is not a bot; it is a person, a printed notice in two languages, and a phone number, which is cheaper and more inclusive than either **[I]**.

**R4. Relieving drag can thin care — and the regulator has documented the mechanism.** The ersatz-relationship risk in [`../meaning/note.md`](../meaning/note.md) §6 is not speculative in general: a regulator's investigation of nine companion apps found they "doen zich voor als echte mensen", answer evasively when asked whether they are AI, and do not refer to professional help at crisis moments **[D]** [S33]. The transfer to a garden is by analogy and the analogy is not exact: nobody's mental health turns on a garden's opening hours. **But the design temptation is identical — a warm, always-available voice where a person used to be — and in a practice whose documented value is "someone who hosts" ([`../meaning/note.md`](../meaning/note.md) §1.6), substituting a voice for the host is not a neutral efficiency [I].**

**R5. Who owns and hosts it is already a live problem, and the answer today is "nobody good".** The closed node's audience sits on a commercial mailing-list account under a personal brand **[D]** [S03]; the region's own governance layer has no retrievable minutes, membership list or decision rules **[U]**; the city's greening-wishes register has no published response loop. **A tool would inherit a pattern of unowned artefacts rather than correct it [I].** The one retrieved case that got ownership right did it by building in-house with a product manager **[D]** [S16] — i.e. by *becoming* a software organisation.

**R6. Scale versus local control is a false choice at this size.** The tie-layer evidence puts a 30-person group's close relations at a handful ([`../meaning/note.md`](../meaning/note.md) §5), so a city-wide assistant would be serving an audience it cannot be in relationship with; and the crowding-out finding says a new venue can displace existing ones ([`../fragmentation/note.md`](../fragmentation/note.md) §4.7). **The scale argument for AI — "one tool for the whole ecosystem" — is the argument that most clearly fails here [I].**

**R7. Should AI coordinate people, or merely reduce drag on the people already coordinating?** Everything retrieved supports the second and nothing supports the first. There is no retrieved case of software supplying the thing this ecosystem is missing — a second keeper. The one attempt at mutual-aid coordination software found was tested and not evaluated **[D, child-reported]** [S31]; the agent literature says the residual risk of delegation is unmitigable **[D]** [S27]. **"AI as a coordinator" is a category error here: coordination is a relationship with a person accountable for it, and the tool cannot be accountable [I].**

**R8. The strongest piece of counter-evidence against the whole note.** If the reason coordination fails in Eindhoven is *capacity and mandate* rather than *technique* — as the regional record suggests, where the coordination function has money from 2027 but no settled owner ([`../fragmentation/note.md`](../fragmentation/note.md) §4.3) — then this note is answering a question nobody asked, and the real intervention is a funded coordination post. **That reading is compatible with everything above, and it is the one I would bet on [I].** It also explains why "no tool" and "fund a coordinator" are the same recommendation.

---

## 10. Not established

Every item below is a gap in the evidence searched, not a finding of absence.

1. **Any time-use measurement for any Eindhoven green initiative.** No source counts *volunteer* coordination hours for any local node; the one local body that publishes a work-time breakdown publishes percentages, and it is staffed **[U]**.
2. **Whether any local initiative wants any of this.** Nobody was asked; the exclusions forbid asking in this phase. Every "plausible saving" above is inference from other settings.
3. **Whether the Voedselbos volunteer group still exists**, and therefore whether any successor has a group to coordinate at all **[U]** ([`../experiments/note.md`](../experiments/note.md) §9).
4. **Any documented Dutch or European example of AI used in community-garden, allotment or green-volunteer coordination.** Searched, not found. The nearest items are a mutual-aid search prototype with no reported outcomes [S31] and municipal chatbots [S15].
5. **Current capability.** Every technical figure here is from a 2017–2026 source on a named dataset. Nothing establishes what a system released after those evaluations does on Dutch informal speech or Dutch municipal prose **[U]**. The Dutch review of nine companion apps found Dutch answers worse than English because the models were English-first **[D]** [S33] — a warning, not a benchmark.
6. **Downstream harm from a transcription or translation error in a community setting.** No study retrieved measures outcomes; the harm literature documents error classes **[U]**.
7. **Any independent cost-of-an-extra-channel measurement.** The Dutch evidence is audit testimony and qualitative **[U]**.
8. **The rate of civic-tech discontinuation in the Netherlands**, and a fortiori in Eindhoven **[U]**. The one EU-wide figure encountered (7.8% of mapped platforms inactive or discontinued) is **[C]**, from the mapping project's own brief, and its denominator is 141 platforms **[S35, child-reported, not re-retrieved]**.
9. **Whether the AI Act's deployer duties bite on a volunteer initiative at all** — no retrieved source addresses that, and the GDPR controller question is unresolved for a node with no legal entity **[U]**.
10. **Whether the municipal greening-wishes register could be opened as a data source rather than rebuilt** — plausible and unexamined **[U]**.

---

## 11. Investigation and access log

**Retrieval channel.** All retrievals via `source_read`, signed with the operator's Web Bot Auth identity (keyid `ey9Tj49-…`, agent URL `https://dsh-research-reader.complex-tang.workers.dev`). Each source's final URL, media type, sha256 and timestamp are in [`sources.md`](sources.md).

**Robots.txt.** No robots.txt exclusion blocked a retrieval in this pass, so the PI's discretionary exception was not needed for anything cited and is not relied on anywhere in this note. Two sources ([S15], [S18]) were longer than the inline return limit and were read partly through the tool's own spilled full-text file and partly by targeted extraction; the read depth for each is stated in [`sources.md`](sources.md) §1. No login, paywall, CAPTCHA, Cloudflare challenge or authentication wall was bypassed, and no User-Agent was altered.

**Access boundaries met and recorded, not worked around:**

| Resource | Status | Recovery attempted | Outcome |
|---|---|---|---|
| `dl.acm.org/doi/10.1145/3641815` ("What Does 'Failure' Mean in Civic Tech?") | **403 Cloudflare**, `cf-ray a60c2ec90fc87d36-AMS` | DOI route; the related CHI '23 workshop paper was retrieved from the TU Delft repository instead [S14] | not read; the workshop paper carries the claim |
| `research.vu.nl/…/VU_Digitale-geletterdheid-in-Nederland_2026-10.pdf` | **403 Cloudflare**, `cf-ray a60c2fa2bb2a285a-AMS` | — | not read; the digital-divide claim therefore rests on [S18] and [S34] instead |
| `informatieprofessional.nl` (report on the 36-chatbot test) | 200 but served as a compressed stream; extraction unusable | the same study's author-written account at iBestuur retrieved in full [S15] | **recovered** — a derivative of the same work, read at second hand from the authors themselves |
| `cep.org/reimagining-reporting-part-1-…` (guessed slug) | **404** | canonical blog URL found and retrieved [S17] | **recovered**, verbatim numbers confirmed |
| `amsterdam.raadsinformatie.nl` ChatAmsterdam evaluation | 200 (PDF) | — | read in full |
| `imaginecanada.ca/…/the-hidden-cost-of-funding.pdf` | **403 Cloudflare** (child-reported, `cf-ray a60c31253c5460e5-AMS`) | — | not read |
| `pmc.ncbi.nlm.nih.gov` Goddard 2012 automation-bias review | reCAPTCHA interstitial | Lyell et al. 2017 retrieved instead and verified [S28] | substituted deliberately, and stated |

**Deliberate non-substitution.** Where a source was blocked, the note either uses a different, verified source for the same proposition (Goddard → Lyell) or says the proposition is not established. No blocked source's content has been reconstructed from a search snippet, an abstract, or memory.

### 11.1 Delegation and verification

Two bounded lines ran in parallel, each with the same retrieval rules and a prohibition on spawning further agents: **civic-technology sustainability, maintenance and automation bias**, and **task-level technical and regulatory evidence** (translation, transcription, retrieval-grounded answering, agents, data protection). Neither was allowed to design anything, and both were told that "not established" was a valid return. Their raw returns are in [`working/`](working/delegated-lines.md) and are **not** evidence in themselves.

**What I re-retrieved and checked myself, and what changed:**

- **Automation bias.** The delegated note reported "56.9% more commission errors"; that figure is not in the paper. Re-retrieved: commission-error rates of 65.8%, 53.5% and 51.7%, and omission-error increases of 33.3%, 24.5% and 26.7% **[S28]**. The note uses the retrieved figures. The delegated claim that interruptions had no effect is confirmed verbatim.
- **Dutch ASR.** The delegated 0.691 WER for Whisper-large on Dutch broadcast data is correct (Table 2) but was reported without the comparison that makes it interpretable: the *medium* model scores 0.266 on the same data **[S23]**. The note states both.
- **Machine translation.** I re-read the results section rather than the abstract: the XSTS scores (Tigrinya 2.73, Somali 2.96; "only 29% of Tigrinya messages and 40% of Somali messages received an averaged shifted score higher than 3"), the one-way design, the interpreter condition and the two Dutch compound failures are all verbatim **[S22]**. The "Dutch is a harder source language" claim is true as an automatic-metric and nine-of-fourteen XSTS statement; the note reports it that way and does not generalise it.
- **Regulator statements.** Both Dutch AP items were re-retrieved and quoted verbatim, including the "always offer a human employee" condition **[S32]** and the evasive-answer and crisis-referral findings **[S33]**.
- **Reporting hours.** The delegated 8→6-hour figure was confirmed verbatim, and the source's own "not fully representative" caveat was added **[S17]**. The first URL tried was a 404; the canonical one was recovered.
- **Civic-tech discontinuation** and the **German e-government** case were retrieved directly rather than taken from the delegated return **[S14][S19]**.

**Carried as child-reported and not re-retrieved:** Koenecke et al. on Whisper hallucination **[S24]**, RAGTruth **[S25]**, AgentDojo **[S26]**, Coelho & Valente **[S30]**, the uHelp prototype **[S31]**, the Pijnacker-Nootdorp audit **[S34]** and the INNOVADE policy brief **[S35]**. Each is marked in place. **No pivotal claim in this note rests on any of them** — they support, illustrate, or are used to decline a rate.

---

## 12. Adjacent questions noticed, not researched

- **#3 participation and exhaustion** — this note takes its finding (`regeldruk` as the price of participation) as an input and does not re-test it.
- **#11 experiments** — the note says the three experiments need no software; whether they would *test* the software question is that issue's business.
- **#27 fragmentation** — the reporting-burden and "number of accounts" findings are borrowed from there; the question of whether coordination money lands with a named owner from 2027 is not pursued here.
- **#17/2.0 visibility** — a tool for "visibility of the movement" is a different question from coordination, and a worse one for AI (§5.10).
- **The municipal greening-wishes register and Klusbus as existing coordination infrastructure** — both exist, both are cheap, neither has been examined as a *substitute* for anything an initiative would build. That is the most promising unexplored line in this whole note **[U]**.
- **The 26 November 2026 workshop at Student Base** — the one moment in the record where the community itself was asked what it wants. Whether anyone asked for a tool is not public **[U]**, and if a report appears it would change the framing of this note more than any technology claim.
- **Eindhoven's own algorithmic register and AI governance** — whether the city has published rules a partner initiative could borrow. Not researched.

---

## 13. Implications for the three pillars and for the existing experiments

**Pillar 1 — De Wielewaal as central green motor.** Nothing here supports a platform argument for centrality, and something supports the opposite: the estate already possesses what the closed node lacked — staff, a rhythm, and someone whose job is hosting **[D]** ([`../network/note.md`](../network/note.md) §4). If the pillar means "a motor that hosts others' practices", the concrete form is a slot and a host, not a system. **A 145-hectare estate with four paid staff and ~100 volunteers does not need software to convene a neighbouring group; it needs a date [I].**

**Pillar 2 — a city-wide ecosystem.** This is where the temptation to build lives, and where the evidence is most discouraging. The connective layer that exists — eight Groen Cafés a year, a network map, an advisory mandate, a two-weekly municipal alignment — is *human programming*, at 20% of one organisation's hours for communication and 5% for network intensification **[D]** [S20]. Adding a directory or a matchmaker adds a maintained object to a layer that is already thin in capacity rather than in tooling. **The cheapest faithful upgrade to Pillar 2 is not a system; it is one more Groen Café, or one funded brokerage hour [I].**

**Pillar 3 — nature closer to everyday life.** The best-evidenced use in this note is the one that serves this pillar least: translating and transcribing artefacts for people already engaged. The pillar's documented mechanism is a low-threshold occasion with a person at the gate ([`../meaning/note.md`](../meaning/note.md) §7). **A conversational agent is a plausible-looking substitute for exactly that occasion, which is the substitution the AP's companion-app findings warn about in a different domain [D/I].**

**Experiment A (half-day swap).** Unaffected. It needs a text thread and one A4. The coordination cost is a host's four hours, which no tool reduces **[D]** ([`../experiments/note.md`](../experiments/note.md) §3).

**Experiment B ("Twaalf jaar op één A4").** This is the one experiment where the note's §8 verdict bites: a recording plus transcription is defensible, and the *writing must be human* — because the failure mode is a fluent, plausible account of soil the model never saw (§5.6). The note therefore **confirms the repository's existing judgement and narrows it**: transcription yes, drafting of the substantive claims no, and a re-listen rather than a proofread (§7.1(iii)).

**Experiment C (shared hosting).** Unaffected, and it is the strongest argument in the repository against this whole note's subject: an existing English-first strand, a room and two co-hosts already do what a "conversational access" tool would be built to do **[D]** [S10].

**A correction to the repository's software judgement.** [`../BRIEF.md`](../BRIEF.md) §3 and [`../experiments/note.md`](../experiments/note.md) §8 say "a roster and a text thread suffice; the only defensible AI use is transcription with a human checking names". This note finds that **too generous, not too strict**, in one respect: on realistic Dutch meeting audio, transcription error is far higher than a "check the names" step implies (§7.1(iii)). It also finds the judgement **too narrow** in one respect: a *translated* artefact is as defensible as a transcribed one, and arguably more valuable for a node whose audience is partly English-first (§5.3). Both corrections are small and neither changes the verdict.

---

## 14. Limits

1. **This is a 26 November 2026 snapshot of a fast-moving technical surface.** Every capability figure is dated; a reader in 2027 should re-date, not re-quote.
2. **The strongest local evidence is documentary, not observational.** Nothing here observes a volunteer, an enquiry or a dollar of coordination cost in Eindhoven. The measured numbers are: one Dutch body's hours split, one Dutch municipal evaluation's prompt mix, one US funder survey's reporting hours, one Aberdeen interview study's burden finding, and several datasets' error rates.
3. **Three domains are being borrowed.** The burden evidence is Scottish (2024), the baseline evidence is Dutch neighbourhood safety (2018), and the automation-bias evidence is Australian clinical simulation (2017). Each is labelled; none is a finding about Eindhoven's green ecosystem.
4. **The reporting figure is a funder-side, self-reported, non-representative survey** [C], and the note uses it only for magnitude.
5. **No local actor was asked anything,** so the note cannot say whether its verdict matches what the people doing this work actually want. That is the largest limit, and it is imposed by the issue's exclusions rather than chosen.
6. **The note has a known bias in the other direction.** It was written to test a warning, and testing a warning is not the same as being neutral. The things that would most change its mind are listed in §10, and the most likely of them is that someone in Eindhoven is already spending ten hours a week on a task this note calls cheap **[U]**.

---

## 15. Sources

Full metadata — producer, title, date, final URL, media type, sha256, retrieval timestamp, read depth, access status, and which claims each source carries — is in [`sources.md`](sources.md).

**The load-bearing items** are: the municipality's own volunteer programme and its `regeldruk` finding [S12]; Trefpunt Groen's 2025 annual report and its hours split [S20]; the Aberdeen coordinator-burden study [S13]; the Dutch municipal-chatbot practice test [S15]; the ChatAmsterdam evaluation [S16]; the MaTIAS machine-translation study [S22]; the Dutch ASR evaluation [S23]; the CEP reporting research [S17]; the civic-tech discontinuation literature [S14][S19]; the maintenance/repair frame [S29]; the WhatsApp neighbourhood-group study [S18]; and the two Dutch regulator statements [S32][S33].
