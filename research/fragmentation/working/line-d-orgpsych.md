# Line D — The human, group and organisational mechanisms: psychological ownership, territoriality, autonomy, identity and status

**Author:** research subagent (Line D)
**Date of retrieval:** 26 November 2026
**Branch:** `research/27-health-fragmentation`
**Scope:** international peer-reviewed organisational and social psychology, 1989–2026, English. One Dutch doctoral dissertation (Nijs 2022) is included and is labelled as a dissertation. **No claim about Eindhoven, De Kempen, any Dutch health organisation, or any named actor.** No motive is attributed to any real organisation or person anywhere in this file.
**Working file only.** Not for commit by this agent.

**Marking convention**
- **[D]** documented in a retrieved source (verbatim or near-verbatim, with locator)
- **[C]** claimed by one actor (in this line: claimed by a single author/paper and not replicated)
- **[I]** inference drawn by this agent
- **[U]** not established in the sources searched
- **†** marks a quotation reconstructed from OpenAlex's `abstract_inverted_index` (a word→position index) rather than from a publisher-rendered abstract. The wording is deterministic and was checked position by position, but punctuation and hyphenation are the agent's reconstruction, not the publisher's. Do not treat † quotations as bibliographic verbatim.
- **Read depth** per source: `full text` (complete document read/extracted) · `abstract (verbatim)` (publisher-deposited abstract retrieved in full) · `abstract (reconstructed)†` · `metadata only` (no abstract obtainable — no claim made).

---

## 0. What this line changes relative to Line C

Six items, stated first because the parent report may already cite them.

1. **Zhang et al. is 2021, not 2020, and k = 141 is confirmed.** The paper is *Journal of Management* **47(3): 745–770** (print March 2021; first published online 2020), DOI 10.1177/0149206320917195. The abstract confirms "Across 141 studies published over 20 years" and adds a second figure Line C did not report: **294 studies** enter the structural model (291 primary studies and three published meta-analyses) **[D]**. Cite as Zhang et al. 2021.
2. **Avey, Avolio, Crossley & Luthans (2009) does not, at abstract level, test stewardship or extra-role behaviour.** Its abstract reports a confirmatory factor analysis of an expanded ownership measure (four dimensions: self-efficacy, accountability, belongingness, self-identity) and treats **territoriality as a separate, "prevention-focused" form of ownership** **[D]**. The "ownership → stewardship/extra-role effort" claim therefore rests on Van Dyne & Pierce (2004), which *does* test organisational citizenship behaviour — and which finds ownership adds **no** incremental prediction of performance (see §5, C3). The source list in the commissioning brief describes Avey et al. as being "on ownership and stewardship/extra-role behaviour"; that description should not be carried forward as an effect finding.
3. **Founder identity is no longer [U].** Fauchart & Gruber (2011) and Powell & Baker (2014) were recovered at **abstract level** — Crossref has no abstract for Academy of Management journals, but OpenAlex holds the deposited abstracts, which Line C's Semantic Scholar route had reported as "elided by the publisher". Both are quoted in §2.2. Read depth is still abstract only; neither full text was obtained (EPFL repository returned HTTP 429).
4. **Nooteboom et al. (2021) is upgraded from abstract only to full text** (Europe PMC, PMC7803720, CC BY). The "professional identity" theme Line C could only name is now documented with its sub-themes and study counts (§2.2 E20).
5. **A retrieval-channel correction worth carrying into the note:** for management journals, Crossref does **not** carry abstracts from the Academy of Management, and OpenAlex's search endpoint was HTTP 429 throughout this session — but OpenAlex's **by-DOI** endpoint returns deposited abstracts and OA locations, and Crossref's `query.bibliographic` endpoint returns abstracts where the publisher deposits them. That combination is what recovered items 3 and 4.

6. **Four phrasings in the parent note's hypothesis table (`note.md` §4.10, which attributes them to "line D") are stronger than the evidence this line retrieved.** Flagged here rather than edited there, because another agent owns that file.
   - **H1, "produces both stewardship and territorial behaviour."** The meta-analysis documents "territorial behaviors" as a dark-side *outcome category* **[D, D07]**; "stewardship" appears as a dissertation keyword **[D, D10]** and as a theoretical positive consequence **[D, D02]**, and **no retrieved study measures stewardship as a distinct behaviour**. Ownership's best-evidenced behavioural outcome is organisational citizenship behaviour, rated by peers and supervisors — and D03 found **no** incremental prediction of performance. Suggested wording: "is associated with citizenship behaviour, and with territorial behaviour on self- and coworker-report".
   - **H2, "the 'dark side' is real but contested in inter-organisational transfer."** Correct, and this line would put it more strongly: there is **no** inter-organisational measurement at all, so "contested in transfer" understates the gap.
   - **H4, "identity threat in mergers *and collaborations* is documented."** Every retrieved study is a **merger** — involuntary or semi-voluntary consolidation of employment. No retrieved study documents identity threat in a voluntary collaboration between autonomous organisations. Suggested wording: "documented in mergers; not established for voluntary collaboration".
   - **H5, "recognition is a condition, not a motivator, in the network literature."** This line did not retrieve that finding. What it retrieved is that legitimacy, reputation and status are **distinct forms of social judgment addressing different questions** (conceptual) **[D, D23]** and that status conflict undermines information sharing in small groups **[D, D24]**. H5 should cite Line C for the network claim or be marked **[U]** on this line's evidence.
   - **H3 could be strengthened rather than weakened.** The note says autonomy is "a basic psychological need at individual level and a role requirement in professional settings". There is also a genuine **organisational-level** autonomy literature: six dimensions, legal status a poor proxy, and "tensions between different levels of autonomy appear in practice" **[D, D16]**. That gives H3 a measurement frame the note currently lacks.

---

## 1. Scope and brief

**The question this line serves.** Why does health promotion fragment across organisations in Eindhoven–De Kempen, and under what conditions can autonomous initiatives contribute to shared outcomes without surrendering local identity?

**This line's job.** To make the *human, group and organisational* mechanism families empirically strong rather than gestural, across four families: (1) psychological ownership; (2) territoriality; (3) autonomy and self-determination at organisational and inter-organisational level; (4) identity, recognition and status. For each: at least one rival explanation that would produce the same observable behaviour without the proposed mechanism; counter-evidence sought deliberately; and explicit level discipline.

**What was done.** 36 sources retrieved: 2 at full text, 22 at verbatim-abstract level, 12 at reconstructed-abstract level; one further source (Brown 2009) reached metadata only and was excluded from the table, with no claim made from it. Every source was located through a DOI-verified bibliographic match, and every claim below names the retrieved source and its level of analysis. Retrieval channels: Crossref REST, OpenAlex by-DOI, Europe PMC REST (including full-text XML for CC BY articles), publisher sites where accessible, and two direct OA PDF retrievals (Ecology & Society; Utrecht repository landing page).

**What was not done.** No local fieldwork, no interviews, no survey, no measurement in Eindhoven–De Kempen. No Dutch-language literature search. No grey literature beyond one doctoral dissertation. No source was bypassed: two Cloudflare challenges, one repository rate-limit and one oversized PDF are recorded in §7 and nothing was obtained through them.

**Structural warning, stated before the findings.** This literature is **almost entirely individual-level**. Psychological ownership has a validated individual measure and a meta-analysis; it has no validated organisational or inter-organisational measure. Territoriality has one conceptual paper and one empirical field study from the same research group, both about employees and their colleagues. Autonomy has a genuine organisational-level literature (public-administration autonomy), but its central finding is that autonomy is multidimensional and that legal status is a bad proxy — not that autonomy causes fragmentation. Identity and status have strong individual and small-group evidence from *merger* research, which is the closest empirical analogue to consolidation that exists. **Any sentence of the form "organisation X resists sharing because it feels ownership / is territorial / faces identity threat" is, on this evidence base, an analogy, not a measurement.** §3.5 states which findings survive that test; they are fewer than the literature's confidence suggests.

---

## 2. Source table

Level codes: **L1** individual · **L2** group/team · **L3** organisation · **L4** inter-organisational/field/network · **L5** system/institution. Transfer to the L4 question: **direct** · **analogical** · **unwarranted**.

