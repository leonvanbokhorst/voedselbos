# Independent review of the two revised reports (PR #26, PR #28)

**Reviewer:** independent review for the PI · **Date:** 26 November 2026
**Subjects:** `research/25-health-literacy/research/health/note.md` (PR #26, v2) and `research/27-health-fragmentation/research/fragmentation/note.md` (PR #28, v2), with their revision records, source tables and working files, compared against v1 at commit `5660f17` (health) and `988328e` (fragmentation).
**Questions:** issue [#25](https://github.com/leonvanbokhorst/voedselbos/issues/25) and issue [#27](https://github.com/leonvanbokhorst/voedselbos/issues/27).

This review does not try to produce a better verdict on gardens or on fragmentation. It tests two failure modes: whether any revised sentence still asserts more than its evidence stratum licenses, and whether the revision has withdrawn so much that the question is no longer answered. Neither report is admitted by this review; admission remains the PI's act.

---

## 1. Scope and method

**Read in full:** both revised notes (630 and 687 lines), both revision records, both `sources.md`, the health working files on COM-B/SDT, the Dutch search and assessment methods, the fragmentation working files on the funding transition, line D (organisational psychology) and line E (governance modes, grepped for the pivotal claims), plus `QUESTION.md` and both issue texts. v1 of each note was read at its conclusion and status-table sections.

**Re-retrieved and checked by me at source** (§6 has the table): Staatscourant 2026, 25830 (regeling AZWA/HLO, articles and all four annexes, the state-aid passage and the publication/entry-into-force dates); the December 2025 municipal health programme (§D finances); the October 2026 municipal budget Q&A, question 44; the RIVM GALA monitor 2025, table 2.1 and the representativeness passage; Staatscourant 2025, 36343 (the October 2025 amendment); Wiktorowicz et al. 2010 at PMC3031794 (full text); the Lubell, Henry & McCoy 2010 abstract via Crossref; JArDinS at PMC7690132 (full text); Michie, van Stralen & West 2011 at PMC3096582; the Pharos infosheet (October 2026, the URL the health note's `sources.md` records); the Vick et al. teach-back abstract; and the Verwey-Jonker *Groen Verbindt* evaluation.

**Retrieval method, stated plainly.** The small and medium documents were obtained through the signed `source_read` channel (Europe PMC XML/JSON for the papers, HTML for Pharos). The six large Dutch documents (two Staatscourant items, the municipal programme PDF, the budget Q&A PDF, the RIVM monitor and the Verwey-Jonker evaluation) were fetched over HTTPS and their text extracted locally, then searched; no access control was encountered on any of them and none was bypassed. Where a check below rests on a local extraction rather than `source_read`, the table says "full text, local extraction".

**Not verified, and said so:** the GGD board paper (`GGD`), the *Herijking* slides, the municipal subsidy scheme and award note, the 2025 *jaarstukken*, the Fontys pages, the DE STAP directory and listing pages, the VNG Q&A, and the whole of line C except Corbin. Most of §4.7–4.10 in PR #28 and §8 in PR #26 therefore remain **child-reported or single-retrieval**, as both notes already state; I did not re-verify those, and my silence on them is not endorsement.

**One methodological limit of this review.** I checked the pivotal quotations, not every number. A statement marked "verified" below means I saw it in the retrieved source; it does not mean the source is right.

---

## 2. Verdict summary

**PR #26 (health literacy, issue #25): *proportionate with changes*.** The central correction lands: the "implausible vehicle" verdict is withdrawn, the constructs are separated without being made mutually exclusive, JArDinS is re-scoped against its full text (verified), the instrument problem is separated from the assessment question (verified), and the conditional conclusions are real conditions. What remains is a small set of residual over-claims — three sentences that assert more than the source says, one that asserts a mechanism's absence from the absence of study, and one internal inconsistency in which the report's single Dutch datum is simultaneously labelled "Contradicts" and retained as the live hypothesis's (already satisfied) falsifier. **The research question remains open in the right place** — interactive health literacy is genuinely undecided — but in that one place "open" and "contradicted" are being used of the same evidence.

**PR #28 (fragmentation, issue #27): *proportionate with changes*.** This is the larger improvement of the two. The money correction is not a rhetorical softening: I re-read the successor regeling and the municipal Q&A, and the arithmetic and the two-document reconciliation hold exactly. The strata/states discipline is applied with unusual consistency, psychological ownership and territoriality are genuinely retained as open, centralisation is treated as a real rival, and the restriction/exclusion distinction is now correct. What remains: the Wiktorowicz gloss overstates what that study establishes; the five "determined" conditions are a synthesis presented as a finding; P12b's "like-for-like" label is not fair to two differently composed instruments; "indexation frozen" is asserted three times as documented and is not in the document; and one over-correction — §4.1 now says the record "documents the occurrence of none" of the seven manifestations, which is false on its own evidence for two of them. **The research question remains open where it should** (local mechanisms, resident consequences) and is answered where it can be (architecture, money, doors).

Neither report is "not yet proportionate". Neither should be accepted without the changes in §3 and §4.

---

## 3. PR #26 findings

### 3.1 The same Dutch datum is used as "Contradicts" and as the live hypothesis's satisfied falsifier

**Sentences.**
- §1.2: "| Interactive health literacy — asking, negotiating, getting help — rises with participation | **Contradicts** in the one Dutch measurement (4 in 10), **insufficient** elsewhere |"
- §5.3: "**What would falsify it:** the asking figure staying flat while contact rises (**which is what `E8` already shows**);"

**Problem.** These two statements cannot both stand. If `E8` already shows the falsifying pattern, H5 is falsified — and the report's positive claim ("a plausible setting for the relational and practical part of health literacy") rests on the falsified hypothesis. If `E8` does not show it, then the "Contradicts" state is wrong. The underlying trouble is in the source, and the report does not notice it: `E8` is **not a measurement of change over time**. The item is "Sinds het afgelopen jaar durf ik meer mensen om hulp te vragen", affirmed by 4 in 10 respondents **in each annual wave**; the 9-in-10 item is the same construction ("Ik heb het afgelopen jaar nieuwe mensen leren kennen"). There is no baseline, no comparison group and no repeated measure of the same people. A 40% affirmation of a self-reported *increase* is not a finding that asking "stays flat"; it is a finding that 40% report a rise and 60% do not, against 90% and 50% on the neighbouring items.

**Evidence.** Verwey-Jonker, *Groen verbindt zorg en de buurt* (2019), full text: "Sinds het afgelopen jaar durf ik meer mensen om hulp te vragen: elk jaar door 4 op de 10 deelnemers bevestigd"; and the later table giving 2016/2017/2018 percentages per wave. **Verified.**

**Recommended change.** Keep the gradient, drop both over-readings.
- State the row as: "Interactive health literacy — asking, negotiating, getting help — rises with participation | **Insufficient**: the one Dutch datum is a self-reported change item with no baseline (4 in 10 report *more* daring to ask, against 9 in 10 reporting new contacts); **measure-unsuitable** for the proposition as stated."
- Replace the falsifier sentence with: "**What would falsify it:** a repeated measure in one cohort in which asking does not rise while contact does. `E8` is consistent with a weaker asking effect but cannot show this, because it is a cross-sectional change item."
- Add one sentence to §3.1's table noting that `E8`'s three items are all retrospective change items, so the 9/5/4 comparison is a comparison of *reported changes*, not of levels.

### 3.2 "but not knowledge" overstates a "no clear pattern" at very low certainty

**Sentence.** §1.1 finding 10: "teach-back … improves **self-efficacy** (SMD 2.40, very low certainty) and **short-term adherence** (SMD 1.04, low certainty) but **not knowledge** [D, `F9`]."

**Problem.** The source says the opposite of "not": nine RCTs could not be pooled, and "there was **no clear pattern** of the effect of teach-back on knowledge (very low COE)". "No clear pattern" is the absence of an adjudicable result, not a null. The same sentence also uses "improves" for an effect whose confidence interval runs from 0.37 to 4.44 with "substantial heterogeneity" — the source's own caveat, which the note prints in §5.2 and §7 but drops in the headline finding where most readers will meet it.

**Evidence.** Vick et al., *J Gen Intern Med* (2026), abstract: 18 RCTs, n = 1985; "no clear pattern of the effect of teach-back on knowledge (very low COE)"; SMD 2.40 (0.37–4.44), very low; SMD 1.04 (0.45–1.64), low; "large confidence intervals that ranged from small to large effect sizes and had substantial heterogeneity". **Verified.**

**Recommended change.** "is associated with large but very imprecisely estimated gains in self-efficacy (SMD 2.40, 95% CI 0.37–4.44; very low certainty; substantial heterogeneity) and in self-reported short-term adherence (SMD 1.04, 0.45–1.64; low certainty), and with **no clear pattern** on knowledge (very low certainty)". The practical payload ("one teach-back question is the cheapest check") does not need the stronger verb; it rests on feasibility, not effect.

### 3.3 "no mechanism: reading is not what happens there" is the error the revision exists to correct

**Sentence.** §3.2: "**Not claimed:** that a garden produces **functional** health literacy (**no mechanism: reading is not what happens there**)".

**Problem.** This asserts a fact about garden practice — that no reading occurs — and it is exactly the move the revision forbids: inferring the absence of a mechanism from the absence of a study. Gardens involve seed packets, labels, recipes, signage, apps, planting calendars and, in this repository's own material, herbal-remedy material where misreading a dose matters. The report has no observation of any garden's literacy demands anywhere; §4.4's COM-B audit is proposed precisely because nobody has made one.

**Evidence.** No retrieved source observes the literacy demands of a garden. The note itself says so: P33–P34, §5.4 and §15 all record that no one has looked. **Not established.**

**Recommended change.** "**Not claimed:** that a garden produces **functional** health literacy — no retrieved source observes its reading or numeracy demands, and the setting's documented features (a person present, a task, a recurring time) are not textual [I]". This keeps the claim the evidence supports and stops asserting the one it does not.

### 3.4 The 52.8/52.3 discrepancy is misdiagnosed as factsheet sloppiness; it is more probably a report revision

**Sentences.** §6.1: "The band is 44.3–52.8%, and the factsheet itself is internally inconsistent — 52.8% in the headline range, 52.3% in its own explanatory paragraph." `sources.md`: "the Pharos factsheet cites the *revised* report, RIVM 2026-0107. That version's full text was not obtainable … so the note quotes the earlier version 2026-0076, **whose headline figures are identical**."

**Problem.** Both halves of this are checkable and one is wrong. The factsheet today gives "44-52,8%" in the headline and "**52,3% (Q47)**" in the explanatory paragraph, and its source list names **2026-0107** as the "Herziene versie van rapport 2026-0076". So the factsheet is internally inconsistent *and* it is citing a revision the note never obtained; the most economical explanation is that 52.3% is the **revised** Q47 figure and 52.8% is the un-updated headline. The `sources.md` claim that the two versions' headline figures are "identical" is therefore an assumption, not a finding, and if it is wrong the band's upper bound is 52.3% and "44.3–52.8%" mixes two versions of one report.

**Evidence.** Pharos infosheet, October 2026, retrieved 26 November 2026: headline "44-52,8%"; explanatory paragraph "In plaats van 52,3% (Q47) was dit volgens de Q12 46,6% in de algemene bevolking en 44,3% in het Nivel-consumentenpanel"; source list "Rapport nr. 2026-0107. Herziene versie van rapport 2026-0076". **Verified** that the factsheet says this; **not verified** that 0076 says 52.8%, because 0076 was not re-read by me and 0107 was never obtained.

**Recommended change.** "The band is 44.3–52.8% as reported in the two 2025 surveys; the Pharos factsheet that quotes them gives **52.3%** for the Q47 in its explanatory paragraph and cites a **revised** RIVM report (2026-0107) whose full text was not obtained, so the upper bound is uncertain between 52.3% and 52.8% [D/U]." The consequence for the argument is nil — nothing rests on 0.5 points — but the note should not resolve a version question as a proofreading error.

### 3.5 The "Outcome" condition silently re-specifies the claim it is meant to test

**Sentence.** §1.3A, table row: "| **Outcome** | the outcome is **task capability, asking, appraisal-in-a-situation** — measured by performance, teach-back or observation | the outcome is a population HLS19/HLQ score … |" — introduced by "Every row must hold for the claim 'this garden strengthened health literacy' to be defensible".

**Problem.** This is the one row that does not condition the claim; it replaces it. As written, the only admissible evidence for "this garden strengthened health literacy" is evidence about **task capability**, measured by performance or observation — and the note itself says that is a different construct (§3, §7). A reader is entitled to conclude that the health-literacy claim has been redefined into a capability claim and then described as conditional. That is not unfalsifiable in the ordinary sense — the row can fail — but it cannot fail *as a health-literacy claim*, because no health-literacy outcome is admissible.

**Evidence.** The note's own §3 and §7; no garden-suitable interactive- or critical-HL instrument exists in the retrieved record (P32, §5.4). **Established on the report's own evidence.**

**Recommended change.** Rewrite the row as two rows:
- "**Outcome (capability claim)** — task capability, asking, appraisal-in-a-situation, measured by performance, teach-back or observation [D, `F9`,`F8`]"; and
- "**Outcome (health-literacy claim)** — a validated measure of interactive or critical health literacy. No such measure suitable for a garden was retrieved [U]; the population instruments are measure-unsuitable (§7). **This row currently cannot be satisfied, and that is why the claim remains Insufficient.**"

The second row is the honest statement of the position and is more useful than the current single row, because it tells a reader exactly what is missing rather than implying a test exists.

### 3.6 A universal negative in the body where the status table is careful

**Sentence.** §6.5, bold heading: "**Nobody measures the after-the-end period.**"

**Problem.** P11 states this correctly ("No retrieved study measures outcomes after participation ends or a site closes — **not established in the sources searched**"). The body sentence converts a search result into a fact about the world, in the same note whose §2.1 rule 1 forbids exactly that.

**Evidence.** No basis for the universal negative; the note's own P11 basis is "`B` §4.3, `D` §4". **Contradicted by the note's own status.**

**Recommended change.** "**No retrieved study measures the after-the-end period.**"

### 3.7 What would make PR #26 acceptable

Findings 3.1 and 3.5 are the two that matter conceptually; 3.2, 3.3, 3.4 and 3.6 are sentence-level repairs. With those six changes the report is proportionate to its evidence, and the research question is open in exactly one place — whether a garden carries interactive health literacy — which is where the issue wants it open.

---

## 4. PR #28 findings

### 4.1 §4.9 attributes to Wiktorowicz et al. a mechanism the study does not identify, and upgrades a weak lever into a "failure mode"

**Sentences.** §4.9: "the one comparative study … finds that a corporate structure supported by regionalisation 'offered the most direct means' to inter-organisational collaboration. **But the mechanism is not the *existence* of a centre: it is the alignment of budget authority with planning authority.**" And: "**A strategy board without resource authority is a documented failure mode, not a weak version of a working model**".

**Problem.** The study's own abstract puts the structural finding first: "A *corporate structure* supported by regionalization offered the most direct means for local governance to attain inter-organizational collaboration", and the paper's discussion adds that "the appointment of a director with jurisdiction for institutional and community services … was key". Budget/planning alignment appears as a condition that "supported their governance capacity", and its absence as networks "lack[ing] a key governance lever". That is a **supporting condition**, not a replacement mechanism, and the note's "not the existence of a centre: it is …" reverses the paper's emphasis. "Documented failure mode" is also stronger than the evidence: the study documents reduced leverage and unaccountable hospitals, not an observed failure of an arrangement to achieve outcomes.

**Evidence.** Wiktorowicz et al. 2010, *Int J Integr Care* 10(4):e60, PMC3031794, full text: abstract Results; section "Aligning budget authority with service planning" — "we found network governance was less well supported when the province set organizational budgets while networks oversaw service planning, as networks lacked a key governance lever"; "hospitals were not held accountable". "In all 96 key informants participated" — the note's "96 informants" is correct. **Verified.**

**Recommended change.** "The study finds that a **corporate structure supported by regionalisation** offered the most direct route to collaboration, and that **where budget authority was separated from service planning the networks 'lacked a key governance lever'** and hospitals 'were not held accountable'. Its implication for the regional proposal is narrower than a mechanism: *structure plus aligned authority* worked; **planning without budget authority is a documented weakness**, not a demonstrated failure mode."

### 4.2 The five "determined" conditions are a synthesis presented as a finding

**Sentences.** §1 finding 5: "What is determined are five conditions that predict documented outcomes under *either* form — authority aligned with resources, completeness of implementation, coordination burden, the number of separate accounts, and whether competitive allocation sits in the same body as coordination…" §4.9: "What *is* determined is a different and more useful thing: **the variables that predict documented outcomes are the same under either form.**"

**Problem.** No retrieved study tests these five as a set, under either form, in health promotion or anywhere else — as the same section says two paragraphs later ("No retrieved study tests the two head-to-head"). The five are drawn from five different literatures in five different domains and levels: Canadian mental-health networks (structure and budget alignment), English hyperacute stroke reconfiguration (implementation completeness), English inter-municipal cooperation (coordination burden), foundation reporting reform (hours per funder), and health-promotion tendering (competition). Calling their conjunction "determined" and "predictive" is an inference of the report's, and it is the most consequential inference in the revision because it is what replaces the centre-versus-middle verdict.

**Evidence.** The five sources are as cited in §4.7 and §4.9; none tests the set; condition 4 is reported as an 8-to-6-hours movement, described by the note itself as "real, but small"; the competitive-tendering quotation is a single line from one line-E source. **Child-reported, abstract-level, different levels and domains.**

**Recommended change.** "What the retrieved literature **does** supply is five conditions, each associated with documented outcomes in **at least one setting**, and which this note **infers** would matter under either form. None has been tested as a set, none in health promotion, and the list is a synthesis, not a finding [I]." P39's "the conditions are **established**" should become "each condition is supported somewhere; the set is an inference".

### 4.3 P12b's "like-for-like" label is not fair to two differently composed instruments

**Sentence.** P12b: "Like-for-like, the 2027 local allocation (€3,632,993 including NPLV) is **approximately equal** to the 2026 SPUK-GALA envelope for Eindhoven (€3,582,000), with a different composition and different conditions."

**Problem.** The arithmetic is right and the two figures are the right *totals* to compare — but they are not like-for-like. The 2026 envelope was the broad GALA SPUK, covering the full GALA theme set; the 2027 local allocation is an AZWA/HLO instrument that **adds HLO (mantelzorg/logeerzorg) money** and continues **four named ketenaanpakken** while the VNG states that outside those four "blijven er geen structurele middelen over vanuit GALA". A total that is 1.4% higher can therefore conceal a loss in themes that are no longer funded and a gain in themes that were funded elsewhere. The note knows this (P12b's own caveat, §8, §9 item 10) but the label "like-for-like" and the phrase "approximately equal" invite exactly the inference the caveat then withdraws.

**Evidence.** Regeling AZWA en HLO, Bijlagen 3 and 4 (Eindhoven €3,103,887; Woensel Zuid €529,106) — **verified**; municipal programme §D (€3,582,000 SPUK-GALA; €647,000 own funds; 2027 €739,000 own funds) — **verified**; VNG Q&A quotation as carried by the note — **not re-verified**.

**Recommended change.** "**Total-on-total** (not like-for-like per theme), the 2027 local allocation (€3,632,993 including NPLV) is within 1.4% of the 2026 SPUK-GALA envelope for Eindhoven (€3,582,000). The instruments are not comparable per theme: the 2027 figure includes HLO money and four continued ketenaanpakken, and no per-theme comparison exists [U]." Add a sentence to §4.3(d): "equality at the total level is not evidence of equality of prevention capacity."

### 4.4 "The successor allocation for this region is larger than the envelope it replaces" rests on an unreconciled, child-reported baseline

**Sentence.** §1: "the successor allocation for this region is larger than the envelope it replaces and is addressed to municipalities and GGDs, not to community practices."

**Problem.** The comparison is €5,968,460 (2027 regional AZWA/HLO) against the 2025 IZA-SPUK entitlement of €4,436k recorded in the *jaarstukken* — a figure the report itself carries as **provisional** because "the figures do not fully reconcile" (P24), retrieved by a delegated line and not re-read by the Lead. The AZWA/HLO envelope also contains HLO money the IZA-SPUK did not, so "larger" may be composition, not capacity. This is the one place where the revision's own status discipline slips: a *prospective* amount is compared to a *provisional/actual* amount and the result is stated in the answer without its status.

**Evidence.** P24 and §4.3(h) for the provisional status; Bijlage 1 for €5,968,460 — **verified**; the €4,436k entitlement — **not verified** (child-reported). **The comparison's baseline is the weak link.**

**Recommended change.** "the 2027 regional allocation (€5,968,460) is larger than the **provisional, unreconciled** 2025 IZA-SPUK entitlement recorded in the accounts (€4,436k), a comparison that mixes AZWA and HLO money and cannot yet be read as an increase in capacity [D/U]".

### 4.5 "Froze indexation" is asserted three times as documented and is not in the document

**Sentences.** P3: "the 2023–2026 regeling was cut 10% for 2026, **indexation frozen**, and it lapses 16 July 2027". P27: "cut the 2026 budget by 10%, **froze indexation**, added €43m…". §4.2: "The same instrument cut the 2026 budget by 10%, **froze indexation**…".

**Problem.** The amendment says the opposite of "nothing about indexation": it says the 2024 *loon- en prijsontwikkeling* (LPO) was **added** to the 2025 and 2026 tables. The tables' two columns are "Totaalbedrag excl. LPO" and "Totaalbedrag incl. loon- en prijsontwikkeling (LPO) uit 2024" — which is consistent with **no 2025 or 2026 LPO having been added**, i.e. with indexation being frozen in effect, but the document never says "bevroren" or "geen indexatie". The note has converted an inference from a table into a documented fact, in three places, and in a paragraph whose point is that other people cite half a reform.

**Evidence.** Staatscourant 2025, 36343, full text, local extraction: "Tevens is ook de toegepaste indexatie (in de vorm van uitkering van loon- en prijsontwikkeling …) uit 2024 over 2025 en 2026 aan de tabel voor de jaren 2025 en 2026 in bijlage IV toegevoegd"; no occurrence of "bevriez-", "geïndexeerd" or "prijsbijstelling" other than in the LPO columns. **Verified that the document says this; "frozen" not verified.**

**Recommended change.** "cut the 2026 budget by 10% and applied only the 2024 LPO to 2025 and 2026, with no 2025 or 2026 indexation in the tables [D]; that amounts to a freeze [I]". Or simply drop "froze indexation" — nothing in the argument depends on it.

### 4.6 P25 is stratum S1 but is the region's own analysis — S2

**Row.** "| P25 | The region analysed three citizen initiatives; they score positively on several social-coherence indicators but not consistently on health behaviours, and causal attribution is stated as impossible | **S1** | Supports | kept | `HERIJKING` §8.1–8.5 |"

**Problem.** §2.1 defines S2 as including "the region's self-diagnosis", and S1 as statutes, budgets, board papers, governance rules, amounts, dates. A regional project group's ecological comparison of three villages is a self-analysis: the fact that the *document* exists is S1, but the proposition asserted is what the region concluded, which is S2. Every other monitor-derived proposition (P6, P7, P8) is correctly S2; this one is not. It matters because the row is then read in §1 finding 5 and §4.5 as evidence about plurality rather than as the region's own reading.

**Evidence.** §2.1's own definitions; the *Herijking* is produced by the regional project group (note §4.3(f)), which the note elsewhere treats as a regional self-assessment (§5.9). **Contradicted by the note's own scheme.**

**Recommended change.** Stratum "**S2** (regional self-analysis, ecological, causal attribution disclaimed)".

### 4.7 The Lubell crowding-out finding is real, but the note turns an association into a test of new venues and does not carry its status in line

**Sentences.** §5.21: "A study of land-use and transportation planning institutions finds that 'higher levels of cooperation in collaborative institutions are associated with lower levels of cooperation in other land-use and transportation planning institutions'… **Adding a convening venue can crowd out the cooperation it was meant to host.**" §4.9: "**A 'missing middle' route is a new venue, and the one study that looks finds new venues can crowd out the cooperation they were meant to host.**"

**Problem.** The quotation is exactly right — this is the report's strongest counter-evidence and it survives. What does not survive is the **temporal and causal** step: the study is a cross-sectional survey of policy actors in five California regions, testing the ecology-of-games expectation that "collaborative institutions may actually reduce the amount of cooperation in existing policy venues". It observes an association between venues, not the introduction of a new one, and it is not a study of health promotion. "The one study that looks finds new venues can crowd out" is therefore a claim the study does not make. Separately, the note cites it in line as "[D, line E]" while `sources.md` and the revision record both say it is child-reported and unverified; the sharpest counter-evidence in the report is the one place where the verification status is least visible to a reader who does not open `sources.md`.

**Evidence.** Lubell, Henry & McCoy 2010, *AJPS* 54(2):287–300, Crossref-deposited abstract: "The ecology of games framework … identifies several reasons why collaborative institutions may actually reduce the amount of cooperation in existing policy venues. Analyses of survey data from policy actors in five California regions demonstrate that higher levels of cooperation in collaborative institutions are associated with lower levels of cooperation in other land-use and transportation planning institutions." **Verified at abstract level** (full text not read; no need for the claim as reworded).

**Recommended change.** "One retrieved study, a cross-sectional survey of policy actors in five California regions, finds that **more cooperation in collaborative institutions is associated with less cooperation in other land-use and transportation planning venues** [D, abstract, child-reported]. It is the sharpest counter-evidence in this report to *any* new convening route, and it is an association, not a test of adding one." Add "(child-reported, abstract only)" in the §4.9 bullet.

### 4.8 The over-correction: "the occurrence of none of them"

**Sentence.** §4.1: "**the record documents the conditions under which four of the seven could occur, and it documents the occurrence of none of them.**"

**Problem.** On the note's own evidence this is too strong for two of the seven. Manifestation 4, "incompatible eligibility or reporting requirements", is *documented*: the broad SPUK's 15 parts with separate SiSa lines and "een intensieve administratieve last" is a reporting-requirement artefact, reported by the implementers who bear it (S2), and the October 2025 amendment exists because of it. Manifestation 5, "repeated temporary pilots without continuity", is documented as an arrangement — a one-year GGD penvoerderschap followed by a three-year instrument with no named owner — though not as an observed discontinuity. v1 said the record "documents manifestations 4 and 5 most clearly"; that was closer to right than "none". The correction has overshot: to avoid treating the absence of resident-level instruments as a negative finding, the report has also denied the presence of the documentary ones.

**Evidence.** §4.2 (the MTR quotation and the amendment); §4.3(d) (the one-year bridge and P11a); the note's own S2 label for P4. **Verified.**

**Recommended change.** "**The record documents two of the seven as arrangements and reported burdens — incompatible reporting requirements (4) and time-limited instruments without an owner (5) — and documents none of the other five as an observed consequence.** That distribution is a finding about evidence, not about the system." This is both more accurate and more useful: it tells a reader which two are worth pursuing.

---

## 5. Over-caution audit

**PR #26.** The failure mode here is **not** silence. §1 gives a usable answer ("a plausible setting for the relational and practical part of health literacy … never studied"), §1.3 gives conditions with visible failure modes, §1.3B gives a cheap test, and §12 lands the practical conclusion ("the pillar with evidence under it … does not need health literacy to justify itself"). Two places stopped answering more than the evidence requires:

1. **The asking datum (3.1).** Because the report cannot decide whether `E8` contradicts H5 or not, it neither claims the mechanism nor drops it. The evidence now in hand supports a third, more useful sentence: *"The one Dutch measurement shows that most volunteers report new relationships and a minority report more willingness to ask for help; that is consistent with the mechanism operating weakly or not at all, and it cannot distinguish the two."* That is a finding, and it is what a decision-maker needs.
2. **The functional-literacy "no mechanism" claim (3.3).** Withdrawing the assertion would leave the report with *more* to say, not less: a garden's literacy demand profile is an open, cheap, observational question, and the report already has the method (a COM-B audit, §4.4).

**PR #28.** The revision's caution is well judged overall, with two exceptions:

1. **"The occurrence of none of them" (4.8).** This is the clearest over-correction in either report. The two documented manifestations can be re-asserted now, from documents already retrieved, and doing so gives the reader the one thing the current text withholds: *which* fragmentation mechanisms are actually visible in this region.
2. **The centre-versus-middle weighing.** §4.9 lists the centralising case and its limits with care, then concludes that the contest is "under-determined". The evidence it has already assembled is **asymmetric**, and saying so is not a verdict: the *costs* of centralisation are documented as observed outcomes (102 English hospital mergers with "no gains beyond reduced activity"; nine trust mergers undershooting savings by a third with staff reporting "a decrease in the autonomy of services and local decision making"; mandated collaboration shifting cooperation "from trust to contract" and producing "collaborative inertia"), while the *benefits* are documented only under conditions the region's proposal does not yet state (aligned budget authority; complete implementation). A report can say that asymmetry is itself the finding without choosing a side: *"the documented costs of centralisation are outcomes; the documented benefits are conditions. That is an asymmetry in the evidence, not a preference in the report."* That sentence would make §4.9 more usable and more honest at once.

**A note on what was rightly withdrawn.** v1's "binding constraint … is the funding and accountability design, not the absence of goodwill" was an inference stated as a conclusion, and withdrawing it was correct — the reform has changed the design and produced no observable consequence. v1's "the exclusion, if any, is at the door … built for incumbents" was an attribution of intent, and withdrawing it was correct. Neither withdrawal leaves a hole: P22 and §5.18 fill both.

---

## 6. Citation verification table

**Legend:** *verified* = I saw the quoted or asserted content in the retrieved source · *not verified* = could not be checked or the source does not state it · *contradicted* = the source says something else. Retrieval method noted where it was not `source_read`.

### PR #28 (fragmentation)

| # | Claim as used in the note | Source | Result | What I saw |
|---|---|---|---|---|
| 1 | Region 42 "Zuid Oost Brabant" (mandaathouder Eindhoven) receives **€5,968,460** for 2027 | Stcrt. 2026, 25830, Bijlage 1 | **Verified** | "42. Zuid Oost Brabant Eindhoven … € 5.968.460 € 7.229.835 € 5.199.328" |
| 2 | Eindhoven **€3,103,887** local; Woensel Zuid **€529,106** NPLV; GGD BZO **€155,110** | Bijlagen 3, 4, 2 | **Verified** | "Eindhoven € 3.103.887 € 3.736.900 € 4.317.066"; "Eindhoven Eindhoven Woensel Zuid € 529.106"; "GGD Brabant-Zuidoost € 155.110" |
| 3 | Ambtshalve allocation 2027–2029; regional coordination a named activity (art. 2.1(2)(c)); GGD 2027 allocation (2.1(3)); werkagenda by 1 March 2027 (4.1); 100% voorschot (5.1(4)); 70% carry-over (5.2); lapses 16 July 2030 (8.2); in force 22 July 2026 | Stcrt. 2026, 25830 | **Verified** | Article text read; "Deze regeling vervalt met ingang van 16 juli 2030"; publication date "21-07-2026 09:00", in force "de dag na de datum van uitgifte" |
| 4 | Municipalities may not pass on "ongeoorloofde staatssteun" directly or indirectly | Stcrt. 2026, 25830, toelichting "Staatssteun" | **Verified** | "Gemeenten mogen met de uitkering geen ongeoorloofde staatssteun verlenen aan derden en er mag ook geen indirecte staatssteun worden verleend" |
| 5 | €4,229,000 (2026) → €739,000 (2027); cause "(mogelijk) wegvallen"; "alle GALA-enveloppen (alleen voor 2026)"; 2026 covered by €647,000 own + €3,582,000 SPUK-GALA | Municipal programme, §D | **Verified** (PDF, local extraction) | Exact figures and wording; "Er zijn geen structurele verplichtingen ten laste van de SPUK-GALA die doorlopen na 2026" |
| 6 | City's own Q&A puts the AZWA addition at "ca. 9,6 miljoen", budget-neutral, and says the money is "niet opgenomen in de begroting 2027 t/m 2029" | Budget Q&A 2027, q.44 | **Verified** (PDF, local extraction) | "aan de lastenkant komt er een bedrag van ca. 9,6 miljoen bij (dit betreft AZWA-middelen regionaal, lokaal en nationaal programma leefbaarheid en veiligheid voor gebied Woensel Zuid) … Hierdoor blijft het saldo gelijk" |
| 7 | Regional + local + NPLV = **€9,601,453** | arithmetic | **Verified** | 5,968,460 + 3,103,887 + 529,106 = 9,601,453; matches "ca. 9,6 miljoen" |
| 8 | Wiktorowicz: corporate structure "offered the most direct means"; ten networks; **96 informants**; "lacked a key governance lever"; hospitals "were not held accountable"; heading "Aligning budget authority with service planning" | PMC3031794 | **Verified** | All present verbatim, including "In all 96 key informants participated in the research from 2003 to 20…" |
| 9 | "the mechanism is **not the existence of a centre**: it is the alignment of budget authority with planning authority" | same | **Not verified as stated** (interpretation) | The paper credits the corporate structure *plus* regionalisation as "the most direct means" and treats alignment as a supporting condition. See 4.1. |
| 10 | "higher levels of cooperation in collaborative institutions are associated with lower levels of cooperation in other land-use and transportation planning institutions" | Lubell, Henry & McCoy 2010, abstract (Crossref) | **Verified** (abstract only) | Sentence appears verbatim; study is a cross-sectional survey in five California regions. The note's "new venues can crowd out" is an inference. See 4.7. |
| 11 | Joint decision-making 67%→36%; responsibilities 55%→43%; coordination agreements 60%→48%; financial agreements 52%→41% (insurers 44%→60%); n=42; agreements with implementers 37%→46%; referrals 27%→39% | RIVM GALA monitor 2025, table 2.1, p.24 | **Verified** (PDF, local extraction) | Table read; all figures and both n's match, and the opposite insurer movement is as the note states |
| 12 | "Inwoners worden wel geleidelijk meer betrokken bij de planvorming, maar minder in de fasen daarna" | GALA monitor, p.32 | **Verified** | Verbatim |
| 13 | RIVM records the possibility of "een rooskleurige voorstelling van de voortgang" | GALA monitor, p.93 | **Verified** | Verbatim, with the representativeness caveat around it |
| 14 | 2026 budget cut 10%; €43m added from AZWA/HLO; regeling lapses 16 July 2027 | Stcrt. 2025, 36343 | **Verified** | "Het uitkeringsbudget voor het jaar 2026 wordt gekort met 10%"; "In 2026 wordt € 43 miljoen toegevoegd vanuit het … AZWA … en het HLO"; "de Regeling, die vervalt met ingang van 16 juli 2027" |
| 15 | "froze indexation" | same | **Not verified** | The document says the **2024 LPO was added** to the 2025 and 2026 tables; no freezing provision. See 4.5. |
| 16 | Fitcoins platform not live; "alle voorgenomen acties … zijn uitgevoerd" | Municipal programme, §B | **Verified** | "Vanwege technische problemen is het platform nog niet gerealiseerd. Hierdoor kunnen inwoners zich nog niet aanmelden in de app" |

### PR #26 (health literacy)

| # | Claim as used in the note | Source | Result | What I saw |
|---|---|---|---|---|
| 1 | JArDinS: "no significant impact, in spite of sufficient statistical power" | Tharrey et al. 2020, PMC7690132 | **Verified** | Abstract, verbatim |
| 2 | Power computed for **one** outcome (+1 portion/day), target 160 (80/80), 80% power, 30% attrition allowance; 66 pairs analysed | same | **Verified** | "A total sample size of 160 participants (80 gardeners and 80 non gardeners) was previously evaluated to detect an increase of one portion of fruit and vegetables per day … with 80% power … and a planned attrition rate of 30%" |
| 3 | "At t1, half of gardeners (n = 32) had not retrieved any fruit or vegetables"; mean harvest 38.9 g/d (SD 44.1) | same | **Verified** | Verbatim |
| 4 | 75.8% university degree; education p = 0.049; BMI p = 0.046; sample "more concerned about their health than the general population"; "majority … held a university degree … (398 vs 264 g/d)" | same | **Verified** | Table 1: University 50 (75.8%) vs 59 (89.4%), p 0.049; BMI p 0.046; limitations paragraph verbatim |
| 5 | Authors concede "insufficient statistical power and inability of the data collection tools to detect change could explain the lack of results"; "low gardener involvement"; "multicomponent programs are more likely to modify health outcomes" | same | **Verified** | All three phrases located in the limitations and discussion |
| 6 | COM-B: "This system places **no priority** on an individual, group, or environmental perspective — intra-psychic and external factors all have equal status in controlling behaviour" | Michie, van Stralen & West 2011, PMC3096582 | **Verified** | Verbatim (source uses "--" for the dash) |
| 7 | Pharos: health literacy "niet alleen bepaald door wat iemand zelf kan, maar ook door de eisen die de omgeving stelt … ook als zij die vaardigheden in principe wel hebben" | Pharos infosheet, Oct 2026 | **Verified** | Verbatim |
| 8 | Pharos: Q12 "gebaseerd … op het conceptuele raamwerk en niet op basis van uitkomsten van de Q47"; "geen inhoudelijk equivalent van de Q47"; Q47 52.8% vs Q12 46.6% in one sample; Nivel 44.3% | same | **Verified** | Verbatim; but the same page gives **52,3%** for the Q47 and cites revised report 2026-0107. See 3.4. |
| 9 | "the earlier version 2026-0076, **whose headline figures are identical**" | note's own inference | **Not verified** | 0076 was not obtained by me or (in revised form) by the note; the factsheet's 52.3% makes "identical" doubtful. See 3.4. |
| 10 | Teach-back: 18 RCTs, n = 1985; self-efficacy SMD 2.40 (0.37–4.44), very low; adherence SMD 1.04 (0.45–1.64), low; "no clear pattern" on knowledge; large CIs, substantial heterogeneity | Vick et al. 2026, abstract | **Verified** | All figures and the "no clear pattern" wording verbatim |
| 11 | Groen Verbindt: 9 in 10 "nieuwe mensen leren kennen", 5 in 10 "sta eerder klaar", 4 in 10 "durf meer mensen om hulp te vragen", each year | Verwey-Jonker 2019 | **Verified** (PDF, local extraction) | All three statements verbatim; the wording is "Sinds het afgelopen jaar durf ik meer mensen om hulp te vragen" |
| 12 | Volunteer education: "ongeveer de helft … universitaire opleiding of … hoger beroepsonderwijs" against "ruim een derde" of the neighbourhood | same | **Verified** | Verbatim |

**Checks that failed or could not be completed:** the "indexation frozen" claim (15); the identity of the two RIVM report versions (9); and the internal inconsistency in the health note over the asking datum (3.1), which is a reasoning failure rather than a citation failure but is the most consequential item in this table.

---

## 7. What the revisions got right

Specific, because the PI needs to know which corrections landed and should not be undone:

**PR #28.**
1. **The money correction is correct, and it is the strongest single piece of work in either revision.** The regeling exists, the amounts are in the annexes exactly as quoted, the sum of regional + local + NPLV equals €9,601,453, and the city's own budget answer independently arrives at "ca. 9,6 miljoen" budget-neutral. v1's cliff was an artefact of comparing a year with a national envelope to a year without one, and the revision says so without over-correcting into "the money is fine": the 2026 cut, the July 2027 lapse, the four continuing ketenaanpakken and the 2029 evidence conditionality all survive as findings. **Verified twice from different documents.**
2. **The four strata are not decoration.** §2.1's explicit admission that the report "has almost nothing in S4" is the kind of statement that makes a report trustworthy, and §4.6's seven-row table of consequences with the reason for each is exactly what the issue asked for.
3. **P22 works.** "Eligibility restrictions and incumbent advantage are documented; demonstrated exclusion, refusal or intentional gatekeeping are not — insufficient evidence to adjudicate" is the right statement, and §4.4's explanation of why the distinction matters practically ("the first implies a design change; the second implies a conflict") is better than the instruction required.
4. **Centralisation is now a rival, not a tension.** §4.9 gives the centralising case its strongest form (the region's own diagnosis; the Canadian comparison; London versus Greater Manchester; the funding architecture already centralised; the Coöperatie dissolution as a local natural experiment), then gives the middle its strongest form, then says what would discriminate. The "five conditions" framing is over-claimed (4.2), but the *move* — replace "centre or middle" with "which conditions and who holds the money" — is a genuine analytical improvement over v1 and over the PI's framing.
5. **Psychological ownership and territoriality are genuinely open.** §4.10's seven hypotheses, each with a rival and an adjudication test, plus the four counter-findings (ownership predicts knowledge *sharing*; territoriality is trust-contingent; ownership adds nothing incremental to performance; identity preservation can *increase* ingroup bias) is a model of how to keep a mechanism open without smuggling it in. The last of those is the most uncomfortable finding in either report and the revision carries it.
6. **P40 is a real conclusion, not a hedge.** "You can have light accounts and local autonomy, or binding coordination and local discretion over resources, but the same body cannot credibly offer both" is falsifiable, useful and marked as inference.

**PR #26.**
1. **"Implausible" is withdrawn, and the reason is stated as a rule rather than an apology.** §2.1's three rules and §2.2's four states give the report an instrument for not repeating the error, and the JArDinS re-scoping is the demonstration: the full-text read (verified) shows a null about *entering* a garden, in a 75.8%-university cohort, at a dose where half harvested nothing — and the report now says precisely that.
2. **The constructs are separated without being ranked.** §3.1's table (functional/interactive/critical health literacy, food literacy, health-related learning, self-efficacy, situated capability, sustained behaviour change) with "what it cannot carry" for each is the section v1 lacked, and §3.2's refusal of the "consolation prize" reading is the right ethical and analytical call.
3. **Instrument versus assessment is correctly split.** §7's claim (i)/(ii) separation and the eight-method table — with teach-back's CIs and certainty stated at source, and think-aloud honestly recorded as "[U] no source retrieved" rather than described from memory — is exactly the correction the PI asked for.
4. **COM-B and SDT are labelled as theory, and the labelling holds under pressure.** §1.1 finding 9 ("**Both are theory, not evidence about gardens**"), P27/P28 ("Established as theory"), and §4.4's statement of what a test in Eindhoven would require all keep the distinction. The COM-B "no priority" quotation is verified verbatim and is used to defeat v1's inference correctly.
5. **Fontys and DE STAP are treated as complementary in subject, not in practice,** with no assumption of willingness and no partnership proposed — P33's finding that no public Fontys project joins the health-literacy theme to the green-environment theme is a real, checkable negative, and §8.3's "what is not established" list is appropriately blunt.
6. **The intrinsic value of participation is preserved as a boundary rather than a verdict** — §1.3C and §12 — which satisfies the PI's instruction without turning the garden into a behavioural intervention.

---

## 8. Residual risks and what a next reader should not rely on

1. **Do not cite PR #26's "Contradicts" row on interactive health literacy, or its §5.3 falsifier sentence, without reading §3.1 of this review.** As written they say opposite things about the same datum; the underlying source is a cross-sectional change item and cannot bear either reading.
2. **Do not cite PR #26's "but not knowledge" or its "no mechanism: reading is not what happens there".** Neither is what the source says; §3.2 and §3.3 give replacements.
3. **Do not cite PR #28's "five conditions that predict documented outcomes under either form" as a finding.** No study tests the set; it is the report's synthesis, and it is the load-bearing inference of the revision. §4.2 gives a wording that keeps the insight without the claim.
4. **Do not use P12b's "like-for-like" in a budget argument.** The totals are right; the comparison is total-on-total between instruments of different scope, and equality at the total can hide per-theme losses that nobody has quantified.
5. **Almost all of PR #28 §4.7–4.10 and PR #26 §8 remain child-reported at abstract level,** with the exceptions recorded in §6. The Lubell and Wiktorowicz checks improve confidence in the two pivotal items but do not upgrade the rest. A reader who treats the mechanism tables as verified literature would be over-reading both notes.
6. **The "Dutch search found nothing" claims (P25, P34, §15) rest on a search with no hit counts** (OpenAlex 429, no counts from the web engine). The notes say so; a downstream synthesis should not convert "not found in six recorded query sets" into "the Dutch field has not studied this".
7. **PR #28's "temporariness survives" depends on a document that did not exist at retrieval** — the regional werkagenda, due 8 December 2026. Both the coordination-ownership question and the local destination of €5,968,460 turn on it. Until it is public, §4.3(d) and §9 item 1 are the most likely sentences in either report to be overtaken.
8. **A reviewer of the next revision should check three things first:** whether the §4.9 Wiktorowicz gloss and the five-conditions framing were changed; whether §4.1's "none of them" was restored to "two of seven as arrangements"; and whether PR #26 resolved the asking datum one way or the other. If those three are unchanged, the reports are still worth reading but should not be cited for those claims.

**What I would ask the PI to decide before accepting either report:**
- For PR #26: whether the report may say, in one sentence, what the balance of evidence *suggests* about the mechanism (weakly positive for interactive capability, unstudied for health literacy as an outcome), or whether "Insufficient" must stand without a leaning. The revision currently does the latter in the table and the former in the prose, and the inconsistency is visible.
- For PR #28: whether the "five conditions" framing is acceptable as an explicitly-labelled synthesis. If it is, P39 and §4.9 need only the [I] marker; if it is not, the section's conclusion needs rewriting, because it currently rests on that synthesis.
- For both: whether the child-reported literature may continue to carry sections this large. The PI's own standard — "a more trustworthy account of what we know, what we do not know, and what remains worth discovering" — is met by the documentary layers and only partly by the literature layers, and no amount of caution in the prose fixes a literature read at abstract level by a delegated line.
