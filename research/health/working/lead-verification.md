# Lead verification — the issue brief's own starting points, re-read

Raw material for [`../note.md`](../note.md), not evidence in itself. All retrievals 2026-11-26 with signed `source_read` requests (Web Bot Auth identity `dsh-research-reader`, keyid `ey9Tj49-…`); times are UTC. Marks: **[D]** documented in the retrieved source, **[C]** claimed by an actor, **[I]** inference, **[U]** not established. sha256 prefixes identify the exact representation retrieved.

The purpose of this file is narrow: to check, at the primary page, the four documented starting points the issue brief hands the researcher — because a note built on someone else's untested quotation inherits its errors. It is not a summary of those sources.

---

## 1. DE STAP naar gezonder — the partner count is 193, not 189

| Item | Value |
|---|---|
| URL | `https://www.destapnaargezonder.nl/over-de-stap/` (canonical; no redirect) |
| Status | 200, `text/html`, 188 049 bytes |
| sha256 | `7d367ff659236e11e1efaeb9ea44c8148bf9cf81ca94805bfcf32764e82ffa03` |
| Retrieved | 2026-11-26T20:29:37Z |
| Read depth | full page text (3 259 chars extracted) |

**What the page says.** [D]

> "DE STAP naar gezonder is meer dan een website. Het is de naam van een beweging die zich richt op het verbeteren van de gezondheid in de regio Eindhoven en De Kempen. Aan de beweging nemen inmiddels **193 organisaties** ('partners') deel. Dit zijn bijvoorbeeld huisartsengroepen, gemeenten en zorg- en welzijnsinstellingen, maar ook zorgverzekeraars, bedrijven en onderwijsinstellingen."

**Correction to the issue brief.** The brief states "189 partner organisations in Eindhoven and De Kempen at retrieval on 26 November 2026". On 26 November 2026, 20:29 UTC, the page reads **193**. The brief's figure is therefore stale by four partners, or was read on another date, or came from another page. The direction of the error is not important; the lesson is: **the count moves, so the count cannot carry an argument**. Treat 193 as the number read today and as a self-report of a movement's participants, not as an independent count of active organisations, and not as evidence that any one of them does anything.

**Two things the page establishes for the note.** [D]

1. The movement's unit of participation is *organisations* — "huisartsengroepen, gemeenten en zorg- en welzijnsinstellingen … zorgverzekeraars, bedrijven en onderwijsinstellingen". A volunteer garden is not in that list of categories, and the direction of fit is organisation → movement.
2. The website's own promise is **self-service without a gatekeeper**: "tips, activiteiten en handige hulpmiddelen waarmee je direct aan de slag kunt, zonder dat je daarvoor eerst naar je huisarts, je zorgverzekeraar of een andere plek hoeft. Het gebruik van de website is helemaal gratis. Wel tonen we soms activiteiten of andere hulpmiddelen waarvoor een (kleine) financiële bijdrage gevraagd wordt." That is a *signposting* claim: it routes people to existing activities. Nothing on the page claims to run, fund, train for or evaluate any of them.
3. The six domains are confirmed on this page as site navigation: *Gezond en fit · Mentaal sterk · Zinvol leven · Kwaliteit van leven · Contact met anderen · Voor jezelf zorgen*. Note that **"leren" is not a domain** and no domain names knowledge, literacy or skills.

No legal form, no founding date, no governance and no budget appear on this page. That gap is pursued by the delegated regional line, not here. **[U]** in this file.

---

## 2. The Eindhoven directory — gardens are filed under "Ontmoeten", and that is the finding

| Item | Value |
|---|---|
| URL | `https://www.destapnaargezonder.nl/eindhoven/` |
| Status | 200, `text/html`, 601 078 bytes |
| sha256 | `1ab60cb1d1910d11fbcff8eecf1fd86c8ef77ff2e54d79d3cf683c49b4b27fa4` |
| Retrieved | 2026-11-26T20:29:51Z |
| Read depth | full page text (11 780 chars extracted); the activity list as rendered |

**What the page promises.** [D]

