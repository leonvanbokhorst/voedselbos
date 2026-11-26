# The Dutch-language search: what was run, what came back, what was screened in

**Line:** revision line (v2), serving issue #25. **Author:** health-reviser. **Retrieved:** 26 November 2026, 21:11–21:14 UTC.
**Status:** raw working material and search audit for [`../note.md`](../note.md). Not evidence in itself.

**Why this file exists.** v1 stated its own limitation plainly: "No Dutch-language grey literature was systematically searched for the outcome literature (Line B searched English-language bibliographic databases only), so **the Dutch evidence base here is thinner than the Dutch question deserves** — that is a coverage limit, not a finding" (v1 §8). The PI required the Dutch search to be completed and to be auditable. This file records the queries, the engines, the counts where a count exists, the screening decisions, and the read depth of everything screened in.

**An honest limitation about counts, stated first.** Of the three engines used, only Europe PMC returns an exact `hitCount`. The general web-search engine used for Dutch grey literature returns a **ranked list capped at eight results per query and publishes no hit count**; a count cannot be reported for it and I do not invent one. **OpenAlex** — which would have given counts for Dutch-language scholarly works — returned **HTTP 429 (rate limit)** on both queries attempted and was abandoned. So: exact counts exist for the English-language bibliographic legs (§3), and for the Dutch legs the audit trail is the **verbatim query plus the screening decision for every result returned**, which is reproducible but not countable.

---

## 1. What v1 already had in Dutch (not re-searched here)

So that "the Dutch search is incomplete" is not confused with "there is no Dutch evidence", the Dutch-language material v1 already retrieved and this revision retains:

| v1 id | Document | Kind |
|---|---|---|
| `A1`, `A2`, `A3` | Pharos infosheet, theme page, 10 characteristics of a health-literate organisation | health-literacy grey literature, national |
| `A4`, `A6`, `A7` | RIVM M-POHL report 2026-0076, Nivel *Gezondheidsvaardigheden ontleed*, Staat VenZ kerncijfer | measurement / prevalence |
| `A25`, `A26` | Poelman et al. SPFL (Dutch instrument); *Voeding Nu* on schooltuin, samen eten, koken | food literacy |
| `C24`, `C25`, `C26`, `C29` | Municipal health evaluation + uitvoeringsagenda; GGD BZO board paper; GGD BZO VTV-2019 health-literacy factsheet | municipal and regional policy |
| `C37`, `C40`–`C43` | iPH; TSG 2022; *Tijdschrift voor Psychiatrie* 2025; *Tijdschrift Positieve Psychologie* 2017; *Huisarts en Wetenschap* 2021 | Positieve Gezondheid and its critique |
| `D2`, `D5`, `D6`, `D7`, `D8` | GNW jaarverslag; Nature For Health jaarverslag; WUR MSc thesis *Van Tuin Tot Bord*; RIVM/TNO *Welzijn op Recept*; ZonMw effectstudie page | Dutch green-health programmes, social prescribing |
| `D23` | Stichting Lezen en Schrijven, *Taal maakt gezonder* | literacy / health literacy overlap |
| `E8` | Verwey-Jonker, *Groen verbindt zorg en de buurt* 2015–2018 | the 9/5/4 gradient; volunteer education profile |

**What that set was missing, and what this revision adds:** published Dutch *applied research* on growing and health (as opposed to programme self-description), a Dutch PhD thesis, a Dutch realist/participatory study of green interventions in vulnerable neighbourhoods, and Dutch grey literature on food forests and health.

---

## 2. The Dutch queries, verbatim, with screening

### Q1 — community gardening and health (applied research)
Queries (one call, results merged, 8 returned):
`buurtmoestuin gezondheid onderzoek Nederland` · `volkstuin tuinieren gezondheid onderzoek Nederland` · `voedseleducatie volwassenen effect onderzoek Nederland` · `groene interventies zorg welzijn effectonderzoek Nederland`