| ID | Citation | DOI / PMID | Design | Sample / setting | Level | Read depth | Principal finding |
|---|---|---|---|---|---|---|---|
| D01 | Pierce, Kostova & Dirks 2001, "Toward a Theory of Psychological Ownership in Organizations", *Academy of Management Review* 26:298ff | 10.2307/259124 | Conceptual theory paper | — | L1 (theory) | abstract (reconstructed)† | Defines psychological ownership; identifies its "roots" and primary "routes"; proposes outcomes; distinguishes it from related constructs |
| D02 | Pierce, Kostova & Dirks 2003, "The State of Psychological Ownership", *Review of General Psychology* 7:84–107 | 10.1037/1089-2680.7.1.84 | Conceptual | — | L1 (theory) | abstract (verbatim) | Three motives — efficacy/effectance, self-identity, "having a place to dwell"; experiences that give rise to ownership; "several positive and negative consequences" |
| D03 | Van Dyne & Pierce 2004, "Psychological ownership and feelings of possession: three field studies…", *Journal of Organizational Behavior* 25:439–459 | 10.1002/job.249 | Three field studies; manager and peer ratings | >800 employees (three field samples) | L1 | abstract (verbatim) | Ownership predicts commitment, satisfaction, organisation-based self-esteem, performance and OCB; adds incremental variance for OBSE and OCB over satisfaction/commitment; **fails to add incremental value for performance** |
| D04 | Avey, Avolio, Crossley & Luthans 2009, "Psychological ownership: theoretical extensions, measurement…", *Journal of Organizational Behavior* 30:173–191 | 10.1002/job.583 | CFA of an expanded measure | Employed adults (n not in abstract) | L1 | abstract (verbatim) | Four "promotion-focused" dimensions (self-efficacy, accountability, belongingness, self-identity); territoriality as a distinct "prevention-focused" form |
| D05 | Pierce & Jussila 2010, "Collective psychological ownership within the work and organizational context", *Journal of Organizational Behavior* 31:810–834 (online 2009) | 10.1002/job.628 | Conceptual construct introduction | — | L2 (theory) | abstract (verbatim) | Collective ownership as "a single and shared mind-set"; discusses genesis, motives, "what can and cannot be owned", and attitudinal/motivational/behavioural/stress outcomes |
| D06 | Dawkins, Tian, Newman & Martin 2017, "Psychological ownership: A review and research agenda", *Journal of Organizational Behavior* 38:163–183 | 10.1002/job.2057 | Narrative review | Field-wide | L1 | abstract (verbatim) | Construct, measurement and nomological network still debated; calls for "examination of possible multilevel applications of PO research" and "identification of potential boundary conditions" |
| D07 | Zhang, Liu, Zhang, Xu & Cheung 2021, "Psychological Ownership: A Meta-Analysis and Comparison of Multiple Forms of Attachment in the Workplace", *Journal of Management* 47(3):745–770 | 10.1177/0149206320917195 | Meta-analysis + two-stage MASEM + dominance analysis | k = 141 studies over 20 years; 294 studies (291 primary + 3 meta-analyses) in the structural model | L1 | abstract (verbatim) | Antecedents: control, knowing, investment **plus "safety" (justice, trust, POS, relational closeness)**; outcomes include "dark-side outcomes (e.g., territorial behaviors)"; PO has incremental validity over commitment and identification for in-role performance and OCB |
| D08 | Brown, Lawrence & Robinson 2005, "Territoriality in Organizations", *Academy of Management Review* 30:577–594 | 10.5465/amr.2005.17293710 | Conceptual | — | L1/L3 (theory) | abstract (reconstructed)† | Territories include physical spaces, ideas, roles, relationships; territorial behaviours "construct, communicate, maintain, and restore" territories; consequences include commitment, conflict, preoccupation, individual isolation |
| D09 | Brown, Crossley & Robinson 2014, "Psychological Ownership, Territorial Behavior, and Being Perceived as a Team Contributor", *Personnel Psychology* 67:463–485 | 10.1111/peps.12048 | Field study; focal employee + coworker ratings | Working adults and one coworker each (n not in abstract) | L1/L2 | abstract (verbatim) | Ownership → claiming and anticipatory defending **depending on trust**; a high-trust environment **reduces** territorial behaviour, but when it occurs there, coworkers rate the person's contribution significantly **lower** — a "double-edged sword" |
| D10 | Nijs 2022, *This place is ours: Collective psychological ownership and its social consequences*, doctoral dissertation, Utrecht University | 10.33540/1092 | Dissertation: large-scale surveys + experiments | Dutch and British respondents; territories = country, neighbourhood, neighbourhood park, hangout place | L2 | abstract (verbatim, repository) | Collective ownership has "two faces": an exclusive right to determine → exclusion of outsiders; a responsibility to care → prosocial investment ("stewardship behavior") |
| D11 | Nnadozie 2026, "Mine to share: psychological ownership and resilience in medical knowledge sharing", *The Learning Organization* (online) | 10.1108/tlo-09-2025-0221 | Cross-sectional survey, convenience sample | 342 medical doctors, Nigeria | L1 | abstract (verbatim) | Ownership **positively** predicted both knowledge donating and knowledge collecting; resilience attenuated only the ownership→collecting path |
| D12 | Gagné & Deci 2005, "Self-determination theory and work motivation", *Journal of Organizational Behavior* 26:331–362 | 10.1002/job.322 | Conceptual/theory | — | L1→L3 (theory) | abstract (verbatim) | Differentiating extrinsic motivation by degree of autonomy makes SDT applicable to work settings; SDT presented as a theory of work motivation and organisational behaviour |
| D13 | Deci, Olafsen & Ryan 2017, "Self-Determination Theory in Work Organizations: The State of a Science", *Annual Review of Organizational Psychology and Organizational Behavior* 4:19–43 | 10.1146/annurev-orgpsych-032516-113108 | Review | — | L1→L3 | abstract (verbatim) | Autonomous vs controlled motivation; competence, autonomy, relatedness needs; "policies, practices, and environments that promote both wellness and high-quality performance" |
| D14 | Van den Broeck, Ferris, Chang & Rosen 2016, "A Review of Self-Determination Theory's Basic Psychological Needs at Work", *Journal of Management* 42:1195–1229 | 10.1177/0149206316632058 | Meta-analytic review | 99 studies, 119 distinct samples | L1 | abstract (verbatim) | Tests SDT's requirement that each need **uniquely** predicts growth, internalisation and well-being; tests whether an overall need-satisfaction score is appropriate; tests scale effects |
| D15 | Ng et al. 2012, "Self-Determination Theory Applied to Health Contexts: A Meta-Analysis", *Perspectives on Psychological Science* 7:325–340 | 10.1177/1745691612447309 | Meta-analysis + path analysis | 184 independent data sets; health care and health-promotion studies | L1 (patient) | abstract (verbatim) | Practitioner autonomy support → need satisfaction → autonomous motivation → better mental and physical health outcomes |
| D16 | Verhoest, Peters, Bouckaert & Verschuere 2004, "The study of organisational autonomy: a conceptual review", *Public Administration and Development* 24:101–118 | 10.1002/pad.316 | Conceptual review + survey | Survey of Flemish public organisations | **L3** | abstract (verbatim) | Six dimensions of organisational autonomy; existing research uses "a diverse and a too restrictive conceptualisation"; formal–legal status is a poor autonomy indicator given heterogeneity; "tensions between different levels of autonomy appear in practice" |
| D17 | Saz-Carranza & Ospina 2011, "The Behavioral Dimension of Governing Interorganizational Goal-Directed Networks — Managing the Unity-Diversity Tension", *Journal of Public Administration Research and Theory* 21:327–365 | 10.1093/jopart/muq050 | Comparative case studies | Four immigrant-serving networks, USA | **L4** | abstract (reconstructed)† | Unity and diversity are both essential to network performance yet "each makes contradictory demands which require attention"; three mechanisms of network-level managerial work |
| D18 | Ashforth & Mael 1989, "Social Identity Theory and the Organization", *Academy of Management Review* 14 | 10.5465/amr.1989.4278999 | Conceptual | — | L1 (theory) | abstract (reconstructed)† | Social identification as "a perception of oneness with a group of persons"; sources include distinctiveness and prestige; consequences include identity-congruent activity and support for institutions embodying the identity; applied to role conflict and intergroup relations |
| D19 | Terry, Carey & Callan 2001, "Employee Adjustment to an Organizational Merger: An Intergroup Perspective", *Personality and Social Psychology Bulletin* 27:267–280 | 10.1177/0146167201273001 | Survey, social-identity model | 465 fleet staff, newly merged airline | L1 (in a merger) | abstract (verbatim) | Negative effects "most marked for employees of the low-status premerger organization"; perceived **permeability** of intergroup boundaries helped low-status members' identification and outcomes but **hurt** high-status members' person-related outcomes; mediated by identification |
| D20 | van Dick, Ullrich & Tissington 2006, "Working Under a Black Cloud: How to Sustain Organizational Identification after a Merger", *British Journal of Management* 17 | 10.1111/j.1467-8551.2006.00479.x | Argument + merger study | One merger (sample not in abstract) | L1 (in a merger) | abstract (verbatim) | Argues against "merger folklore" that job insecurity is the main mechanism; post-merger identification has effects **above and beyond** job insecurity; recommends continuity and specific communication |
| D21 | van Leeuwen, van Knippenberg & Ellemers 2003, "Continuing and Changing Group Identities", *Personality and Social Psychology Bulletin* 29:679–690 | 10.1177/0146167203029006001 | Two experiments, minimal group paradigm | Laboratory samples (composition not stated in abstract) | L2 | abstract (verbatim) | Perceived **continuation** of pre-merger identity strengthened the link between pre-merger and superordinate identification — **and strengthened, rather than reduced, ingroup bias at the subordinate level** |
| D22 | Petriglieri 2011, "Under Threat: Responses to and the Consequences of Threats to Individuals' Identities", *Academy of Management Review* 36:641–662 | 10.5465/amr.2011.65554645 | Conceptual | — | L1 (theory) | abstract (reconstructed)† | Identity threat defined as "an experience appraised as indicating potential harm to the value, meanings, or enactment of an identity"; model of responses by source of threat; individual and organisational consequences |
| D23 | Bitektine 2011, "Toward a Theory of Social Judgments of Organizations: The Case of Legitimacy, Reputation, and Status", *Academy of Management Review* 36:151–179 | 10.5465/amr.2009.0382 | Conceptual | — | L3→L4 (theory) | abstract (reconstructed)† | Legitimacy, reputation and status are distinct **forms of social judgment**, "each addressing a different question about the organization"; evaluator perspective under bounded rationality |
| D24 | Bendersky & Hays 2012, "Status Conflict in Groups", *Organization Science* 23 | 10.1287/orsc.1110.0734 | Mixed methods: qualitative identification, 4-item scale validation, performance analysis | Task groups (sample not stated in abstract) | L2 | abstract (reconstructed)† | Status conflict = disputes over relative respect positions; significant negative main effect; moderates task-conflict effects; "hurts performance by undermining information sharing more than other types of conflict do" |
| D25 | Fauchart & Gruber 2011, "Darwinians, Communitarians, and Missionaries: The Role of Founder Identity in Entrepreneurship", *Academy of Management Journal* 54:935–957 | 10.5465/amj.2009.0211 | Qualitative, inductive | 49 firm founders, sports-related equipment industry | L1→L3 | abstract (reconstructed)† | Three "pure types" of founder identity that "systematically shape key decisions in the creation of new firms", "imprinting" start-ups with founders' self-concepts |
| D26 | Powell & Baker 2014, "It's What You Make of It: Founder Identity and Enacting Strategic Responses to Adversity", *Academy of Management Journal* 57:1406–1433 | 10.5465/amj.2012.0454 | Longitudinal field study, grounded theory | 13 resource-constrained founder-run textile and apparel firms | L1→L3 | abstract (reconstructed)† | Founders "enact distinctly different definitions" of the same adversity and "use their firms as vehicles to defend who they are or become who they want to be" |
| D27 | Liberati, Gorli & Scaratti 2016, "Invisible walls within multidisciplinary teams: Disciplinary boundaries and their effects on integrated care", *Social Science & Medicine* 150:31–39 | 10.1016/j.socscimed.2015.12.002; PMID 26730879 | Ethnography | Sub-intensive stroke unit, Italian public hospital; 180 h observation; 42 health-care providers | L2 (professions in a team) | abstract (verbatim, Europe PMC) | Disciplinary boundaries hinder both intra- and inter-professional collaboration; doctors and nurses construct discipline-specific identities; conflicts "over the regulation of the medical-nursing boundary" |
| D28 | Nooteboom, Mulder, Kuiper, Colins & Vermeiren 2021, "Towards Integrated Youth Care: A Systematic Review of Facilitators and Barriers for Professionals", *Administration and Policy in Mental Health* 48:88–105 | 10.1007/s10488-020-01049-8; PMID 32424453; PMC7803720 | Systematic review (PROSPERO CRD42018084527) | 55 studies, youth care, multiple countries | L2/L3 (professionals) | **full text (CC BY)** | Seven themes; Theme 7 "Professional identity" has four sub-themes with study counts: roles and responsibilities (27), attitudes (16), shared thinking (22), trust/respect/equity (20) |
| D29 | Chun 2005, "Goal Ambiguity and Organizational Performance in U.S. Federal Agencies", *Journal of Public Administration Research and Theory* 15:529–557 | 10.1093/jopart/mui030 | Measure development + regression | U.S. federal agencies; 2000 National Partnership for Reinventing Government employee survey | L3 | abstract (reconstructed)† | Four dimensions of goal ambiguity (mission comprehension, directive, evaluative, priority); three related to age, financial publicness and regulatory status; ambiguity dimensions negatively related to performance indicators (managerial effectiveness, customer service orientation, productivity, work quality) |
| D30 | Froelich 1999, "Diversification of Revenue Strategies: Evolving Resource Dependence in Nonprofit Organizations", *Nonprofit and Voluntary Sector Quarterly* 28:246–268 | 10.1177/0899764099283002 | Structured literature review with comparative profiles | Nonprofit sector, international literature | L3 | abstract (verbatim) | Each revenue source (private contributions, government funding, commercial activity) has distinct profiles of **revenue volatility, goal displacement, and process/structure effects**; diversification raises unanswered performance and legitimacy questions |
| D31 | Ashworth, Boyne & Delbridge 2009, "Escape from the Iron Cage? Organizational Change and Isomorphic Pressures in the Public Sector", *Journal of Public Administration Research and Theory* 19:165–187 | 10.1093/jopart/mum038 | Longitudinal survey analysis | 101 English public organisations, 2001–2004 | **L4 (field)** | abstract (reconstructed)† | Distinguishes **compliance** from **convergence**; "substantial evidence of compliance but more limited support for convergence"; impacts stronger for strategies and culture than structures and processes |
| D32 | Ansell & Gash 2008, "Collaborative Governance in Theory and Practice", *Journal of Public Administration Research and Theory* 18:543–571 | 10.1093/jopart/mum032 | "Meta-analytical" case review → contingency model | 137 cases of collaborative governance, multiple sectors | L4 | abstract (verbatim) | Starting conditions (prior conflict, incentives, power/resource asymmetries) and process factors (face-to-face dialogue, trust building, commitment, shared understanding); "virtuous cycle" develops from **small wins** |
| D33 | Vangen & Huxham 2003, "Nurturing Collaborative Relations: Dealing with Distrust in Interorganizational Collaboration", *Journal of Applied Behavioral Science* 39:5–31 | 10.1177/0021886303039001001 | Synthesis of trust research + collaboration research | Cross-sector partnerships (UK action-research tradition) | L4 | abstract (verbatim) | "the likelihood of disappointing outputs is high"; a trust-building loop; trust management means both coping where trust is lacking and building it where possible |
| D34 | Devine-Wright 2009, "Rethinking NIMBYism: The role of place attachment and place identity in explaining place-protective action", *Journal of Community & Applied Social Psychology* 19:426–441 | 10.1002/casp.1004 | Review + framework proposal | Local opposition to energy developments, European policy context | L2/L4 | abstract (verbatim) | Local opposition reconceived as **place-protective action** arising when developments "disrupt pre-existing emotional attachments and threaten place-related identity processes"; five-stage framework across levels |
| D35 | Cox, Arnold & Villamayor-Tomás 2010, "A Review of Design Principles for Community-based Natural Resource Management", *Ecology and Society* 15(4):38 | 10.5751/ES-03704-150438 | Systematic review of principle evaluations + Fisher's exact tests and effect sizes | 91 studies of common-pool resource institutions | L4/L5 | **full text (PDF)** | Principles "well supported empirically" (mean 3.73 of 5, n = 91). **Principle 7 "minimal recognition of rights to organize": 28 of 31 successful vs 13 of 20 unsuccessful cases, Fisher p = 0.032, effect 2.2** |
| D36 | Ancona & Caldwell 1992, "Bridging the Boundary: External Activity and Performance in Organizational Teams", *Administrative Science Quarterly* 37:634ff | 10.2307/2393475 | Interviews + log data + questionnaires | 38 new-product team managers; log data from 2 teams; 45 questionnaire respondents; US high-tech firms | L2 | abstract (reconstructed)† | Teams develop **distinct external strategies** towards their environment; "type of [external activity], not just [the] amount, determines performance"; positive cycles over time |