> "Ga aan de slag met je gezondheid vanuit je eigen wijk of buurt. … Kijk hieronder waar je gebruik van kunt maken. Zonder dat je daarvoor eerst naar je huisarts, de gemeente of je zorgverzekeraar hoeft te gaan. Leuk en gezond. En meestal gratis."

**Inventory of the rendered list, 26 November 2026.** [D for the rendering; the page has filter facets and this is the list as loaded, not a guaranteed complete catalogue]

| Category label | Entries |
|---|---|
| Ontmoeten | 52 |
| Hulp en advies | 47 |
| Bewegen en sporten | 26 |
| Creatief aan de slag | 10 |
| Klussen | 4 |
| Training en coaching | 4 |
| Bijeenkomst | 3 |
| Website | 1 |
| **Total rendered** | **147** |

Counted by exact category label in the retrieved text. A sibling count of the "Doe mee" call-to-action buttons gives 135, the difference being entries whose link reads "Lees meer"; the category count is the better estimate of entries and is the one used here.

**Every green or food activity in that rendered list**, with its own category label [D]:

| Entry | Category | Stadsdeel |
|---|---|---|
| Buurtmoestuin Irisbuurt | **Ontmoeten** | Stratum |
| De Vergeten Tuin | **Ontmoeten** | Gestel |
| Buurttuin (unspecified) | **Ontmoeten** | — |
| Adopteer een stukje groen | Klussen | — |
| Wandelen met IVN | Bewegen en sporten | Meerdere gemeenten |
| Samen koken in het kookatelier · Samen koken en eten (×2) · Samen eten · Soep koken · Open soep · Samen aan tafel bij de Buurtkeuken · Kookclub voor mannen · Koekjes bakken | **Ontmoeten** (all) | various |
| Troep Troepers: samen troep opruimen | Ontmoeten | — |

**Three observations, each marked.** 

- **[D]** No entry in the rendered Eindhoven directory is categorised as health education, health literacy, learning about health, or prevention. The green and food entries sit under *Ontmoeten* (meeting people) or *Klussen* (odd jobs). "De Vergeten Tuin" — the 25-year-old residents' garden that has its own beheerovereenkomst with the municipality and appears in issue #20's research — is filed as a place to meet people.
- **[D]** The directory is dominated by company and company-like offers: walking groups, walking football, jeu de boules, chair exercise, repair cafés, language help, debt help, coffee mornings. Of 147 rendered entries, 9 are food/cooking and 4 are growing/green.
- **[I]** Being listed is co-presence in a signposting instrument, not a relationship, a partnership, or a collaboration. It tells you that somebody submitted an entry and it was accepted; it tells you nothing about who runs the activity, whether it is current, or whether the movement and the garden have ever spoken. That distinction is the same one this repository already drew for Voedselbos Eindhoven's Trefpunt Groen relations.

---

## 3. Buurtmoestuin Irisbuurt — 63 words, no time, no cost, no organiser

| Item | Value |
|---|---|
| URL | `https://www.destapnaargezonder.nl/buurtmoestuin-irisbuurt/` |
| Status | 200, `text/html`, 193 212 bytes |
| sha256 | `d9e6a4d213e338e1c0e814205aface58e708aaa5f1cb1a1d3050330f81d338ff` |
| Retrieved | 2026-11-26T20:29:40Z |
| Read depth | full page text (2 304 chars extracted) |

The whole substance of the entry [D]:

> "**Buurtmoestuin Irisbuurt** — Ontmoeten · Eindhoven · Stratum
> De moestuin in de Irisbuurt is een groene plek in Eindhoven. Kom eens langs! Je kunt meehelpen in de tuin, anderen ontmoeten of gewoon even genieten van deze rustige plek midden in de stad. In de zomer zijn er geregeld activiteiten. Iedereen is welkom.
> Bekijk de Iristuin op Facebook"

What the entry **does not** contain: opening times, address, cost, contact person, organiser's name, legal form, whether plots are available, whether food is harvested and shared, whether anything is taught, or any date. The only outbound route is a Facebook page. [D for the absences]