Screened **in**: `edepot.wur.nl/409294` → **`F6`** (Schram-Bijkerk, Dirven-van Breemen & Otte, *Hoe gezond is stadslandbouw?*, *Bodem*, feb 2016 — RIVM authors, Dutch literature review). `projecten.zonmw.nl/nl/project/groen-samenspel` → **`F7`**. `edepot.wur.nl/116701` (*Vitamine G* — screened in as a lead, **not retrieved**, budget). `leydenacademy.nl/groen-samenspel-…` (project partner page, derivative of `F7`, **not retrieved**).
Screened **out**: a RIVM rapport 2017-0189 PDF (air-quality measures, wrong topic); a raadsinformatie memo on PFAS (wrong topic); two Google Scholar citation pages; an IARC conference page.

### Q2 — Dutch PhD theses and applied-research publications
Queries: `proefschrift buurtmoestuinen Nederland cohesie Veen Wageningen` · `ervaringsleren informeel leren gezondheid volwassenen onderzoek Nederland` · `gezondheidsvaardigheden wijkgerichte aanpak Pharos buurt` · `lectorale rede groen gezondheid hogeschool lectoraat`

Screened **in**: WUR staff-publications page for **E.J. Veen** (led to `F8`); `cris.maastrichtuniversity.nl … ROA_R_2024_5` (screened out on inspection — labour-market analysis of lifelong learning, no health link); `gezondin.nu … Overdrachtsdocument_Gezondheidsverschillen_Maart2026.pdf` (screened **in as relevant, not retrieved** — budget); `drenthesamengezond.nl … Aan-de-slag-met-leren` (screened in, not retrieved); Pharos *Jaarplan 2019* (screened out, superseded); `edepot.wur.nl/206884` (a 2013 hbo lectoraat reportage, screened out on age and topic); `greeni.nl`/(hbo-kennisbank) file (screened out — no identifiable health content in the snippet).

### Q3 — the thesis, stigma, and HAS
Queries: `Veen buurtmoestuinen onderzoek Wageningen publicatie` · `gezondheidsvaardigheden buurtbewoners onderzoek GGD gemeente artikel` · `hulp vragen schaamte stigma laagdrempelig onderzoek Nederland Movisie` · `HAS hogeschool lectoraat groene leefomgeving gezondheid onderzoek`

Screened **in**: `research.wur.nl/en/publications/community-gardens-in-urban-areas-…` → **`F8`** (Veen 2015 PhD thesis abstract, read in full). `movisie.nl … Wat-werkt-bij-Stigma-en-bestaansonzekerheid_dossier-2025.pdf` (screened **in as relevant and current, not retrieved** — budget). `gezondheidinkaart.nl/handlers/ballroom.ashx?function=download&id=685` (the Feitenkaart Gezondheidsvaardigheden — **retried, failed again**, see §4). `ggdgelderlandzuid.nl … AB-Stukken-1-oktober-2020.pdf` (screened in, not retrieved).
Screened **out**: WUR publications search page; a HAS jaarverslag 2023 PDF (no health-literacy or green-health content in the snippet); `anp.nl` press item on food-bank stigma (news, not research); an Ovid journal page (paediatric-family intervention in the UK).

### Q4 — health literacy in neighbourhood settings; adult cooking education; asking for help
Queries: `gezondheidsvaardigheden versterken buurtbewoners project evaluatie GGD Nederland` · `kookcursus volwassenen effect groenteconsumptie onderzoek Nederland` · `"hulp vragen" moeilijk mensen met beperkte gezondheidsvaardigheden onderzoek`

Screened **in**: `pharos.nl … poh_geen_doorsnee_patient_gezondheidsvaardigheden.pdf` (Pharos, health literacy in general practice — screened in, **not retrieved**); `pharos.nl … Master-thesis-Oumaima-Zaanani … toegankelijkheid-digitale-triage.pdf` (screened in, **not retrieved**).
Screened **out**: an immunisation-foundation PDF (vaccination information, off-topic); a horticulture cash-crop report; `open.overheid.nl` NPLV document (screened out on relevance after inspection of the snippet); `edepot.wur.nl/189856` (design of a vegetable intervention for *adolescents* — off-population). **Negative result recorded:** no Dutch study of adult cooking education with an outcome measure was surfaced by this query.

### Q5 — the decisive pairing, asked directly
Queries: `"gezondheidsvaardigheden" buurttuin OR moestuin OR voedselbos` · `voedselbos gezondheid onderzoek Nederland` · `ervaringsleren volwassenen buurt informeel leren professional`

**This is the query that matters most, and its result is the finding.** Nothing returned pairs *gezondheidsvaardigheden* with *buurttuin / volkstuin / voedselbos*. What came back instead:

