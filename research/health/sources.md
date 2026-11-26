# Sources — issue #25, health literacy and shared green practice

Every source cited in [`note.md`](note.md), with the id used there. Ids keep the delegated line's own numbering so that a claim can be traced back to the line's full source table and access log without duplication:

- **`A`** — [`working/hl-construct.md`](working/hl-construct.md) §8 (37 sources)
- **`B`** — [`working/green-health-evidence.md`](working/green-health-evidence.md) §9 (24 sources; `S13` was reserved and dropped, so the numbering has a visible gap)
- **`C`** — [`working/regional-map.md`](working/regional-map.md) Sources (44 sources)
- **`D`** — [`working/nl-programmes.md`](working/nl-programmes.md) §8 (25 sources)
- **`E`** — the Lead's own retrievals, listed in full below with sha256 and retrieval time; also transcribed in [`working/lead-verification.md`](working/lead-verification.md)
- **`F`** — the **revision line's** retrievals (v2, 26 November 2026), listed in full below with sha256 and retrieval time; the working notes are [`working/com-b-and-sdt.md`](working/com-b-and-sdt.md), [`working/nl-literature.md`](working/nl-literature.md) and [`working/assessment-methods.md`](working/assessment-methods.md)

Read depth matters and is reproduced for the ids that carry a load-bearing claim: **full** = the whole retrieved text was read; **partial** = named sections; **abstract** = the publisher or Europe PMC abstract only. Where a claim rests on an abstract, the note says so.

All retrievals 26 November 2026 unless stated. No login, paywall, CAPTCHA or Cloudflare challenge was bypassed; failed retrievals are logged in [`note.md`](note.md) §8 and in each working file's access log.

---

## E — the Lead's own retrievals (signed `source_read`, Web Bot Auth `dsh-research-reader`, keyid `ey9Tj49-…`)

| Id | Document | Publisher | Date | URL | Retrieved (UTC) | sha256 (first 16) | Depth |
|---|---|---|---|---|---|---|---|
| **E1** | Over DE STAP (about page) | DE STAP naar gezonder | pub. 2022-10-04, mod. 2026-03-03 | https://www.destapnaargezonder.nl/over-de-stap/ | 2026-11-26T20:29:37 | `7d367ff659236e11` | full (3 259 chars) |
| **E2** | Eindhoven — activity directory (147 entries) | DE STAP naar gezonder | undated, live 2026 | https://www.destapnaargezonder.nl/eindhoven/ | 2026-11-26T20:29:50 | `1ab60cb1d1910d11` | full (11 780 chars), counted |
| **E3** | Buurtmoestuin Irisbuurt (listing) | DE STAP naar gezonder | pub. 2026-05-26, mod. 2026-08-28 | https://www.destapnaargezonder.nl/buurtmoestuin-irisbuurt/ | 2026-11-26T20:29:40 | `d9e6a4d213e338e1` | full (2 304 chars) |
| **E4** | 't Kruidenkafe Kalmoesplein (listing) | DE STAP naar gezonder | pub. 2025-02-25, mod. 2026-11-24 | https://www.destapnaargezonder.nl/t-kruidenkafe-kalmoesplein/ | 2026-11-26T20:29:40 | `0080e86cc6d831c3` | full (2 534 chars) |
| **E5** | Centre of Expertise Health (page served under browser title "Startpunt Samenzorg") | Fontys Hogeschool | undated, live 2026 | https://www.fontys.nl/Onderzoek/Gezonde-en-inclusieve-samenleving-1/Centre-of-expertise-Health.htm | 2026-11-26T20:30:08 | `e6c9e60793830029` | full (15 807 chars) |
| **E6** | Gezondheidsvaardigheden in Nederland. M-POHL Health Literacy Survey 2024-2026 (RIVM-briefrapport **2026-0076**) | RIVM (Fransen, Meulman, Rademakers, Heijmans); commissioned by VWS | 2026 | https://www.nivel.nl/sites/default/files/bestanden/13473.pdf | 2026-11-26T20:36:41 | `c521c7317c121370` | full text retrieved (PDf, 55 pp.); quotes verified in §3.1/§3.2 |
| **E7** | Infosheet gezondheidsvaardigheden en laaggeletterdheid | Pharos | oktober 2026 | https://www.pharos.nl/infosheets/gezondheidsvaardigheden-en-laaggeletterdheid/ → resolves to `.../infosheetgezondheidsvaardighedenenlaaggeletterdheid/` | 2026-11-26T20:29:44 | `a575a3d7cab2d83e` | full (11 742 chars) |
| **E8** | Groen verbindt zorg en de buurt. Van storming naar performing in een stimuleringsprogramma, 2015-2018 | Verwey-Jonker Instituut (Van der Klein, Wilderink & Reches), for the Oranje Fonds | Mei 2019 | https://www.verwey-jonker.nl/wp-content/uploads/2020/07/315009_Groen_verbindt_zorg_en_de_buurt_WEB-2.pdf | 2026-11-26T20:41:18 | `4cffe46428cb9c60` | full text retrieved (PDF, 358 720 chars); summary figures for the three statements and the education profile verified in §3.4, §3.9 and §4 |