**Metadata verification note.** Titles, journals, years, volumes and pages above were read from Crossref or OpenAlex records, except where the record displayed only a title (D01, D08, D18, D22, D23, D24, D25, D26, D29, D31, D36 — DOI and journal verified, pages as cited in the commissioning brief or the publisher's canonical pagination). Author strings: for D04, D06, D07, D10, D11, D12, D17, D27, D28, D29, D31, D33, D35 the full author list was displayed in a retrieved record. For the remainder the author string is the canonical one supplied in the commissioning brief or the standard citation; **it was not re-verified against the publisher record in this session** and should be checked at citation time. D29 is deposited in both Crossref and OpenAlex with a **single** author ("Y. H. Chun"); it is conventionally cited as Chun & Rainey — this agent could not confirm the second author from any retrieved record and flags the discrepancy rather than resolving it.

---

### 2.2 Verbatim excerpts with locators

All retrieved 26 November 2026. † = reconstructed from the OpenAlex abstract index.

**E1 — Pierce, Kostova & Dirks 2001 (abstract†).**
> "Building upon the observation that individuals feel ownership toward a variety of targets, we suggest that, under certain conditions, organizational members can develop feelings of ownership [toward the] organization and various factors. We define psychological ownership, identify its 'roots' and primary 'routes' through which it develops, and propose outcomes."

**E2 — Pierce, Kostova & Dirks 2003 (abstract, verbatim).**
> "They propose that this state finds its roots in a set of intraindividual motives (efficacy and effectance, self-identity, and having a place to dwell)."

**E3 — Van Dyne & Pierce 2004 (abstract, verbatim).**
> "…results, however, fail to show an incremental value of psychological ownership in predicting employee performance."

**E4 — Avey, Avolio, Crossley & Luthans 2009 (abstract, verbatim).**
> "In addition, territoriality was examined as a unique and more 'prevention-focused' form of ownership."

**E5 — Pierce & Jussila 2010 (abstract, verbatim).**
> "Reflecting the psychology of 'us' and 'ours,' collective psychological ownership emerges through interactive dynamics whereby individuals come to a single and shared mind-set as it relates to a sense of ownership for a particular object."

**E6 — Dawkins, Tian, Newman & Martin 2017 (abstract, verbatim).**
> "In addition, we call for greater investigation of PO towards different objects or foci; examination of possible multilevel applications of PO research; identification of potential boundary conditions of PO…"

**E7 — Zhang, Liu, Zhang, Xu & Cheung 2021 (abstract, verbatim).**
> "Across 141 studies published over 20 years, our meta-analysis shows that apart from the factors related to the three traditional categories of PO antecedents (i.e., control, knowing, and investment), safety (e.g., organizational justice, trust, perceived organizational support, and relational closeness) is an emerging antecedent leading to PO. In addition, we find that PO is related not only to employees' attitudinal and performance outcomes but also to some dark-side outcomes (e.g., territorial behaviors)."

**E8 — Zhang et al. 2021 (abstract, verbatim).**
> "…the results reveal that PO has an incremental validity above that of organizational commitment and organizational identification in predicting employees' in-role performance and organizational citizenship behaviors."

**E9 — Brown, Lawrence & Robinson 2005 (abstract†).**
> "Territorial feelings and behaviors are important, pervasive, yet largely overlooked aspects of organizational life. Organizational members can and do become territorial over physical spaces, ideas, roles, relationships, [and] other potential possessions in organizations. We examine how territorial behaviors are used to construct, communicate, maintain, and restore territories, then go on to discuss the consequences of these behaviors, including their effects on commitment, conflict, preoccupation, [and] individual isolation."

**E10 — Brown, Crossley & Robinson 2014 (abstract, verbatim).**
> "Findings suggest that a work environment of trust is a 'double-edged sword': On the one hand, a high trust environment reduces the territorial behavior associated with psychological ownership; on the other hand, when territorial behavior does occur in high trust environments, coworkers rate the territorial employee's contributions to the team significantly lower."

**E11 — Nijs 2022 (dissertation abstract, Utrecht repository).**
> "He concludes that collective psychological ownership has two faces. On the one hand, as ownership is accompanied by an exclusive right to determine what happens with what is owned, collective psychological ownership can lead to the exclusion of outsiders (such as immigrants). On the other hand, as ownership also comes with a responsibility to take care of what is owned, collective psychological ownership can lead to prosocial behaviour to invest into the territory."

**E12 — Nnadozie 2026 (abstract, verbatim).**
> "The results revealed that psychological ownership positively predicted both knowledge donating and knowledge collecting."

**E13 — Deci, Olafsen & Ryan 2017 (abstract, verbatim).**
> "…the postulate that all employees have three basic psychological needs—for competence, autonomy, and relatedness—the satisfaction of which promotes autonomous motivation, high-quality performance, and wellness."

**E14 — Van den Broeck, Ferris, Chang & Rosen 2016 (abstract, verbatim).**
> "…to test SDT's requirement that each basic psychological need should uniquely predict psychological growth, internalization, and well-being; to test whether use of an overall need satisfaction measure is appropriate… we conducted a meta-analytic review of 99 studies with 119 distinct samples…"

**E15 — Verhoest, Peters, Bouckaert & Verschuere 2004 (abstract, verbatim).**
> "The empirical material points at the dangers of using formal–legal status of a public organisation as an indicator of its autonomy, given substantial heterogeneity of organisations with the same formal–legal status on each dimension of autonomy. Moreover, tensions between different levels of autonomy appear in practice…"

**E16 — Saz-Carranza & Ospina 2011 (abstract†).**
> "…although unity and diversity are essential [to] network performance, each makes contradictory demands which require attention."

**E17 — Ashforth & Mael 1989 (abstract†).**
> "It is argued that (a) social identification is a perception of oneness with a group of persons…"

**E18 — Terry, Carey & Callan 2001 (abstract, verbatim).**
> "As predicted from social identity theory, the negative effects of the merger were most marked for employees of the low-status premerger organization. Also, as predicted, the perception of permeable intergroup boundaries in the new organization was associated positively with identification with the new organization and both job-related and person-related outcomes among employees of the low-status premerger organization but negatively with person-related outcomes among employees of the high-status premerger organization."

**E19 — van Leeuwen, van Knippenberg & Ellemers 2003 (abstract, verbatim).**
> "Moreover, perceived continuation strengthened, rather than reduced, ingroup bias at the subordinate level of the merged groups."

**E20 — Nooteboom et al. 2021, Theme 7 (full text, PMC7803720).**
> "Facilitators and barriers of the theme 'Professional identity' were described in four subthemes: professional roles and responsibilities (27 studies), attitudes (16 studies), shared thinking (22 studies), and trust, respect and equity (20 studies)."

**E21 — Nooteboom et al. 2021, Discussion (full text).**
> "It is often difficult for professionals to define clear roles in interprofessional collaboration and to share responsibility over a care process… studies reported that roles and responsibilities must be flexible when responding to the changing needs of families."

**E22 — Liberati, Gorli & Scaratti 2016 (abstract, verbatim, Europe PMC).**
> "Findings show that disciplinary boundaries hinder both intra-professional and inter-professional collaboration… conflicts emerge between doctors and nurses from different disciplines over the regulation of the medical-nursing boundary."

**E23 — Bitektine 2011 (abstract†).**
> "The proposed theory extends research on cognitive and sociopolitical legitimacy, reputation, and status by advancing an evaluator's perspective on these concepts as forms of social judgment, each addressing a different question about the organization."

**E24 — Petriglieri 2011 (abstract†).**
> "I review and reconceptualize identity threat, defining it as an experience appraised as indicating potential harm to the value, meanings, or enactment of an identity."

**E25 — Bendersky & Hays 2012 (abstract†).**
> "We introduce status conflicts—defined as disputes over people's relative (i.e., respect) positions in their group's social hierarchy—as a key group process that affects task performance… [status conflict] hurts performance by undermining information sharing more than other types of conflict do."

**E26 — Fauchart & Gruber 2011 (abstract†).**
> "Our analysis suggests the existence of three pure types of founder identities and shows how these systematically shape key decisions in the creation of new firms, thereby 'imprinting' start-ups with founders' distinct self-concepts."

**E27 — Powell & Baker 2014 (abstract†).**
> "We discovered that founders enact distinctly different definitions of the adversity and use their firms as vehicles to defend who they are or become who they want to be."

**E28 — Froelich 1999 (abstract, verbatim).**
> "A wide-ranging literature review is condensed into summary profiles comparing revenue volatility, goal displacement, process, and structure effects of each strategy."

**E29 — Ashworth, Boyne & Delbridge 2009 (abstract†).**
> "We find substantial evidence [of] compliance but more limited support for convergence. Furthermore, the impact of isomorphic pressures was stronger for strategies and culture than [for] structures and processes."

**E30 — Ansell & Gash 2008 (abstract, verbatim).**
> "We found that a virtuous cycle of collaboration tends to develop when collaborative forums focus on 'small wins' that deepen trust, commitment, and shared understanding."

**E31 — Vangen & Huxham 2003 (abstract, verbatim).**
> "Such collaborations, however, are difficult to manage, and the likelihood of disappointing outputs is high."

**E32 — Devine-Wright 2009 (abstract, verbatim).**
> "Local opposition is conceived as a form of place-protective action, which arises when new developments disrupt pre-existing emotional attachments and threaten place-related identity processes."

**E33 — Cox, Arnold & Villamayor-Tomás 2010, Table 3 (full text).**
> "7. Minimal recognition of rights to organize: The rights of appropriators to devise their own institutions are not challenged by external governmental authorities." — Success 28 / Failure 13; 51 cases; Fisher's exact p = 0.032; effect size 2.2.
> "6. Conflict-resolution mechanisms: Appropriators and their officials have rapid access to low-cost local arenas to resolve conflicts…" — p = 0.01; effect 3.2.

**E34 — Cox et al. 2010, abstract (full text).**
> "We analyzed 91 such studies to evaluate the principles empirically… We found that the principles are well supported empirically and that several important theoretical issues warrant discussion."

**E35 — Ancona & Caldwell 1992 (abstract†, lower confidence — use as paraphrase only).**
> "Over time, teams following a comprehensive [external] strategy enter into positive cycles of [external] activity, internal processes, and performance [that] enable long-term success."
> *Caution: the clause boundaries in this reconstruction are uncertain; the report should cite the paraphrase in C7 rather than this sentence.*

---

## 3. Appraisal by mechanism family

### 3.1 Psychological ownership

**Established (L1, individual).**
- Ownership is a distinct construct with replicable antecedents. The meta-analysis (k = 141; MASEM on 294 studies) supports control, knowing and investment, and adds **"safety"** — justice, trust, perceived organisational support, relational closeness — as an emerging antecedent **[D, D07/E7]**. That addition matters for this report: it makes ownership partly a *relational and contextual* product, not a personal trait. If the regional architecture is experienced as procedurally unfair or low-trust by small initiatives, the literature predicts weaker ownership of shared arrangements, not stronger.
- Ownership predicts discretionary contribution: incremental variance in organisation-based self-esteem and organisational citizenship behaviour, rated by peers **and** supervisors, over job satisfaction and commitment (three field samples, >800 employees) **[D, D03]**.
- Ownership has a documented dark side, but the meta-analysis reports it as an **outcome category**, not as a demonstrated cause of inter-organisational refusal: "dark-side outcomes (e.g., territorial behaviors)" **[D, D07/E7]**.

**Contested.**
- Whether ownership is *psychologically distinct* from commitment and identification, or a relabelled attitude. D07 argues incremental validity; D06 (narrative review) says the construct, its measurement and its nomological network remain **debated** and calls for boundary-condition work **[D]**. The honest reading: distinct enough to survive meta-analysis, not settled.
- Whether ownership yields *stewardship*. "Stewardship" appears in the literature as a label for prosocial investment **[D, D10 keyword list]** and in theory as a positive consequence **[D, D02]**, but no retrieved organisational-level study measures stewardship as a distinct behaviour attributable to ownership.

**Not established.**
- **Any organisational-level or inter-organisational-level measure of psychological ownership.** D05 supplies a group-level *construct* (collective ownership as a "single and shared mind-set") but is conceptual, with no instrument and no test in inter-organisational settings. D06 explicitly lists "multilevel applications of PO research" as a **future** agenda item — that is a direct, retrieved statement that the multilevel work had not been done as of 2017 **[D, E6]**. A targeted search for psychological ownership in inter-organisational collaboration returned no such study (only unrelated nonprofit network-portfolio work) **[U]**.
- Whether an *initiative* (as opposed to the people in it) can hold ownership. This is a conceptual gap, not a measurement gap.

**Level-jump risk: high.** Every measurement in D01–D07 is a person reporting a feeling. Transferring "the initiative feels ownership of its programme" is **analogical at best**. The strongest legitimate transfer is *aggregative and explicit*: the people who run an initiative report ownership of it, and those reports predict their citizenship behaviour toward it. That is a claim about staff and volunteers, not about the organisation as a corporate actor.

**Rival that would produce the same observable behaviour.** Resource dependence. An organisation that will not hand over a programme may be protecting the funding line that keeps its staff employed, with no ownership feeling involved. Retrieved evidence that this mechanism is real and consequential: revenue source shapes *goal displacement* and organisational structure **[D, D30/E28]**, and formality of collaboration tracks budget size and funding-stream concentration (Guo & Acar 2005, in Line C). **Discriminator:** ownership predicts discretionary, unrewarded contribution; resource dependence predicts contribution that tracks the funding stream and stops when it stops. These make *opposite* predictions about a programme whose funding has ended.

### 3.2 Territoriality

**Established (L1, individual; small groups).**
- The construct is well specified: territories include physical space, **ideas, roles and relationships**; behaviours are used to "construct, communicate, maintain, and restore" them; consequences include commitment *and* conflict, preoccupation and isolation **[D, D08/E9]**. That the consequences are listed as both positive and negative is the theory's own position — territoriality is not defined as dysfunction.
- One empirical field study measures the mechanism with *other people's* ratings, which is the strongest design retrieved in this family: ownership → claiming and anticipatory defending **conditional on trust**; high trust reduces territorial behaviour; but territorial behaviour in a high-trust setting is penalised by coworkers **[D, D09/E10]**.

**Contested.**
- Whether marking is functional or obstructive. Nothing retrieved adjudicates this at organisational level. The individual-level evidence says the *same* behaviour is read differently depending on the relational context (D09) — which implies the question "is marking functional?" has no context-free answer.
- The "identifying–marking–defending" triad as a measured sequence. D08 is conceptual; D09 measures claiming and anticipatory defending but not identity marking as a distinct step. The triad should be cited to D08 as **theory**, and to D09 as **partial empirical support**.

**Not established.**
- **Territoriality between organisations.** No retrieved study measures organisational claiming/defending (branding and naming, vetoes over referral routes, control of a target group, exclusion from a venue or a data set) between organisations. This is the single largest gap in this family, and it is the gap that matters most for the parent question.
- Whether organisational boundary-defence is functionally equivalent to individual territoriality. Analogy only.

**Level-jump risk: high.** Note also the *framing* risk: "territoriality" is a loaded label. On this evidence base it would be unwarranted to describe any real organisation's conduct as territorial, because nothing measures it at that level and because §4 shows at least three non-territorial mechanisms that produce identical conduct.

**Rival that would produce the same observable behaviour.** Accountability and legal responsibility. A board that will not transfer a statutory duty is not defending a territory; it is discharging a duty it cannot lawfully delegate. No retrieved empirical study tests this mechanism in collaboration settings **[U]** — its absence is a finding, and it means the fiduciary explanation cannot currently be weighed against the ownership explanation on evidence. A second rival is **professional boundary work**: in health care, what looks like organisational turf is often jurisdictional negotiation between professions, documented ethnographically (D27) and as a review theme (D28).

### 3.3 Autonomy and self-determination — and the level problem

This family splits cleanly into three bodies of evidence that are routinely conflated.

**(a) Individual need satisfaction (L1) — established, and irrelevant to organizational autonomy by itself.**
- Meta-analytic support across 99 studies/119 samples for need satisfaction predicting growth, internalisation and well-being, with the caveat that the review tests whether *each* need uniquely predicts and whether a composite score is defensible **[D, D14/E14]**.
- In **health** contexts specifically, 184 independent data sets show autonomy support → need satisfaction → autonomous motivation → better health outcomes **[D, D15]**. This is the one SDT finding that transfers into the *content domain* of this report: it is about patients and health behaviour, not about organisations.

**(b) Organisational autonomy (L3) — established as a measurement problem, contested as an effect.**
- Six dimensions; formal–legal status is a poor indicator; organisations with identical legal status differ substantially; "tensions between different levels of autonomy appear in practice" **[D, D16/E15]**. This is genuinely organisational-level and it is the most useful source in this family for the parent question: it says that asking "is this initiative autonomous?" is unanswerable without saying *which* autonomy (and that autonomy from the funder may coexist with dependence on a host organisation or a professional group).
- **The effect of autonomy on performance is not established here.** D16's contribution is that prior research conceptualised autonomy too narrowly; it does not report an autonomy→fragmentation or autonomy→performance effect. No retrieved meta-analysis of organisational autonomy and performance was located **[U]**.

**(c) Network-level unity/diversity (L4) — established as a management function.**
- Four case studies of immigrant-serving networks find unity and diversity both essential and mutually contradictory, requiring explicit network-level managerial work **[D, D17/E16]**. This is the closest retrieved evidence to the report's design question: diversity of autonomous members is treated as a *performance asset* whose costs must be actively managed, not as a defect to be designed out.
- Institutional-level support: recognition of the right of local appropriators to devise their own institutions is associated with success across 91 CPR studies (p = 0.032; effect 2.2) **[D, D35/E33]**. Domain transfer from common-pool resources is required; the *direction* of the finding is directly relevant to "autonomy as a reason, not an excuse".

**Level-jump risk: moderate, and asymmetric.** Organisational autonomy has a real L3 literature (D16). SDT's three needs have **no** L3 or L4 measurement in anything retrieved — applying "autonomy, competence, relatedness" to an organisation is an analogy, and applying it to an inter-organisational arrangement is a double analogy. What *is* defensible is the weaker, retrieved claim: the conditions that support autonomous motivation in people (support for volition, competence and connection) are the conditions under which the people who staff autonomous initiatives are likely to keep investing — and funder-imposed control is a documented threat to autonomous motivation (Deci et al. 2017; Cerasoli et al. 2014 in Line C).

**Rival that would produce the same observable behaviour.** Goal ambiguity and task uncertainty. Organisations that decline to align may simply be unable to specify what alignment would achieve, because the outcomes are unmeasurable. Retrieved evidence that ambiguity is consequential: four dimensions of goal ambiguity, with ambiguity negatively related to performance indicators in US federal agencies **[D, D29]**. If the regional outcome set is unmeasurable, the literature predicts coordination failure **without** any autonomy motive. **Discriminator:** coordination improves markedly when outcomes are made measurable, with no change in autonomy or ownership.

### 3.4 Identity, recognition and status

**Established (L1, in mergers — the closest empirical analogue).**
- Social identification is defined as "a perception of oneness", sourced partly in distinctiveness and prestige, and produces identity-congruent activity and support for institutions that embody the identity **[D, D18/E17]**. Conceptual, but the load-bearing definition for everything below.
- Merger evidence with real samples: 465 employees of a newly merged airline; the negative effects were "most marked for employees of the low-status premerger organization"; **permeability of intergroup boundaries helped the low-status group and hurt the high-status group** **[D, D19/E18]**. That asymmetry is a genuinely useful, counter-intuitive finding for collaboration design: the same openness that reassures a small partner may threaten a large one.
- Post-merger identification has effects **above and beyond** job insecurity, against the "merger folklore" **[D, D20]**. The practical recommendation retrieved is continuity plus specific communication.
- Identity threat is defined as an *appraisal* of "potential harm to the value, meanings, or enactment of an identity" **[D, D22/E24]** — a definition that makes threat measurable in principle (ask what is appraised as at risk), even though nothing retrieved measures it in a collaboration.
- Status conflict: disputes over relative respect positions; negative main effect on group performance; "hurts performance by undermining information sharing more than other types of conflict do" **[D, D24/E25]**. This is the mechanism that most directly connects *status* to *the thing fragmentation is supposed to destroy* — information flow.
- Founder identity now established at L1→L3: 49 founders, three identity types shaping firm-creation decisions **[D, D25/E26]**; 13 firms followed longitudinally, founders "use their firms as vehicles to defend who they are" **[D, D26/E27]**. Both are qualitative, small-n, single-industry. They establish that founder self-concept shapes organisational strategy; they do **not** establish that founder identity causes resistance to collaboration.

**Contested.**
- Whether identity threat is a *cause* of failed collaboration rather than a *consequence* of it. No retrieved study measures identity threat before and after a collaboration decision.
- Recognition vs funding. Bitektine's distinction between legitimacy, reputation and status as different social judgments, "each addressing a different question about the organization" **[D, D23/E23]** supplies the *conceptual* basis for separating "being recognised" from "being funded" — but it is conceptual, and **no retrieved empirical study tests recognition without funding in health promotion** **[U]**. The distinction is therefore available as a framing for local measurement (§6), not as a finding.

**Not established.**
- That identity threat materialises in *voluntary* collaborations between autonomous organisations. Every merger study retrieved is about involuntary or semi-voluntary consolidation of employment. Voluntary partnership may be a different psychological situation, and nothing retrieved tests that.
- Organisational-level identity threat measurement. D22 is about individuals' identities.

**Level-jump risk: moderate-to-high.** The merger literature is L1 measured inside an L3 event. Using it to explain why organisations decline to merge is analogical, though the analogy is closer than most because the event (consolidation) is the same kind of event.

**Rival that would produce the same observable behaviour.** Place and community attachment. Resistance that looks like identity defence may be protection of a site or a community. Devine-Wright reconceives local opposition as place-protective action arising when developments "disrupt pre-existing emotional attachments and threaten place-related identity processes" **[D, D34/E32]**; Nijs shows collective ownership of a *place* produces both exclusion of outsiders and prosocial investment in it **[D, D10/E11]**. In a food-and-green-space domain this rival is not exotic — it is the most plausible alternative in the report's own subject matter.

### 3.5 Level-discipline verdict

| Finding | Level measured | Status for the L4 question |
|---|---|---|
| PO antecedents (control, knowing, investment, safety) | L1 | **Analogical.** Usable as a hypothesis about staff/volunteers, not about organisations |
| PO → OCB, OBSE (incremental) | L1, multi-source | **Analogical.** The strongest L1 finding; still not an organisational behaviour |
| PO → no incremental performance | L1 | **Analogical**, and *binding*: it caps claims that ownership produces effectiveness |
| PO dark side = territorial behaviours | L1 (meta-analytic outcome category) | **Analogical, and weaker than usually assumed** — an outcome category, not a measured cause |
| Collective PO construct | L2 (theory) | **Analogical**; construct without instrument |
| Collective PO of place → exclusion + stewardship | L2 (surveys/experiments, Dutch/British) | **Analogical but nearest in kind** — group-level, place-based, two-sided |
| Territoriality construct; marking/defending | L1/L2 | **Analogical** |
| Territoriality conditional on trust | L1, coworker-rated | **Analogical**; the contingency finding is the transferable part |
| Six dimensions of organisational autonomy | **L3** | **Direct** (as a measurement frame), not as an effect |
| Autonomy → performance | L3 | **Contested / [U]** — do not assert |
| SDT needs at work | L1 | **Analogical** at L3; **unwarranted** at L4 |
| SDT in health contexts (patients) | L1 | **Direct for the domain**, irrelevant to organisational autonomy |
| Unity–diversity as network-level work | **L4** | **Direct** (qualitative, 4 cases) |
| Institutional recognition of rights to organise | L4/L5 (91 CPR cases) | **Direct in direction**, domain transfer required |
| Merger identification; status effects; permeability asymmetry | L1 in an L3 event | **Analogical (close)** |
| Status conflict → information sharing | L2 | **Analogical** |
| Founder identity → firm strategy | L1→L3, qualitative n = 49 / n = 13 | **Analogical**; establishes the mechanism exists, not its prevalence |
| Legitimacy vs reputation vs status | L3/L4 (theory) | **Conceptual**; supplies the recognition/funding distinction |
| Professional boundaries in integrated care | **L2/L3 (health)** | **Direct for the sector**; not organisational turf |
| Goal ambiguity → performance | L3 | **Direct** (US federal agencies; domain transfer) |
| Revenue source → goal displacement | L3 | **Direct** (review level) |
| Compliance without convergence | **L4 (field)** | **Direct** (101 English public organisations) |
| Collaboration conditions; trust loop | L4 | **Direct** (case-review level) |
| Place-protective action | L2/L4 | **Direct in direction**, different object |
| Design principles incl. conflict-resolution arenas | L4/L5 | **Direct in direction**, domain transfer required |
| Boundary spanning as strategy | L2 | **Analogical** |

**What survives.** Four things, and they are not the ones the mechanism vocabulary advertises: (i) organisational autonomy is **multidimensional** and legal status is a bad proxy (D16); (ii) the **field-level** evidence that organisations comply with institutional pressure without converging in practice (D31); (iii) the **network-level** evidence that unity and diversity are jointly required and contradictory (D17); (iv) the **institutional-design** evidence that recognition of the right to organise and low-cost conflict-resolution arenas are associated with durability (D35). Everything else in this line is analogy, however well-evidenced at its own level.

**What does not survive.** "The initiative is territorial." "The organisation feels ownership." "Autonomy is a basic need of organisations." Each of these would be a level jump, and the first would also be a motive attribution that no retrieved instrument supports.

---

## 4. Competing explanations, and what would discriminate between them

For each mechanism, at least one rival that produces the *same observable behaviour* without the proposed mechanism. "Observable behaviour" here means what the parent question can actually see in documents: refusal, non-participation, duplicate offers, separate reporting, non-merger.

| # | Rival explanation | What it substitutes for ownership/territoriality/identity | Retrieved evidence (level) | What would discriminate in Eindhoven–De Kempen |
|---|---|---|---|---|
| R1 | **Resource dependence** | Behaviour tracks funding exposure and mandate, not feeling | Revenue source shapes goal displacement and structure (L3, review) **[D, D30]**; formality of collaboration tracks budget and funding concentration (L3, Line C Guo & Acar) | Behaviour that changes when the funding stream changes while identity/ownership stay constant; contribution that stops when the money stops; matched pairs with similar identity but different exposure |
| R2 | **Institutional isomorphism / legitimacy** | Organisations copy the funder's categories to be fundable; looks like turf, is compliance | 101 English public organisations: "substantial evidence of compliance but more limited support for convergence" (L4) **[D, D31]** | **Decoupling**: the same organisation uses the funder's categories in reports but different categories in its own planning documents. Directly testable from public documents; a strong isomorphism result shows *divergence between reporting and practice*, not rivalry between organisations |
| R3 | **Accountability and legal responsibility** | A board cannot lawfully hand over a duty; looks like territoriality, is fiduciary | **No empirical study retrieved [U].** Nearest: coordination-burden management as what separates sustained from dissolved collaborations (Line C, Elston et al. 2023) | Behaviour changes when the duty is discharged differently (delivery shared, accountability retained) but not when the money changes; statutory basis visible in governance documents |
| R4 | **Goal ambiguity and task uncertainty** | Coordination fails because outcomes are unmeasurable, not because actors defend domains | Four ambiguity dimensions; ambiguity negatively related to performance indicators (L3) **[D, D29]** | Coordination improves sharply once outcomes are operationalised, with no change in autonomy or ownership. Also: whether the regional outcome set contains measurable indicators at all |
| R5 | **Transaction costs and capacity** | Small organisations do not collaborate because it is unaffordable | "the likelihood of disappointing outputs is high" (L4) **[D, D33]**; coordination burden as the survival variable (Line C, Elston et al.); boundary-spanning is a deliberate team strategy rather than an automatic response (L2) **[D, D36]** | Behaviour tracks organisational size/staff capacity rather than identity; capacity support (a funded coordination role) changes participation without changing identity |
| R6 | **Attachment to place / community protection** | Resistance protects a site or a community, not ownership of a programme | Place-protective action framework (L2/L4) **[D, D34]**; collective ownership of place → exclusion *and* stewardship (L2, Dutch/British) **[D, D10]** | What the objection targets: a change to a *site/place* versus a change in *who controls a programme*. In a food-forest/green-space setting this is the rival most likely to be confused with territoriality |
| R7 | **Professional boundary work** | Jurisdictional negotiation between professions, not between organisations | Ethnography in a stroke unit: discipline-specific identities and conflict over "the regulation of the medical-nursing boundary" (L2) **[D, D27]**; "professional identity" as one of seven review themes, 27 studies on roles/responsibilities (L2/L3) **[D, D28]** | Whether the contested object is a *role/expertise boundary* (who may do what) rather than an organisational boundary (who may decide/be paid) |
| R8 | **Identity is not threatened — diversity is functional** | Diversity of autonomous members is an asset requiring management, not a threat | "unity and diversity are essential to network performance, each makes contradictory demands" (L4) **[D, D17]** | Evidence that diverse, separately-branded members outperform harmonised ones on the shared outcome; and evidence that the coordination work is being done (network-level managerial work exists) |

**The discriminating logic in one sentence.** Ownership/territoriality predicts *discretionary, identity-linked, unrewarded* defence that persists after funding changes and is aimed at control of a programme; resource dependence predicts behaviour that tracks money; isomorphism predicts reporting that diverges from practice; fiduciary duty predicts persistence of the *duty* but flexibility about the *delivery*; goal ambiguity predicts collapse that dissolves once outcomes are specified; transaction costs predict a size gradient; place attachment predicts objections aimed at sites; professional boundary work predicts disputes about jurisdiction over tasks. These are distinguishable with documentary and interview data, and none of them requires attributing a motive.

---

## 5. Counter-evidence and failed replications

Searched deliberately, for evidence *against* the ownership/territoriality explanation. Reported as found, including where it weakens the mechanism.

**C1 — Ownership predicts knowledge *sharing*, not hoarding (L1).** 342 medical doctors, cross-sectional: ownership positively predicted both knowledge donating and knowledge collecting **[D, D11/E12]**. *Weight:* single study, convenience sample, cross-sectional, lower-tier journal (ABDC C), self-report. *Effect on this line:* it falsifies the simple inference "ownership → withholding". At individual level, ownership and sharing are positively associated. The "dark side" must therefore be about *what* is shared and with whom, not about sharing per se — which is exactly what D09's trust contingency predicts.

**C2 — Territorial behaviour is contingent, and high trust suppresses it (L1, two-source).** In a high-trust environment, ownership produced *less* territorial behaviour **[D, D09/E10]**. *Effect:* territoriality is not a fixed consequence of ownership; it is a response to a relational context. This shifts the explanatory burden onto the *context* (which is designable) rather than onto the actor (which is not).

**C3 — Ownership adds nothing incremental for performance (L1, three field studies).** D03 found ownership failed to add incremental value in predicting performance **[D, D03/E3]**. *Effect:* the "ownership produces extra-role effort" claim must be restricted to citizenship behaviour and self-esteem. Any argument that ownership improves *outcomes* is not supported by this line's best multi-source study.

**C4 — Preserving subgroup identity can increase bias (L2, two experiments).** Perceived continuation of the pre-merger identity strengthened the link to superordinate identification **and strengthened, rather than reduced, ingroup bias** **[D, D21/E19]**. *Effect:* this is the most important counter-evidence to the parent question's hopeful premise. "Protect local identity and cooperation will follow" is **not** what the experimental evidence says. Preserving identity can *increase* favouritism toward the preserved subgroup. The design implication is not "merge anyway"; it is that identity preservation needs to be paired with something that makes the superordinate category salient and the boundary permeable (D19).

**C5 — Shared/common ownership institutions work, when designed (L4/L5).** Across 91 studies, Ostrom's principles are "well supported empirically"; recognition of rights to organise (p = 0.032) and low-cost conflict-resolution arenas (p = 0.01) are associated with success **[D, D35/E33–E34]**. *Effect:* shared ownership is not inherently conflictual. Conflict is what the design has to handle, and the literature names the mechanisms (arenas, monitoring accountable to members, graduated sanctions) rather than relying on goodwill. Domain transfer from CPRs is required **[I]**.

**C6 — Diversity is essential to network performance (L4).** **[D, D17]** *Effect:* diversity is treated by the network-governance literature as a performance asset whose costs are managed, not as the problem.

**C7 — Boundary crossing is routine and strategic, not resisted (L2).** Teams develop distinct strategies towards their environment, and the study reports that the *type* of external activity — not merely its amount — determines performance **[D, D36, paraphrase of a reconstructed abstract]**. *Effect:* crossing boundaries is normal organisational work that varies in competence, not a symptom of pathology. Coordination failure may be a *skill and resource* problem (R5) rather than a motivational one.

**C8 — Isomorphism produces compliance without convergence (L4).** **[D, D31/E29]** *Effect:* when organisations adopt the funder's categories, the adoption may be presentational. This is counter-evidence to reading shared vocabulary as shared practice — and counter-evidence to reading *divergent* practice as territorial refusal.

**C9 — Professional boundaries do obstruct integration, in health care (L2).** **[D, D27/E22]** *Effect:* this is counter-evidence to the optimistic reading, and it is the health-sector evidence. But note what it documents: professional identity and jurisdiction, inside one hospital team — not organisational turf between organisations.

**Failed replications: none located.** No retrieved study reports a failure to replicate the ownership→territoriality link, and no retrieved meta-analysis reports a null for the dark-side category. **This is not reassurance.** The dark side is measured as self- or coworker-reported territorial behaviour on a small number of scales by a small number of research groups, mostly self-report, and D06 records that measurement is contested **[D]**. A literature with contested measurement has not yet had the chance to fail to replicate. **What would be needed:** an independent, multi-group replication with behavioural (not self-report) outcomes, ideally in a field setting where the "territory" is organisational rather than personal. **[U]**

**Where the mechanism family is weakest overall.** Not in the evidence for the mechanism at L1 — that is decent. In the complete absence of L3/L4 measurement, and in the failure of the mechanism's own literature to distinguish *ownership-driven refusal* from *resource-driven refusal*. The single most useful thing this line found for the parent report is a **negative** structural finding: the mechanism families are not currently capable of adjudicating the parent question at the level the parent question is asked.

---

## 6. What would have to be measured locally, and what this line cannot establish

### 6.1 No local measurement exists in the public record

This line found **no** measurement of psychological ownership, territorial behaviour, identity threat, status conflict, need satisfaction, or perceived autonomy in any Eindhoven or De Kempen health-promotion setting, in any retrieved source. Nothing in this file is evidence that any of these mechanisms operates in the region. Nothing in this file should be read as a statement about any named organisation or person. **[U]**

### 6.2 What would have to be measured, and with what

Ordered by feasibility from public documents first.

1. **Recognition versus funding (documentary; feasible now).** The Bitektine distinction operationalised as two independent counts per organisation per year: (a) *recognition* — named, invited, cited, listed as partner, given a speaking or governance role in regional documents; (b) *funding* — euros awarded, as penvoerder or co-financier. If recognition and funding diverge systematically (recognised but unfunded; funded but unnamed), then "being recognised" and "being funded" are separate goods in this region, and the status/identity mechanism becomes testable without fieldwork. **This is the highest-value measurement this line can propose**, because it uses the documents the other lines have already retrieved.
2. **Autonomy, six dimensions (documentary + one short survey).** Apply Verhoest's dimensions to a sample of local initiatives: autonomy to decide *what* to do, *how*, *with whom*, *with what budget*, and hiring/procurement. D16's warning is the method: do not infer autonomy from legal form. **[D, D16]**
3. **Contested-object log (meeting records, if obtainable).** Code each documented disagreement by object: a site/venue; a target group; a referral route; a data set; a name/brand; a budget line; a statutory duty. This is what separates territoriality (control of a programme), place attachment (a site) and professional boundary work (a task) — the three rivals that look identical in prose.
4. **Goal-ambiguity audit (documentary).** Score the regional outcome set on Chun's four dimensions: is there a comprehension-ambiguous mission, directive ambiguity (no clear objectives), evaluative ambiguity (no indicators), priority ambiguity (no ranking)? If evaluative and priority ambiguity are high, R4 predicts coordination failure with no motivational mechanism at all. **[D, D29]**
5. **Funding-exposure gradient (documentary + administrative data).** Budget share by stream per organisation, and whether participation in joint arrangements tracks it. This is the resource-dependence discriminator (R1) and is testable from Line A/B material.
6. **Capacity gradient (documentary).** Staff FTE and coordination time per organisation against participation. Tests R5.
7. **Only with fieldwork (excluded by the parent's scope):** identity-threat appraisals ("what would be at risk if this programme were jointly run?"), ownership of a shared arrangement (a group-referent ownership scale applied to a *programme*, not to an employer — no validated instrument exists for this, so it would be instrument development, not measurement **[U]**), and observed marking/defending in meetings.

### 6.3 What this line cannot establish

- That fragmentation in Eindhoven–De Kempen is caused by ownership, territoriality, autonomy needs or identity threat. **The evidence base cannot test these at the level the question is asked.**
- That any local actor is territorial, protective of a domain, or suffering identity threat. No measurement exists, and three rival mechanisms produce identical conduct.
- The relative weight of the mechanisms. No retrieved study compares ownership against resource dependence against goal ambiguity in the same setting. **[U]**
- Whether preserving local identity helps or hurts shared outcomes in this region. The best experimental evidence (C4) says preservation can increase subgroup bias; the best network evidence (C6) says diversity is essential. These are not reconciled in the literature, and this line will not pretend they are.
- Whether recognition without funding has measurable effects. Conceptual basis only (D23). **[U]**

### 6.4 Honest adjudication per mechanism

| Mechanism | Adjudication |
|---|---|
| Psychological ownership | **Established at L1; insufficient evidence to adjudicate at L3/L4.** Do not use as an explanation of organisational behaviour without new measurement |
| Territoriality | **Established at L1 with a trust contingency; insufficient evidence to adjudicate inter-organisationally.** At most an analogy |
| Autonomy (organisational) | **Established as a multidimensional construct (L3); effect on fragmentation not established.** Usable as a measurement frame, not as an explanation |
| Autonomy (SDT needs) | **Established at L1; not transferable to organisations without unwarranted inference.** Insufficient evidence to adjudicate at L3/L4 |
| Identity / identity threat | **Established at L1 inside mergers; insufficient evidence to adjudicate voluntary collaboration.** Analogy, close in kind |
| Status / recognition | **Established at L2 (status conflict harms information sharing); recognition-vs-funding distinction conceptual only.** Insufficient evidence to adjudicate at L4 |

---

## 7. Access log

All requests were made with `source_read`, signed with the operator's Web Bot Auth identity (`dsh-research-reader`, keyid `ey9Tj49-…`). Robots.txt was not relied on for any material source. No login, paywall, CAPTCHA, Cloudflare challenge or authentication wall was bypassed.

| # | Resource sought | Failure | Class | Recovery attempted | Outcome |
|---|---|---|---|---|---|
| A1 | Brown, Lawrence & Robinson 2005, *AMR* full text, `journals.aom.org/doi/10.5465/amr.2005.17293710` | **HTTP 403 Cloudflare challenge**, `cf-ray a60be14c0a3506ce-AMS` | access-restricted (Cloudflare) | OpenAlex by-DOI (deposited abstract); Crossref (no abstract for AOM) | **Recovered at abstract level†.** Full text not obtained; not bypassed |
| A2 | Deci, Olafsen & Ryan 2017, `annualreviews.org/.../annurev-orgpsych-032516-113108` | **HTTP 403 Cloudflare challenge**, `cf-ray a60be2a87f5966bd-AMS` | access-restricted (Cloudflare) | Crossref by-DOI | **Recovered at abstract level (verbatim).** Full text not obtained |
| A3 | Crossref REST, multiple parallel calls | **HTTP 429** on roughly half of parallel requests | transient (rate limit) | Sequential pacing; OpenAlex by-DOI as alternate channel | Recovered; no source lost |
| A4 | OpenAlex **search** endpoint (`/works?search=…`) | **HTTP 429** on every attempt (5 attempts, including a single isolated call) | transient/access-restricted (shared egress) | Crossref `query.bibliographic` for discovery; OpenAlex **by-DOI** (which worked) for abstracts and OA locations | Recovered; discovery was slower than planned |
| A5 | Semantic Scholar Graph API | **HTTP 429** on the `paper/search` endpoint and on single-DOI lookups after the first | transient (rate limit) | Abandoned the channel | No source depended on it |
| A6 | Nijs 2022 dissertation PDF (8.7 MB), `dspace.library.uu.nl/bitstream/handle/1874/416531/…pdf` | **"connection was aborted before the body completed"**, twice, on two URL variants | transient/format (oversized body) | DSpace landing page (`/handle/1874/416531`) → verbatim abstract + keyword list | **Recovered at abstract level (verbatim).** Full text not obtained; chapters not read |
| A7 | Fauchart & Gruber 2011 full text via EPFL Infoscience `infoscience.epfl.ch/record/151894` | **HTTP 429** | transient (rate limit) | OpenAlex by-DOI → green-OA record confirmed at EPFL, deposited abstract recovered | **Abstract level only†.** Full text not obtained |
| A8 | Powell & Baker 2014 | Crossref: DOI, **no abstract** (AOM deposit); OpenAlex by-DOI returned the deposited abstract | not-public (publisher elision) | OpenAlex by-DOI | **Recovered at abstract level†** (Line C had recorded this as "elided") |
| A9 | Liberati et al. 2016 abstract | Crossref: DOI, no abstract (Elsevier); OpenAlex: `abstract_inverted_index: null` | not-public | Europe PMC `resultType=core` by DOI | **Recovered at verbatim abstract level** (PMID 26730879) |
| A10 | Nooteboom et al. 2021 full text | Crossref: no abstract; OpenAlex: no abstract | not-public | Europe PMC `PMC7803720/fullTextXML` (CC BY) | **Recovered at full-text level**; theme 7 and discussion extracted |
| A11 | Brown 2009, "Claiming a corner at work", *J. Environmental Psychology* 29:44–52 | No abstract in Crossref or OpenAlex | not-public | — | **Metadata only. Excluded from the source table; no claim made** |
| A12 | Gagné & Deci 2005 PDF at `selfdeterminationtheory.org/...` (guessed path) | **HTTP 404** | moved (wrong path) | Crossref by-DOI abstract; did not pursue the SDT repository further | **Recovered at abstract level (verbatim)**; full text not obtained |
| A13 | Cox et al. 2010, Ecology & Society frames page | `"You must view this manuscript with a frames-capable browser"` | format | Direct PDF `…/vol15/iss4/art38/ES-2010-3704.pdf` | **Full text PDF recovered** (96,384 characters) |
| A14 | Crossref single-work endpoint with `select=` | **HTTP 400** (`select` unsupported on `/works/{doi}`) | defective request | Used `select` on the work-list endpoint; OpenAlex `authorships` for author strings | Recovered |
| A15 | Author-string verification for D01, D08, D18, D22–D26, D29, D31, D34, D36 | Publisher records display authors, but Crossref `/works/{doi}` could not be queried with `select` and several records displayed title only | not-public at the depth sought | Work-list `select=author` for 2 of them (Ashworth: confirmed; Chun: **single author in both indexes**) | **Partially unresolved.** Author strings flagged in the table's verification note; D29 flagged as a discrepancy |
| A16 | `web_search` tool as a discovery channel | Returned lists of links **without usable snippets**, and several results were library catalogues rather than sources | degraded channel | Switched to Crossref `query.bibliographic` + OpenAlex by-DOI | Discovery continued; no source lost, but DOI discovery was slower and partly dependent on the agent's prior knowledge of the literature (which is **not** a source and was used only to formulate queries, never as evidence) |
| A17 | Full text of the 12 reconstructed-abstract sources (D01, D08, D17, D18, D22–D26, D29, D31, D36) | Not attempted at full text: AOM/INFORMS/OUP/Oxford Academic are behind Cloudflare or subscription, and the abstracts were sufficient to state and bound the claim | access-restricted | Publisher landing pages were **not** probed further after the two recorded Cloudflare challenges (A1, A2) | **Abstract level only†** for these 12 sources; claims limited accordingly |

**No source was bypassed.** Two Cloudflare challenges, one repository rate-limit, one oversized PDF and one 404 were recorded rather than routed around. Where a publisher elided an abstract, no claim was made until an independent index supplied the deposited abstract; where that abstract was reconstructed from a word-position index, the quotation is marked † and used only where the reconstruction is unambiguous.

**Degradations to report to the Lead.** (i) `web_search` was not usable for discovery (no snippets); (ii) OpenAlex search and Semantic Scholar were 429 throughout, so discovery depended on Crossref's bibliographic endpoint and on the agent's knowledge of the literature *for query formulation only*; (iii) 10 of 36 sources are at reconstructed-abstract depth, and one is metadata only; (iv) no full text was obtained for any Academy of Management or Annual Reviews article.

---

## 8. Adjacent questions noticed, not researched

Logged, not pursued; each would require a different mandate.

1. Whether *recognition* without funding has measurable effects on small initiatives — the Bitektine distinction is available and untested in health promotion.
2. Whether collective psychological ownership of a *place* (D10) can be converted into stewardship of a shared programme without exclusion of newcomers — the two-faces finding implies a real design tension, and no study tests the conversion.
3. Instrument development for organisational- or programme-level ownership: no validated measure exists, and D06 lists multilevel application as future work.
4. Volunteer and staff retention under organisational change — an L1 literature that would matter for the "who bears the coordination cost" question, not retrieved here.
5. Whether the fiduciary/legal-accountability mechanism has *any* empirical literature in collaborative governance. One search direction, no hits retrieved; it may exist under "accountability in networks" (Klijn/Koppenjan tradition), which Line C did not retrieve either.
6. Whether status conflict has been measured in inter-organisational settings (as opposed to small groups) — no retrieved study.
7. Mission drift specifically in health-promotion NGOs (as distinct from the general nonprofit professionalisation and revenue-diversification reviews).

---

*End of Line D working file.*