- **Screened in:** `platform31.nl/artikelen/zo-versterken-voedselbossen-onze-gezondheid-en-het-landschap/` → **`F11`** (Dutch grey literature, 26 October 2026, on food forests and health). It is the closest Dutch text to the issue's proposition and it does **not** mention literacy, capability or measurement of either.
- **Screened in, not retrieved:** `kenniswest.be/artikel/voedselbossen-als-klimaatadaptatie-in-nederland-…` (a Flemish republication of a Dutch item — a **derivative**, not an independent witness); `pimmartens.com … voedselbos-als-dierenapotheek-vbm-winter-2025.pdf` (same author as `F11`, medicinal framing — screened in, not retrieved, and it would raise the "no medicinal claims" caution if used); `mboin2030.nl … Dialogisch Valideren` (recognition of informal learning — adjacent to *ervaringsleren*, not health); `gezondheidinkaart.nl/mosaic/dashboard/bestaanszekerheid/gezondheidsvaardigheden` (retrieved — a JavaScript shell, see §4); `gezondheidsvaardigheden.nl/aan-de-slag/agenderen/wat-zijn-gezondheidsvaardigheden` (Alliantie Gezondheidsvaardigheden explainer — screened out as duplicative of `A1`–`A3`).
- **Screened out:** `onsgebied.nl` dialog page; an EPALE toolkit PDF.

### Q6 — locating the thesis copy
Query: `"Community gardens in urban areas" Veen thesis edepot.wur.nl social cohesion alternative food` → research portal, WUR library catalogue and AGRIS records for the same thesis. The **full text was not retrieved**; the abstract/summary on the research portal was read in full (§3).

---

## 3. Everything screened in, with read depth

| Id | Document | Producer / venue | Date | Read depth | What it contributes |
|---|---|---|---|---|---|
| **`F6`** | *Hoe gezond is stadslandbouw? Een literatuuronderzoek* (D. Schram-Bijkerk, L. Dirven-van Breemen, P. Otte) | RIVM authors, published in *Bodem* 26(1):30–31 | februari 2016 | **full text** (PDF, edepot.wur.nl/409294, 12 000 of 15 544 chars) | The Dutch applied-research review of urban agriculture and health: movement, fruit and vegetable consumption, stress, social contact, neighbourhood cohesion; plus the RIVM questionnaire developed to measure health effects, and the counter-findings on integration and exclusion |
| **`F8`** | *Community gardens in urban areas: a critical reflection on the extent to which they strengthen social cohesion and provide alternative food* (E.J. Veen) | Wageningen University, internal PhD thesis (Rural Sociology / WASS) | 2015 | **abstract and summary read in full** (research.wur.nl record); **thesis full text not retrieved** | Seven Dutch cases, two years of participant observation plus interviews and questionnaires; place-based vs interest-based gardens; "mutual help" as the depth of social cohesion; the finding that the organisational form determines whether produce reaches the plate; the exclusion finding |
| **`F7`** | *Groen Samenspel* (ZonMw project 11010012310010) | Hecht GGD Hollands Midden, with LUMC, Leyden Academy, Gemeente Leiden, AWPG Lumens, iPH + Hogeschool Leiden, Provincie Zuid-Holland | 2024–2025 | **full text of the project record** (projecten.zonmw.nl) | A Dutch realist review plus participatory action research on green interventions in vulnerable neighbourhoods; the resident finding (green valued as a place to rest and meet) and the "leefwereld" condition |
| **`F11`** | *Zo versterken voedselbossen onze gezondheid én het landschap* (E. Wits) | Platform31 | 26 oktober 2026 | **full text** | Dutch grey literature on food forests and health: health framed as being outside, social activity, heat and biodiversity; the MANTRA rural-lab approach; **no literacy, no outcome measurement** |
| **`F12`** | NARCIS service notice | DANS (KNAW/NWO) | retrieved 2026-11-26 | **full text** | The Dutch national research portal **went offline on 3 July 2023**; a successor ("Portal of Research Output from the Netherlands", UKB/SURF) is named. This is why the instruction to search NARCIS cannot be executed as written |