Note on **E6**: the Pharos factsheet (`A1`/`E7`) cites the *revised* report, RIVM **2026-0107**. That version's full text was not obtainable (no accessible bitstream; record and abstract only), so the note quotes the earlier version **2026-0076**, whose headline figures are identical. The version difference is recorded rather than hidden. DOI 10.21945/RIVM-2026-0076 / 10.21945/RIVM-2026-0107.

**Open discrepancy, deliberately not resolved.** The Pharos factsheet gives the Q47 upper bound as **52.8%** in its headline range and **52.3%** in its own explanatory paragraph. **No source retrieved explains the difference, and this note does not attribute it to a difference between report versions** — that would require reading 2026-0107, which was not possible. The discrepancy is reported as observable, and the upper bound is stated as **52.3–52.8%** (note §6.1).

**`E5` re-retrieved in the revision (v2).** Same URL, retrieved 2026-11-26T21:13:51Z, `text/html`, sha256 `8885d9ebd2737d7a…`, browser title "Startpunt Samenzorg – Samen werken aan toekomstbestendige zorg | Fontys". The three themes, the board composition ("Slimmer Leven, Pharos, GGD-BZO, Transvorm, Fontys Mens en Gezondheid en Fontys Paramedisch"), the DE STAP partnership line, the "Groene stedelijke leefomgeving" and "Gezonde voedselomgeving" documents, the Theory of Change paragraph, the "Impact for Health" research calls and the named contacts were all confirmed present. **New in the revision:** the *projects* listed under the health-literacy theme are clinical/organisational (hospital food and fluid monitoring, Contactladder, KwilT) and the *documents* listed under the green-environment theme are urban green and heat stress — no public project joins the two themes (P33).

---

## A — health literacy construct, Dutch prevalence, food literacy (line A)