**Reading.** [I] On the movement's own platform, the garden is presented as a *place to be* rather than a *thing to do*, with the weakest possible commitment signal ("kom eens langs", "iedereen is welkom", "gewoon even genieten"). That is consistent with what issue #20 found about participation being "designed to be possible without being productive" — but it also means the listing supplies no evidence of any learning offer, and cannot be used to support a claim that the movement already connects gardens to health literacy. The garden's own practice, schedule and reach are **[U]** from this source and would need its own site or the Facebook page.

---

## 4. 't Kruidenkafe Kalmoesplein — "kruiden" is in the name only

| Item | Value |
|---|---|
| URL | `https://www.destapnaargezonder.nl/t-kruidenkafe-kalmoesplein/` |
| Status | 200, `text/html`, 197 759 bytes |
| sha256 | `0080e86cc6d831c3e39b6ab01e47c0075ec6bf78ff74cd2cf213aa90a62b8b33` |
| Retrieved | 2026-11-26T20:29:40Z |
| Read depth | full page text (2 534 chars extracted) |

> "'t Kruidenkafe Kalmoesplein — Ontmoeten · Eindhoven · Stratum
> Zin om te ontspannen met klankschalen of Tai Chi? Of om creatief aan de slag te gaan? Wil je rondstruinen in de pop-up kledingwinkel? Of doe je liever mee met een yogales of Arabische aerobicsles? Het kan allemaal in 't Kruidenkafe in Stratum. Houd Facebook in de gaten voor de activiteiten.
> Wanneer: Maandag 9.00 – 15.00 uur | dinsdag 9.00 – 15.00 uur | donderdag 9.30 – 15.00 uur en vrijdag 9.00 – 15.00 uur
> Waar: 't Kruidenkafe, Kalmoesplein 70, Eindhoven" [D]

**Verdict on the brief's cautious phrasing.** The issue brief says the Kruidenkafé is "a social and wellbeing venue, not established as a garden". That is **confirmed and should be stated more strongly**: what is documented is sound bowls, tai chi, yoga, Arabic aerobics, a pop-up clothing shop, four fixed opening blocks per week, and a Facebook page for the programme. **No growing, no herb cultivation, no garden, no food activity and no health education appears in the listing.** [D]

**Why it still matters to this note.** [I] It is the clearest local example of the naming trap the issue warns about: a place called a *herb café* that a keyword search will return as a herb garden, and that a plausible argument would then cite as evidence of herb-growing practice in Eindhoven. "Kruidenkafe" names a social venue in Stratum. Anyone claiming a herb-growing site here has to produce a source that is not this page.

---

## 5. Fontys — the 2023 article, checked; and the CoE Health page in 2026

### 5.1 The 9 June 2023 news article

| Item | Value |
|---|---|
| URL | `https://www.fontys.nl/nieuws/zo-zetten-fontys-en-jij-de-stap-naar-gezonder/` |
| Status | 200, `text/html`, 170 009 bytes |
| sha256 | `e3f0e9cb79d84f9070415a89fdb6ba97db0a44b29d037f1183b1463a61003967` |
| Retrieved | 2026-11-26T20:29:44Z |
| Read depth | full article text (8 162 chars extracted) |
| Byline / date | Koos de Bie · **09 juni 2023, 10:38 Europe/Amsterdam** [D] |

Confirmed claims in the brief [D], with the wording that matters:

- "**Fontys is vanaf het allereerste uur betrokken bij DE STAP.**" Attributed to Janienke Sturm, described as "**lector Mens & Technologie, kartrekker Centre of Expertise Health en lid van de partnerraad DE STAP**".
- "**Fontys is binnen DE STAP eigenaar van de bouwsteen 'lerend vermogen'**, om ervoor te zorgen dat we samen ook leren van wat we doen. Het Centre of Expertise Health en het Fontys-programmateam brengen daarin onderzoek, onderwijs en praktijkbevindingen samen."
- "In het Fontys-programma DE STAP werken studenten bijvoorbeeld in **Professionele Werkplaatsen in Tongelre, De Achtse Barrier en Son en Breugel** samen met inwoners en professionals aan het **verkleinen van gezondheidsverschillen in de wijk**."