**Screened in and not retrieved (recorded so the gap is visible, not hidden):** Movisie, *Wat werkt bij stigma en bestaansonzekerheid* (2025); Pharos, *Geen doorsnee patiënt*; Pharos/Hogeschool master thesis on digital triage accessibility; *Vitamine G* (WUR, effects of green environment on health); gezondin.nu *Overdrachtsdocument Gezondheidsverschillen* (March 2026); *Voedselbos als dierenapotheek* (P. Martens, 2025). Each is a plausible addition; none was needed for a claim in the note, and the note makes no claim from any of them.

---

## 4. Failures, classified

| Target | Failure | Class | Recovery attempted | Outcome |
|---|---|---|---|---|
| `gezondheidinkaart.nl/handlers/ballroom.ashx?function=download&id=685` (Feitenkaart Gezondheidsvaardigheden) | Served as `application/octet-stream`; the reader rejects it | **format** | Retried the exact URL that failed in v1; tried the dashboard HTML instead | **Not retrieved — second failure, same mode.** Recorded rather than worked around; no bypass attempted |
| `gezondheidinkaart.nl/mosaic/dashboard/bestaanszekerheid/gezondheidsvaardigheden` | Page returns a JavaScript application shell ("Loading…", "Kies een gebied", "Kies een dimensie") with **no data values server-side** | **format** (client-rendered dashboard) | Read the shell to establish that area selection exists | **Values not retrieved.** That a municipal-level Dutch health-literacy figure exists in this dashboard is **[U]** — it is a legitimate route for the PI |
| `narcis.nl` | Redirects to a DANS service notice: service ended 3 July 2023 | **moved / discontinued** | Recorded the successor portal named by DANS | Recovered as a finding (`F12`); the thesis search was done through the WUR research portal instead (`F8`) |
| `api.openalex.org` (2 Dutch queries) | **HTTP 429**, empty body, twice | **transient / rate limit** | Abandoned the engine; no retry loop | **Two planned Dutch hit counts not obtained.** Stated as a gap, not papered over |
| `sciencedirect.com` (SDT gardening paper) | **403**, Cloudflare challenge, `cf-ray a60be0c9084f23e3-AMS` | access-restricted | Unpaywall → HAL repository copy | Recovered (`F5`); see `com-b-and-sdt.md` §6 |
| `voedseleducatie volwassenen` (Q1) and `kookcursus volwassenen effect` (Q4) | Nothing relevant returned | **not published / not indexed in the engines used** (as far as searched) | Two phrasings; one English-language bibliographic route already covered adult cooking by `D16`–`D18` | **Recorded as a negative result:** no Dutch adult food-education study with outcomes surfaced |

No login, paywall, CAPTCHA, cookie wall or Cloudflare challenge was bypassed. robots.txt was not consulted as a blocker for any of these retrievals; nothing here depended on it.

---

## 5. What the Dutch search changes, and what it does not

**Changes.** Three things that v1 could not say:

1. **There is a genuine Dutch applied-research literature on growing and health, and it is modest, observational and about exposure and contact** — not about literacy (`F6`, `F8`). It reports movement, fruit and vegetable consumption among those who garden, stress reduction, social contact and neighbourhood cohesion; it reports its own counter-findings (gardens "do not necessarily foster a more inclusive society"; groups may work *next to* rather than *with* each other; a tight group can make others feel excluded) [D, `F6`, `F8`].
2. **The Dutch field has a measurement instrument of its own for this**, developed at RIVM to measure health effects of urban agriculture [D, `F6`]. That is directly relevant to the "instruments vs assessment" question: a context-specific Dutch instrument exists, and it measures movement, consumption, stress, social contact and cohesion — **it does not measure health literacy**, and no source claims it does.
3. **Dutch green-intervention research is already doing the thing this report recommends** — realist review plus participatory work, with the finding that the condition of success is "aansluiten bij de leefwereld van bewoners" [D/C, `F7`]. That is a Dutch precedent for context-sensitive evaluation, and it comes from the GGD/academic network, not from a garden.

**Does not change.** Nothing retrieved in Dutch pairs *gezondheidsvaardigheden* with *buurttuin*, *volkstuin* or *voedselbos*. The Dutch search therefore **confirms the shape of the gap** rather than filling it: the construct and the practice exist in the same country, in the same provinces, in institutions one governance step apart, and no retrieved Dutch source puts them in one study. That is a statement about the sources searched — **not** a finding that the mechanism does not work.