| Id | Document | Publisher / venue | Date | URL or DOI | Depth |
|---|---|---|---|---|---|
| A1 | Infosheet gezondheidsvaardigheden en laaggeletterdheid | Pharos | okt 2026 | pharos.nl (see E7) | full |
| A2 | Themapagina Gezondheidsvaardigheden en laaggeletterdheid | Pharos | undated (2026) | https://www.pharos.nl/thema/laaggeletterdheid-gezondheidsvaardigheden/ | full |
| A3 | De 10 kenmerken van een gezondheidsvaardige organisatie | Pharos | undated | https://www.pharos.nl/gezondheidsvaardige-organisatie/ | full |
| A4 | Gezondheidsvaardigheden in Nederland (M-POHL HLS 2024-2026), rapport 2026-0076 | RIVM | 2026 | see E6 | full |
| A6 | Gezondheidsvaardigheden ontleed — cijfers 2025 | Nivel (Heijmans et al.) | juni 2026 | https://www.nivel.nl/sites/default/files/bestanden/13475.pdf | full |
| A7 | Gezondheidsvaardigheden: ontoereikend of problematisch (kerncijfer) | Staat van Volksgezondheid en Zorg | updated 7-7-2026 | https://www.staatvenz.nl/kerncijfers/gezondheidsvaardigheden-ontoereikend-problematisch | full |
| A9 | Critical health literacy: a review and critical analysis (Chinn) | Soc Sci Med | 2011 | doi:10.1016/j.socscimed.2011.04.004 | abstract |
| A14 | Health literacy reductionism (Okuhara, Okada & Furukawa) | Health Promot Int 41(4) | 2026 | doi:10.1093/heapro/daag118 | abstract |
| A16 | Does health literacy mediate SES → health? (Berete et al., n = 8 080) | BMC Public Health | 2024 | doi:10.1186/s12889-024-18676-7 | abstract |
| A25 | Self-perceived food literacy scale, NL (Poelman et al.) | IJBNPA 15:54 | 2018 | doi:10.1186/s12966-018-0687-z | abstract |
| A26 | "Schooltuin, samen eten of koken helpt" (Voedingscentrum authors) | Voeding Nu | 8-10-2021 | https://voedingnu.nl/artikelen/schooltuin-samen-eten-of-koken-helpt | full |
| A27 | Literacy approaches at the environment-health nexus: scoping review (Kallenbach et al.) | Front Public Health 14 | 19-10-2026 | doi:10.3389/fpubh.2026.1960284 | partial |
| A28 | FoodACT school-garden protocol (NCT05839080), Denmark | PLoS ONE | 2025 | doi:10.1371/journal.pone.0320574 | abstract |
| A29 | Enhancing food literacy through school gardening, Tasmania | IJERPH | 2023 | doi:10.3390/ijerph20186794 | abstract |
| A31 | School-based interventions on Food and Nutrition Literacy: systematic review | Br J Nutr | 2023 | doi:10.1017/s0007114522002811 | abstract |
| A32 | Employees' mental health at a botanical garden, India | Ind Psychiatry J | 2019 | doi:10.4103/ipj.ipj_94_18 | abstract |

Not used for any claim but present in the line's table: `A5`, `A8`, `A10`–`A13`, `A15`, `A17`–`A24`, `A30`, `A30b`, `A30c`, `A33`, `A34` (see the working file). **`A`'s central limitation:** most entries are abstract-level; Nutbeam (2000) and Vidgen & Gallegos (2014) were not obtained, so the tripartite typology is stated from four retrieved secondary attestations.

---

## B — gardening, green practice and health outcomes (line B)

| Id | Document | Authors / venue | Year | DOI or URL | Depth |
|---|---|---|---|---|---|
| B1 | Gardening is beneficial for health: a meta-analysis | Soga, Gaston & Yamaura, *Prev Med Rep* 5:92–99 | 2017 | doi:10.1016/j.pmedr.2016.11.007 (PMC5153451) | full to §3.3; **Lead re-read Table 2** |
| B3 | Nature-based outdoor activities for mental and physical health: SR & MA | Coventry et al., *SSM Popul Health* 16:100934 | 2021 | doi:10.1016/j.ssmph.2021.100934 | abstract |
| B4 | Community gardens and their effects on diet, health, psychosocial and community outcomes: a systematic review | Hume et al., *BMC Public Health* 22:1247 | 2022 | doi:10.1186/s12889-022-13591-1 | abstract |
| B5 | Urban collective garden participation and health: a systematic literature review | Tharrey & Darmon, *Nutr Rev* 80(1):6–21 | 2021 | doi:10.1093/nutrit/nuaa147 | abstract; OA copy exists at hal.inrae.fr/hal-03229527 (not retrieved) |
| B7 | Improving lifestyles sustainability through community gardening: the JArDinS quasi-experimental study | Tharrey et al., *BMC Public Health* 20:1798 | 2020 | doi:10.1186/s12889-020-09836-6 | **Lead re-read abstract + methods** |
| B9 | Allotment gardening and health: a comparative survey among allotment gardeners and their neighbours | van den Berg, van Winsum-Westra, de Vries & van Dillen, *Environ Health* 9:74 | 2010 | doi:10.1186/1476-069X-9-74 (PMC3001426) | **Lead re-read abstract** |
| B11 | Effectiveness of horticultural therapy: SR of RCTs | Kamioka et al., *Complement Ther Med* 22(5) | 2014 | doi:10.1016/j.ctim.2014.08.009 | abstract |
| B12 | Effectiveness of Horticultural Therapy in Older Adults without Dementia: SR & MA | Giang et al., *JAMDA* 25(12) | 2024 | doi:10.1016/j.jamda.2024.105296 | abstract |
| B15 | A systematic review of the health and well-being impacts of school gardening | Ohly et al., *BMC Public Health* 16:286 | 2016 | doi:10.1186/s12889-016-2941-0 | abstract |
| B16 | School gardening and children's fruit and vegetable intake: a cluster RCT | Christian et al., *IJBNPA* 11:99 | 2014 | doi:10.1186/s12966-014-0099-7 | abstract |
| B23 | Unexpected effects of urban food activism on community and human wellbeing | Wardle et al., *Local Environment* 29(5):647–662 | 2024 | doi:10.1080/13549839.2023.2298675 | abstract |