Two things the brief did not cite, both worth having:

- **The dated partner count for comparison:** "Aan die beweging doen inmiddels **meer dan 95 organisaties** in de regio mee" (June 2023) → **193** (26 November 2026). The movement has roughly doubled its partner count in three and a half years. That is growth in *signatories*, and it says nothing about activity.
- **The movement's headline target, as Fontys states it:** "Zodat iedereen in Brainportregio **in 2030 drie (!) jaar extra in goede gezondheid leeft**, want dat is het doel van DE STAP." [C — an ambition reported by a partner]. Three additional healthy-life years is a population-level outcome with a 2030 date; whether any baseline, monitoring design or attribution exists for it is **[U]** in this file and belongs to the delegated regional line.

Note on the neighbourhoods: **Tongelre** and **De Achtse Barrier** are Eindhoven *stadsdelen* with a documented concentration of health disadvantage; that the professional learning workplaces sit there is [D] for the location and [I] for the targeting rationale.

### 5.2 The Centre of Expertise Health page, as it stands in 2026

| Item | Value |
|---|---|
| URL | `https://www.fontys.nl/Onderzoek/Gezonde-en-inclusieve-samenleving-1/Centre-of-expertise-Health.htm` |
| Status | 200, `text/html`, 163 740 bytes |
| sha256 | `e6c9e60793830029f22abb695bac096e00c21d4609eefe64788af88fc8df0586` |
| Retrieved | 2026-11-26T20:30:08Z |
| Read depth | full page text (15 807 chars extracted) |

The brief's claim that the Centre "explicitly combines health literacy, healthy physical and social environments, and future shared care" is **confirmed verbatim** [D]:

> "Met praktijkgericht onderzoek en innovatie richten we ons binnen het Centre of Expertise Health op drie thema's: **gezondheidsvaardigheden, gezonde fysieke en sociale leefomgeving en samenzorg voor de toekomst**."

On the health-literacy theme specifically [D]:

> "Om een eerlijke kans te hebben op een gezond leven, is het een voorwaarde dat je in staat bent om voor je eigen gezondheid te zorgen. Dat is niet voor iedereen vanzelfsprekend. … We kijken in de eerste plaats naar informatievaardigheden en digitale vaardigheden met betrekking tot gezondheidsonderwerpen. Daarnaast kijken we naar de rol van (toekomstige) professionals daarin en de (cultuur)sensitiviteit in hun werkzaamheden. Daarbij zetten wij sterk in op **inclusief onderzoek en co-creatie met gebruikers met lage gezondheidsvaardigheden**."

On the green environment theme [D] — this is the closest thing to a green–health research line found anywhere in the repository's region:

> "Een gezonde leefomgeving draagt direct bij aan gelijke kansen op gezondheid en het terugdringen van gezondheidsverschillen. Dat gaat bijvoorbeeld over schonere lucht en **een groene omgeving**, maar over een goede sociale en financiële omgeving …"
> listed documents under this theme: "**Groene stedelijke leefomgeving** — Onderzoek naar de vraag: wat is het effect van een groene stedelijke omgeving op de gezondheid?" · "**Hittestress in steden** …" · "**Gezonde voedselomgeving** — Een menukaart voor een omgeving waarin de gezonde voedselkeuze ook de makkelijke, logische en aantrekkelijke is."

**Governance, which the brief did not have** [D]:

> "Het Centre of Expertise Health is een publiek-private samenwerking met in het bestuur **Slimmer Leven, Pharos, GGD-BZO, Transvorm, Fontys Mens en Gezondheid en Fontys Paramedisch**."

and, currently, on DE STAP:

> "**DE STAP naar gezonder** — Fontys is partner in DE STAP naar gezonder, het regioplatform gericht op positieve gezondheid en preventie."

plus networks "**Coalitie Vitaal in Brainport**" and "**Alliantie Gezondheidsvaardigheden**", and "Het gedachtegoed van Positieve Gezondheid vormt een belangrijke basis voor het Centre of Expertise Health."

**Three consequences for this note.**