**`B`'s central limitation, reproduced because it bounds every number above:** no full text of any empirical study was read except Soga (partly) and the UK green social prescribing summary (partly); all effect sizes are the authors' abstract figures.

---

## C — the regional health landscape (line C)

| Id | Document | Publisher | Date | URL | Depth |
|---|---|---|---|---|---|
| C1 | Over DE STAP | DE STAP naar gezonder | mod. 2026-03-03 | see E1 | full |
| C3 | DE STAP partners (193 names, counted) | DE STAP naar gezonder | mod. 2026-03-27 | https://www.destapnaargezonder.nl/de-stap-partners/ | full, counted |
| C4 | Partner worden | DE STAP naar gezonder | undated | https://www.destapnaargezonder.nl/de-stap-partners/partner-worden/ | full |
| C5 | Paco — online partnercommunity | DE STAP naar gezonder | undated | https://www.destapnaargezonder.nl/de-stap-partners/paco/ | full |
| C6 | Aanmelden aanbod DE STAP (the four criteria) | DE STAP naar gezonder | undated | https://www.destapnaargezonder.nl/de-stap-partners/aanmelden-aanbod-de-stap/ | full |
| C7 | Eindhoven — activity directory | DE STAP naar gezonder | undated | see E2 | full, parsed |
| C9 | Onze tuin (De Iristuin, Buurthuis De Blokhut) | Buurthuis De Blokhut | undated | https://www.buurthuisdeblokhut.nl/onze-tuin/ | full |
| C10 | 't Kruidenkafe Kalmoesplein (listing) | DE STAP naar gezonder | mod. 2026-11-24 | see E4 | full |
| C11 | 't Kruidenkafé programma april–mei 2026 | 't Kruidenkafé / GGzE | March 2026 | https://www.destapnaargezonder.nl/wp-content/uploads/2026/03/Kruidencafe-april-mei-2026.pdf | full |
| C12 | Vacature Vrijwillige kok Kruidenkafe (the GGzE attribution) | werkenbijggze.nl | undated | https://www.werkenbijggze.nl/vrijwilliger/vrijwillige-kok-kruidenkafe | full |
| C24 | Evaluatie uitvoeringsagenda gezondheid 2023 en bijstelling 2024-2025 | Gemeente Eindhoven | 2024 | https://www.eindhoven.nl/sites/default/files/2024-07/DT_4%20Bijlage%201%20Evaluatie%20uitvoeringsagenda%20gezondheid%202023%20en%20bijstelling%202024%202025.pdf | full |
| C25 | Evaluatie 2024-2025 en Uitvoeringsagenda Programma Gezondheid 2026-2027 | Gemeente Eindhoven | December 2025 | https://www.eindhoven.nl/sites/default/files/2025-12/Evaluatie%202024-2025%20en%20Uitvoeringsagenda%20Programma%20Gezondheid%202026-2027_0.pdf | full |
| C26 | Voorlegger Penvoerderschap Vitale Communities & Bewustwording in 2026 (AB 10-12-2025) | GGD Brabant-Zuidoost | 18-11-2025 | https://www.ggdbzo.nl/app/uploads/sites/2/2022/07/20.-Voorlegger-Penvoerderschap-Vitale-Communities-Bewustwording-in-2026.pdf | full; **Lead re-read** |
| C30 | Zo zetten Fontys en jij DE STAP naar gezonder | Fontys Hogeschool | 09-06-2023 10:38 | https://www.fontys.nl/nieuws/zo-zetten-fontys-en-jij-de-stap-naar-gezonder/ | full; **Lead re-read** |
| C31 | Centre of Expertise Health | Fontys Hogeschool | live 2026 | see E5 | full |
| C33 | DE STAP naar Gezonder – Eckart / Vaartbroek (professionele werkplaats) | Fontys Paramedisch | live 2026 | fontys.nl (see working file) | full |
| C34 | Gezondheidskloof in buurten aanpakken: 'Moet duurzamer' | BRON (Fontys) | 02-12-2025 | https://bron.fontys.nl/gezondheidskloof-in-buurten-aanpakken-moet-duurzamer/ | full |
| C35 | Bestuursverslag en jaarrekening 2025 Stichting Fontys | Stichting Fontys | 2026 | https://www.fontys.nl/Download/Bestuursverslag-en-jaarrekening-2025-Stichting-Fontys.htm | partial |
| C37 | Effecten meten (Positieve Gezondheid) | Institute for Positive Health | undated | https://www.iph.nl/positieve-gezondheid/effecten-meten/ | full |
| C40 | Het meten van een brede benadering van gezondheid vraagt een brede aanpak in wetenschappelijk onderzoek (Nahar-van Venrooij & Timmers) | TSG 100:170–173 | 27-10-2022 | doi:10.1007/s12508-022-00366-7 | full |
| C41 | Hoe stevig is de wetenschappelijke basis van het concept positieve gezondheid? (Vinkers & Chiu) | Tijdschrift voor Psychiatrie 67(4):213–215 | April 2025 | tijdschriftvoorpsychiatrie.nl (see working file) | full |
| C42 | Positieve gezondheid kritisch beschouwd — niet nieuw, onduidelijk, misleidend en niet zonder risico (Van Staa, Cardol & Van Dam) | Tijdschrift Positieve Psychologie 2017 nr. 3/4 | 2017 | surfsharekit.nl (see working file) | full |
| C43 | Is positieve gezondheid een aanwinst voor de huisarts? (book review, Lucassen) | Huisarts en Wetenschap | Sept 2021 | henw.org (see working file) | full |

Ids `C2`, `C8`, `C13`–`C23`, `C27`–`C29`, `C32`, `C36`, `C38`, `C39`, `C44` are in the working file but carry no claim in the note.

---

## D — Dutch green-health programmes, social prescribing, cooking, exclusion (line D)

| Id | Document | Publisher | Date | URL or DOI | Depth |
|---|---|---|---|---|---|
| D2 | Jaarverslag en jaarrekening 2024 Stichting Gezond Natuur Wandelen | Stichting GNW | 2024 (vastgesteld 14-06-2024) | gezondnatuurwandelen.nl (PDF, see working file) | full |
| D5 | Jaarverslag Nature For Health 2020 (records *Beter in het Groen* going offline) | Nature For Health | 2021 | nfhfoundation.com (PDF, see working file) | full |
| D6 | Qualitative Evaluation 'Van Tuin Tot Bord' (MSc thesis) | Wageningen University | 2022 | https://edepot.wur.nl/569428 | full |
| D7 | Duurzaam borgen van Welzijn op Recept | RIVM & TNO, rapport 2024-0027 | 2024 | doi:10.21945/RIVM-2024-0027 | partial (~p.30) |
| D9 | National Evaluation of the Green Social Prescribing Project — Final Report Summary | Defra / Sheffield, Sheffield Hallam, Exeter, Plymouth | Jan 2024 | http://shura.shu.ac.uk/34171/1/GSP-eval-final-report-summary-2024.pdf | full summary (107k-char full report unread) |
| D10 | The Humber and North Yorkshire Green Social Prescribing Programme Cohort Evaluation | University of York et al. | Apr 2023 | eprints.whiterose.ac.uk/201362 (DOI 10.15124/yao-3jbj-8776) | partial |
| D11 | Social prescribing: less rhetoric and more reality. A systematic review (Bickerdike et al.) | *BMJ Open* 7:e013384 | 2017 | doi:10.1136/bmjopen-2016-013384 | abstract |
| D12 | Bayesian re-analysis suggests participation rather than referral underlies the benefits of social prescribing (Huang et al.) | *Front Public Health* 14:1951236 | 2026 | doi:10.3389/fpubh.2026.1951236 | abstract |
| D14 | Patient uptake and adherence to social prescribing: a qualitative study (Pescheny et al.) | *BJGP Open* 2(3) | 2018 | doi:10.3399/bjgpopen18X101598 (PMC6189784) | full |
| D15 | Community engagement: improving health and wellbeing and reducing health inequalities (NG44) | NICE | 2016 | https://www.nice.org.uk/guidance/ng44 | overview only |
| D16 | Impact of cooking and home food preparation interventions among adults: systematic review (Reicks et al.) | *J Nutr Educ Behav* 50(2) | 2018 | doi:10.1016/j.jneb.2017.08.004 | abstract |
| D17 | Critical review of behaviour-change techniques in cooking/food-skills interventions (Hollywood et al.) | *Crit Rev Food Sci Nutr* 58(17) | 2018 | doi:10.1080/10408398.2017.1344613 | abstract |
| D18 | Jamie's Ministry of Food: quasi-experimental evaluation, Australia (Flego et al.) | *PLoS ONE* 9(12):e114673 | 2014 | doi:10.1371/journal.pone.0114673 | abstract |
| D19 | Communities of practice to improve public health outcomes: a systematic review (Barbour et al.) | *J Knowledge Management* 22(2) | 2018 | doi:10.1108/JKM-03-2017-0111 | full; **Lead re-read the PDF abstract page** |
| D20 | Learning as peripheral participation in communities of practice (Fuller et al.) | *Br Educ Res J* 31(1) | 2005 | doi:10.1080/0141192052000310029 | abstract |
| D21 | Re-embedding situatedness: the importance of power relations in learning theory (Contu & Willmott) | *Organization Science* 14(3) | 2003 | doi:10.1287/orsc.14.3.283.15167 | abstract |
| D22 | A realist evaluation of community-based participatory research (Jagosh et al.) | *BMC Public Health* 15:725 | 2015 | doi:10.1186/s12889-015-1949-1 (PMC4520009) | full |
| D23 | Taal maakt gezonder — feiten en cijfers | Stichting Lezen en Schrijven | 2023 (V2) | lezenenschrijven.nl (PDF, see working file) | full; **primary citations not retrieved — second-hand** |
| D24 | MENE 2009–2012: visits to the natural environment — variations by social group (DATA 005) | Natural England / TNS | 2013 | nepubprod.appspot.com (see working file) | partial |