1. **[D]** The 2023 involvement is **not** a dead letter: the CoE Health page in 2026 still lists DE STAP partnership. That answers the brief's "verify what is still active in 2026; do not assume that the 2023 governance remains unchanged" — the *partnership* is current; the 2023 *governance description* is what has drifted (see 3).
2. **[D]** Pharos — the Dutch health-literacy knowledge institute whose factsheet the brief cites — and GGD-BZO are **on the board** of the same Centre. So the region's health-literacy expertise is not a distant literature; it is one governance step from the university of applied sciences that owns DE STAP's "lerend vermogen" workstream. Whether any of them has ever engaged a community food initiative is **[U]** — and that absence is the honest answer to "what opportunities already exist".
3. **[C→D on role drift]** Sturm's public role has narrowed between sources: "kartrekker Centre of Expertise Health" (2023) vs "Lector Mens en Technologie" and the named contact for "Ook samen onderzoek doen?" (2026 CoE page). Both are Fontys pages and may simply be different hats. Recorded as a dating problem, not as a contradiction.

**What this file cannot do.** It cannot tell you whether DE STAP has ever evaluated anything, who owns it, what "partnership" obliges a partner to do, or whether any garden in Eindhoven has ever been invited into it. Those are the delegated regional line's questions.

---

## 6. The *Groen Verbindt* evaluation — read at source rather than inherited

| Item | Value |
|---|---|
| URL | `https://www.verwey-jonker.nl/wp-content/uploads/2020/07/315009_Groen_verbindt_zorg_en_de_buurt_WEB-2.pdf` |
| Status | 200, `application/pdf`, 5 718 979 bytes |
| sha256 | `4cffe46428cb9c60b774dabad87a0ef889c2d1f8739644b1db6f3de15ebe693e` |
| Retrieved | 2026-11-26T20:41:18Z |
| Document | Van der Klein, Wilderink & Reches (Verwey-Jonker Instituut), *Groen verbindt zorg en de buurt. Van storming naar performing in een stimuleringsprogramma, 2015-2018*, mei 2019, for the Oranje Fonds |
| Read depth | full text retrieved (358 720 chars); summary figures and the education paragraph read directly |

**Why read it.** The sibling report for issue #22 cites this evaluation for three figures this note depends on. Rather than inherit them, I re-read the report — and the inherited summary was slightly wider than its source.

**What the report says** [D], verbatim from the summary of year-on-year results on the volunteer questionnaire:

> "• Ik heb het afgelopen jaar nieuwe mensen leren kennen in de buurt: **elk jaar door 9 op de 10 deelnemers** bevestigd."
> "• Sinds het afgelopen jaar sta ik eerder voor andere mensen klaar: elk jaar door **5 op de 10** deelnemers bevestigd."
> "• Sinds het afgelopen jaar **durf ik meer mensen om hulp te vragen**: elk jaar door **4 op de 10** deelnemers bevestigd."

And, on the background characteristics [D]:

> "De vrijwilligers bij de tuinen zijn redelijk hoogopgeleid. **Ongeveer de helft van de vrijwilligers heeft een universitaire opleiding of een opleiding in het hoger beroepsonderwijs** afgerond; en bij de buurtbewoners is dat **ruim een derde**."

One further figure worth recording because it is a self-attribution and should not be read as an effect [C]:

> "Ongeveer 80% van de respondenten wijt hun voortgang op sociale contacten, geluk en gezondheid aan hun deelname."

**What this changes.** Two things. (1) The inherited "eight to nine in ten" is **9 in 10** for the new-contacts statement — a small tightening. (2) The report contains a **gradient** the earlier summary flattened: 9 in 10 meet new people, 5 in 10 say they stand ready for others, **4 in 10** dare ask for help. That gradient — giving rises, asking does not — is the empirical basis for this note's H3, and it is stronger than a single "4 in 10" figure on its own.

**What it does not change.** The earlier note's qualification still holds: this is a volunteer self-report survey in a funded stimulation programme (2015–2018), with no comparison group, and the 80% attribution is exactly the kind of statement the repository treats as **[C]**.