Ids `D1`, `D3`, `D4`, `D8`, `D13`, `D25` are in the working file and are not cited here.

---

## F — the revision line's retrievals (v2, 26 November 2026)

All retrieved with signed `source_read` requests (Web Bot Auth identity `dsh-research-reader`, keyid `ey9Tj49-…`). Times are UTC. **Read depth** is stated per source and is not upgraded anywhere in the note: *full* means the whole extracted text was read; where a character ceiling truncated the document, the fraction read is given.

| Id | Document | Producer / venue | Date | Identifier and URL | Retrieved (UTC) | sha256 (first 16) | Depth |
|---|---|---|---|---|---|---|---|
| **F1** | The behaviour change wheel: a new method for characterising and designing behaviour change interventions (COM-B) | Michie S, van Stralen MM & West R · *Implementation Science* 6:42 | published 23 April 2011 | doi 10.1186/1748-5908-6-42 · `implementationscience.biomedcentral.com/articles/10.1186/1748-5908-6-42` → served from `link.springer.com/…?error=cookies_not_supported` | 21:09:52 | `10c5623e031848f6` | **full text, first 30 000 of 57 204 chars** (abstract, intro, methods, COM-B definitions, framework review) |
| **F2** | Promoting planting in front gardens: a systematic approach to intervention development | Allison AL, Frost R & Murtagh N · *UCL Open: Environment* 6:e3147 | 24 May 2024 | doi 10.14324/111.444/ucloe.3147 · PMC11152043 | 21:10:09 | `fb8b67df8c8e1984` | **full text, first 25 000 of 108 577 chars** (abstract, intro, BCW/COM-B/APEASE description, methods) |
| **F3** | Celebrating variability and a call to limit systematisation: the example of the BCT Taxonomy and the Behaviour Change Wheel | Ogden J · *Health Psychology Review* 10(3):245–250 | Sept 2016 | doi 10.1080/17437199.2016.1190291 · Europe PMC `resultType=core` (PMID 27189585) | 21:10:36 | `bfcd7554069212b2` | **abstract only** |
| **F4** | Self-Determination Theory and the facilitation of intrinsic motivation, social development, and well-being | Ryan RM & Deci EL · *American Psychologist* 55(1):68–78 | January 2000 | doi 10.1037/0003-066X.55.1.68 · authors' repository `selfdeterminationtheory.org/SDT/documents/2000_RyanDeci_SDT.pdf` | 21:10:22 | `e14779081a999b49` | **full text, first 30 000 of 79 248 chars** (abstract, CET, motivation continuum, start of organismic integration theory) |
| **F5** | "To me, it's just natural to be in the garden": a multi-site investigation of new community gardener motivation using Self-Determination Theory | Sachs A, Tharrey M, Darmon N, Alaimo K, Boshara A, Beavers A & Litt J · *Wellbeing, Space and Society* 3:100088 | 2022 (available online 9 June 2022) | doi 10.1016/j.wss.2022.100088 · **publisher 403 (Cloudflare, `cf-ray a60be0c9084f23e3-AMS`)**; read from HAL-INRAE `hal-03761818v1` (author-deposited **submitted version**) | 21:10:41 | `c7a39044e7863168` | **full text, first 40 000 of 76 719 chars** (abstract, methods, results to autonomy/relatedness); version caveat: page numbers not citable |
| **F6** | Hoe gezond is stadslandbouw? Een literatuuronderzoek | Schram-Bijkerk D, Dirven-van Breemen L & Otte P (RIVM) · *Bodem* 26(1):30–31 | februari 2016 | `edepot.wur.nl/409294` | 21:11:35 | `7f709985b293fe13` | **full text, 12 000 of 15 544 chars** |
| **F7** | Groen Samenspel (ZonMw project 11010012310010) | Hecht GGD Hollands Midden, with LUMC, Leyden Academy, Gemeente Leiden, AWPG Lumens, iPH + Hogeschool Leiden, Provincie Zuid-Holland | 2024–2025 | `projecten.zonmw.nl/nl/project/groen-samenspel` | 21:11:35 | `3b55b6abcc3f1b42` | **full text** (6 537 chars) — a project record reporting its own results, i.e. **[C]** for the findings |
| **F8** | Community gardens in urban areas: a critical reflection on the extent to which they strengthen social cohesion and provide alternative food (PhD thesis) | Veen EJ · Wageningen University (Rural Sociology / WASS) | 2015 | `research.wur.nl/en/publications/community-gardens-in-urban-areas-a-critical-reflection-on-the-ext/` | 21:12:24 | `955d8ed6b359f147` | **abstract and summary read in full** (8 000 of 75 390 chars of the record page); **thesis full text not retrieved** |
| **F9** | Teach-Back in Clinical Communication: A Systematic Review and Meta-analysis | Vick JB et al. · *J Gen Intern Med* | e-published 3 Sept 2026 | doi 10.1007/s11606-026-10678-y · Europe PMC `resultType=core` (PMID 42693371) | 21:14:12 | `41ec3a6aee900d68` | **abstract only** |
| **F10** | Evaluation of a New Performance-Based Health Literacy Measurement Tool for Individuals With Chronic Airways Disease (VAHLT) | Poureslami I et al. · *Respiratory Care* 68(5):638–648 | May 2023 | doi 10.4187/respcare.10441 · Europe PMC `resultType=core` (PMID 36411057) | 21:14:24 | `0498ec6578b6bf9d` | **abstract only** (the PMC copy exists and was not read) |
| **F11** | Zo versterken voedselbossen onze gezondheid én het landschap (E. Wits; webinar with P. Martens and W. van Eck) | Platform31 | 26 oktober 2026 | `platform31.nl/artikelen/zo-versterken-voedselbossen-onze-gezondheid-en-het-landschap/` | 21:13:55 | `466ee76c3b386875` | **full text** (11 256 chars) |
| **F12** | NARCIS service notice ("Per 3 juli 2023 is de NARCIS website offline gehaald…") | DANS (KNAW/NWO) | retrieved 2026 | `narcis.nl` → `dans.knaw.nl/nl/data-diensten/narcis/` | 21:13:22 | `9131b1b8110e1a4e` | **full text** (2 440 chars) — infrastructure/access finding, not evidence of substance |
| **F13** | Correction to: Improving lifestyles sustainability through community gardening (JArDinS) | Tharrey M et al. · *BMC Public Health* 21:15 | 4 January 2021 | doi 10.1186/s12889-020-10010-1 · PMC7783970 (`fullTextXML`) | 21:12:52 | `2ce7330fb56d2fa3` | **record retrieved; the substantive change was not isolated** — [U] what it corrected; no claim rests on a number it might have touched |

**`B7` upgraded read depth in the revision.** JArDinS was re-read at **full text** via the Europe PMC `fullTextXML` endpoint (PMC7690132), retrieved 2026-11-26T21:12:35Z, sha256 `f2ec94dc7a930282…`, 139 861 chars (45 000 read inline plus the remainder extracted locally from the retrieved file). v1 had read the abstract and methods; the population, design, power calculation, measured outcomes, achieved dose, limitation section and authors' conclusions quoted in note §6.5 are from this read. **Nothing in v1's characterisation was found to be wrong; several things it could not know were found** (see [`revision-record.md`](revision-record.md) §2).

**Derivatives and near-duplicates, recorded so witnesses are not double-counted:** `F11` and the Flemish `kenniswest.be` article found in the Dutch search report the same webinar — **one source, one witness**. `F5` and `B7` derive from **the same two research cohorts** — one research programme, not independent corroboration.

---

## Repository cross-references

Cited in [`note.md`](note.md) by path rather than by id, because they are this repository's own notes rather than external sources. They are **not independent witnesses** to the literature — one retrieval each, carried through from the earlier notes.

- [`../continuity/note.md`](../continuity/note.md) — the closure, tenure and operator-concentration findings.
- [`../network/note.md`](../network/note.md) — the edge list, and Voedselbos Eindhoven's absence from Trefpunt Groen's *achterban*.
- [`../meaning/note.md`](../meaning/note.md) — the Voedselbos archive's own "open klaslokaal" and "duurzame leefstijl" framing, and the participant silence.
- [`../decisions/note.md`](../decisions/note.md) — the four decision-critical uncertainties.
- **Two sibling notes are unmerged on their own branches** at the time of writing, so they are linked at their branches: [#20 practices](https://github.com/leonvanbokhorst/voedselbos/blob/research/20-local-practices/research/practices/note.md) — the four local practices and "participation designed to be possible without being productive"; [#22 climate](https://github.com/leonvanbokhorst/voedselbos/blob/research/22-climate-adaptation/research/climate/note.md) — cited only for the climate pillar, because the *Groen Verbindt* evaluation it also reports was re-read at source for this note (`E8`) rather than inherited.
