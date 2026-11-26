# Dutch / Eindhoven local evidence line — participation instruments, datasets, and who appears in them

Working note for issue #9 ("Who is 'the community' — and how do we research with it rather than on it?").
Desk research only. All retrieval via `source_read`, public sources, no contact with anyone, no logins,
no closed groups. Retrieval date: 2026-11-26. Numbers below are computed by me from the retrieved
machine-readable export unless a line says otherwise; interpretation is marked **[I]**.

---

## 0. Headline answer

The Eindhoven instruments we can see (the greening-wishes dataset, the "groenarme buurten" project
dataset, the participation ordinance, the area-oriented subsidy scheme, and the Woensel-West community
platform) are all **producer-shaped records of participation**. They count *wishes, projects, channels and
rated involvement*. None of them records residents' own self-description in a form that would let a
researcher say who "the community" is. The most person-like thing in the largest dataset is a free-text
one-line description of a location, and in 10 of 124 records that text is literally `??`.

**[I]** Consequence for the research design: these datasets can evidence *what the municipality counted*,
not *who participated*. Any claim about the composition of "the community" has to come from either
(a) national/provincial statistics that name the selection effects (section 5), or (b) research done
*with* residents, which no public dataset substitutes for.

---

## 1. Open-data dataset "Vergroeningsprojecten" (gemeente Eindhoven) — load-bearing

### 1.1 Identity and edition

- Canonical portal page: <https://data.eindhoven.nl/explore/dataset/vergroeningsprojecten/>
- Machine-readable export used: <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroeningsprojecten/exports/json> (N2)
- Dataset metadata API: <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroeningsprojecten> (N1)
- Publisher (metadata): `Gemeente Eindhoven`. `modified` = **2026-11-20T23:01:46+00:00**; `records_count`
  declared = **124**; `license` = `null`.
- data.overheid.nl record (N4) shows: **Bijgewerkt 21-11-2026**, **Data eigenaar: Eindhoven (Gemeente)**,
  **Toegang: Beperkt**, **Licentie: Onbekende licentie**. So "updated around 21 November 2026" is confirmed
  by the national registry; the portal's own timestamp is 20 Nov 2026 23:01 UTC (= 21 Nov local).
- Same description text appears on the portal metadata AND on data.overheid.nl → **one witness, two
  renderings** (counted once below).
- A parallel ArcGIS service is listed as a related source:
  <https://gisservice.eindhoven.nl/arcgis/rest/services/GRN_Wensen_Groeninitiatieven_Extern/MapServer>
  (listed on N4; not retrieved — see access log).

### 1.2 Dataset description (verbatim, from N1 `description_nl`, corroborated by N4)

> "Deze dataset bevat wenslocaties voor vergroeningsprojecten (Wensenkaart Vergroeningsprojecten) en
> locaties van het project "Actief Ontharden en Vergroenen" als punten op de kaart."

> "**Wensenkaart Vergroeningsprojecten**
> De Wensenkaart Vergroeningsprojecten bevat wensen van omwonenden en andere betrokkenen voor het
> vergroenen van specifieke locaties. In combinatie met de andere projecten en vergroeningsacties, kunnen
> relaties gemaakt worden. Dit vermijdt het indienen van een wens bij meerdere (mede)financiers en
> medestanders, bevordert het uitvoeren van wensen, en bevordert het geven van terugkoppeling aan
> omwonenden/ betrokkenen die een idee aandragen. Iedere wens bevat gegevens als omschrijving van het
> plan/ idee en het aantal vierkante meters."

> "**Actief Ontharden en Vergroenen**
> Locaties betreft het vergroenen van overbodige en over gedimensioneerde verharde oppervlaktes in de
> openbare ruimte (van 50 tot 200 m2) aangedragen door bewoners.
> Gaat om het actief ontharden van deze locaties en middels participatie het realiseren van een nieuwe
> klimaatbestendige en biodiverse inrichting."

> "Gegevens met betrekking tot het project Vergroenen groenarme buurten zijn onderdeel van een andere
> dataset: Vergroenen groenarme buurten — Eindhoven Open Data."

The earlier pass's quoted passage (duplicate wishes to multiple financiers / "terugkoppeling") is
**verified verbatim**. Note the stated purpose is a *coordination and feedback instrument* — an
anti-duplication register, not a participation survey.

### 1.3 Field names and definitions (verbatim from N1)

| field | type | description (verbatim) |
|---|---|---|
| `locatie` | text | "(Adres omschrijving)" |
| `straatnaam` | text | — (none) |
| `stadsdeel` | text | — (none) |
| `omschrijving_plan_idee` | text | — (none) |
| `verwacht_aantal_m2_nieuw_groen` | int | "Aantal m2 die het betreft." (unit m2) |
| `datum_ingediend` | text | — (none) |
| `binnengekomen_via` | text | **"geco = gebiedscoordinator"** |
| `betrokkenheid_bewoners` | text | **"laag, redelijk, of hoge betrokkenheid"** |
| `type` | text | "Wensenkaart vergroeningsprojecten (wens), of onderdeel van project actief ontharden" |
| `status` | text | — (none) |
| `uitvoeringsjaar_gepland` | text | — (none) |
| `x_coordinaat`, `y_coordinaat`, `geo_shape`, `geo_point_2d` | numeric/geo | — (none) |

**Only one code is documented** (`geco`). The other codes that actually occur in the data
(`bewonersi`, `buitenBet`, `collega`, `anders`, `bouwteam`) have **no published definition**. Any
translation of them is inference, not documentation.

### 1.4 Computed results (my own count on N2; 124 records; cross-checked by API group-by N3)

Total records: **124** (len of export = 124; sum of status groups = 124; declared `records_count` = 124).

**Status** (`status`, N3 group-by, identical to my recount):

| status | n |
|---|---|
| "Kans of wens" | 56 |
| "Lopend" | 21 |
| "Uitgevoerd" | 20 |
| empty (null) | 16 |
| "Afgevoerd" | 9 |
| "On hold" | 2 |
| **total** | **124** |

**Intake channel** (`binnengekomen_via`):

| code | n |
|---|---|
| `geco` | 39 |
| `bewonersi` | 31 |
| empty (null) | 21 |
| `collega` | 11 |
| `anders` | 11 |
| `buitenBet` | 10 |
| `bouwteam` | 1 |
| **total** | **124** |

**Resident-involvement rating** (`betrokkenheid_bewoners`):

| value | n |
|---|---|
| empty (null) | 33 |
| `matig` | 26 |
| `redelijk` | 24 |
| `laag` | 22 |
| `hoog` | 19 |
| **total** | **124** |

**Type**: `Wens` 111, `Actief ontharden` 13.

**Planned execution year** (`uitvoeringsjaar_gepland`): **20 records have a value** —
2025: 11, 2023: 6, 2024: 3. 104 empty.

**Intake dates** (`datum_ingediend`): **90 records dated**, range **2023-05-23 → 2026-09-15**; 34 without a date.

**Stadsdeel** (data-quality note): Gestel 30, Strijp 19, Woensel Zuid 17, Centrum 17, Tongelre 14,
Stratum 12, Woensel Noord 11, empty 3, **`strijp` (lowercase) 1** — the same area appears under two
spellings, so any per-area count is off by one until cleaned.

**Crosstab `binnengekomen_via` × `status`** (for the interpretive section): `geco` records are mostly
`Lopend` (18) or `Kans of wens` (12); `bewonersi` records are mostly `Kans of wens` (24) and `Afgevoerd` (4).

### 1.5 Reconciliation with the earlier repository pass

| item | earlier pass | this pass (computed) | verdict |
|---|---|---|---|
| total records | 124 | 124 | agrees |
| status | 56 / 21 / 20 / 9 / 2 / 16 | identical | agrees |
| intake dates | 90, 23 May 2023 – 15 Sep 2026 | identical | agrees |
| "hoog" | 19 | 19 | agrees |
| unrated | 33 | 33 | agrees |
| residents / external / geco | 31 / 10 / 39 | 31 (`bewonersi`) / 10 (`buitenBet`) / 39 (`geco`) | agrees on numbers; **the labels are inferred, not documented** |
| records with planned year | 14 | **20** | **disagrees** |

The 14-vs-20 difference is fully explained arithmetically: 2023:6 + 2024:3 + 2025:11 = 20; **2024 + 2025 = 14**.
**[I]** The earlier pass most plausibly counted only future-dated years (2024–2025) and dropped the six 2023
values, or filtered on a status subset; the export itself contains 20 non-empty planned years. The 20 figure is
the one reproducible from the retrieved export.

### 1.6 What this dataset can and cannot say about WHO participates

**Can be read (established):**
- How many wish-records exist, in which stadsdeel, with what status, and when they were entered.
- The *intake channel* through which a wish entered the municipal system (`binnengekomen_via`).
- A municipal staff rating of how involved residents are (`betrokkenheid_bewoners`).
- Whether a planned execution year exists (20 of 124 — most wishes have no scheduled year).

**Cannot be read (not established by this source):**
- **No person-level record.** There is no name, no organisation, no household, no unique requester id.
  There is no field in which a resident's own words or identity appear *as such*.
- **No denominator.** 31 `bewonersi` records ≠ 31 residents: one resident or one working group can generate
  several records, and records can be merged (the stated purpose is to avoid duplicate wishes).
- **`binnengekomen_via` is an intake channel, not a self-description.** It records the route into the
  municipal system. A wish brought in by a `geco` may well originate with residents; a `bewonersi` record
  may have been typed in by staff after a phone call. **[I]** The field therefore measures *who did the
  administrative entry*, at best.
- **`betrokkenheid_bewoners` is a producer-side rating** by municipal staff / area coordinators, using an
  ordinal scale with no published rubric and no respondent. `hoog` in 19 of 124 is a staff judgement.
- `status`, `type`, `uitvoeringsjaar_gepland`, `verwacht_aantal_m2_nieuw_groen`, `stadsdeel`, coordinates are
  all administrative codings about the *location/project*, not about people.
- `omschrijving_plan_idee` is the only field carrying anything like a resident's phrasing, and it is a
  one-line summary: **10 of 124 records contain the placeholder `??`**; others are terse staff paraphrases
  ("trottoir ontharden vergroenen", "Tiny Forest", "Vergroenen van de parkeerplaatsen bij de kerk").
  It is not attributable to a speaker and cannot be quoted as a resident's voice.

**Data-protection handling:** the metadata contains **no statement** about personal data, aggregation or
privacy. There is no personal-data field, so the dataset is de facto personal-data-free at record level; but
`geo_point_2d` is address-precision and the free text is location-specific, so a record can identify a
*place* and sometimes an *organisation* (e.g. mentions of a church, a school). data.overheid.nl flags
**Toegang: Beperkt** and **Onbekende licentie**, i.e. reuse rights are not actually cleared. **[I]** Treat as
"openly downloadable, not openly licensed".

**Field-definition drift (a caution for any reuse):** the documented description of
`betrokkenheid_bewoners` says "laag, redelijk, of hoge betrokkenheid", yet the data also contains `matig`
(26 records) and 33 blanks. The codebook and the data disagree; the codebook is not maintained.

---

## 2. "Groenarm" / green-poor indicator and the Limbeek-Zuid natuurwerkgroep

### 2.1 The indicator (definition, geography, producer)

Dataset "Vergroenen groenarme buurten", <https://data.eindhoven.nl/explore/dataset/vergroenen-groenarme-buurten/> (N5, N6).
Producer: Gemeente Eindhoven; theme "Natuur en milieu"; same open-data portal.

Definition (verbatim, N5 `description_nl`):

> "Buurten met minder dan 75m² openbaar groen per woning zijn getypeerd als groenarme buurten."

So the indicator is **square metres of public green per dwelling (< 75 m²)**, i.e. a *distance/area-supply*
measure per housing unit — **not** a distance-to-green measure and **not** a measure of green quality or use.

Verbatim on selection and method:

> "Binnen het project groenarme buurten zijn negen Eindhovense buurten geselecteerd waarin de openbare ruimte
> op enkele plekken actief wordt vergroend. Op basis van ideeën van bewoners zijn er ontwerpen gemaakt om
> tegels te vervangen voor plantvakken en het verruimen van groeiplaatsen voor bomen. Met deze
> vergroeningsprojecten wordt de leefbaarheid in de buurt verbeterd. De negen geselecteerde buurten zijn:
> Bloemenplein, Gildebuurt, Hemelrijken, Joriskwartier, Lakerlopen, Limbeek-Noord, Limbeek-Zuid,
> Rochusbuurt en Tivoli."

**Limbeek-Zuid is one of the nine selected buurten** — verified in the producer's own description.

### 2.2 What the dataset contains (my count, N6)

70 records; fields: `status` ("Status van het initiatief (kan lopend of nieuw zijn)"), `locatie`,
`omschrijving`, `uitvoeringsjaar`, `nummer`, `sub_letter`, `info`, `buurt`, geo.
Status: `Lopend` 51, `Nieuw` 19. `uitvoeringsjaar`: 48 empty; values are quarter-labelled and inconsistently
formatted (`Q1 - 2024`, `Q4 2024`, `Q1 2025`, `2023, afgerond`…). Records per buurt: Hemelrijken 12, Tivoli 9,
Gildebuurt 9, **Limbeek-Zuid 7**, Bloemenplein 6, Lakerlopen 6, Joriskwartier 5, Rochusbuurt 4,
Limbeek-Noord 3, plus 7 records in buurten *outside* the nine named above (Vlokhoven 2, Kronehoef 1,
Schrijversbuurt 1, Groenewoud 1, Burghplan 1, Binnenstad 1, Vonderkwartier 1) and one `Limbeek Noord`
spelling variant. **[I]** The published description ("nine buurten") and the published data (17 buurt labels,
incl. two spellings of Limbeek-Noord) do not match; treat buurt counts as indicative only.

### 2.3 The Limbeek-Zuid natuurwerkgroep record — present, verbatim, in the dataset

Record `nummer` 5, `buurt` "Limbeek-Zuid", `status` "Nieuw", `uitvoeringsjaar` null:

> "Initiatief vanuit de natuurwerkgroep (buurtbewoners) en beheer: voormalig hondenuitlaatterrein een extra
> groene invulling geven."

This is the strongest single find of this line: the working group exists **inside the municipal dataset**, and
the municipal coding itself classifies it as a **resident initiative** ("Initiatief vanuit de
natuurwerkgroep (buurtbewoners)"). It appears once only (`natuurwerkgroep` occurs in exactly 1 of 70 records).
No person, no group name beyond the generic "natuurwerkgroep", no date, no contact.

Context records for Limbeek-Zuid (7): a whole-buurt stoeprand record (`status` Nieuw), Aletta Jacobsplein
("200m² vergroend", Q1 2024), Clara Wichmannstraat ×2 ("Gazon omvormen tot heestervak… 400m²
kwaliteitsimpuls", Q1 2024), "Stukken gras" (biodiversity layer), and "Project Actief ontharden" at Hoek
Lijmbeekstraat–Roosje Vosstraat.

**Resident vs institutional:** the record is coded as a resident initiative *by the producer*, in a
municipal project dataset that itself frames the buurt as a municipal intervention area ("negen …
geselecteerde buurten"). The dataset gives no way to tell whether the working group initiated the project or
was named as a partner afterwards. **[I]** Both readings are consistent with the text; do not overstate.

**Not established:** whether a formal "Groenarm"-*indicator* dataset exists separately from this project
dataset (I found the project/location dataset and the 75 m²/woning definition, not a stand-alone indicator
time series with its own geography and period). No Limbeek-Zuid "natuurwerkgroep" record was found in the
Vergroeningsprojecten dataset (0 hits for `Limbeek`, `werkgroep`, `natuurwerk` in that export).

---

## 3. Woensel-West community platform (woensel-west.com) as a participation instrument

### 3.1 Who runs it

- Footer of every page: "© 2026 **Stichting Woensel-West**" (N7, N8, N9, N10).
- Directory entry, verbatim (N9): "**Stichting Woensel-West** — Beheert de Buurtinfowinkel in het
  Spilcentrum Boschdijk."
- Buurtinfowinkel entry, verbatim (N9): "Heb je een vraag over Woensel-West? Loop dan gerust binnen bij de
  Buurtinfowinkel. **De Buurtinfowinkel wordt beheerd door Stichting Woensel-West en zit in het SPILcentrum
  Boschdijk aan de Wenckenbachstraat 52.** De vrijwilligers denken met je mee. Weten zij het antwoord niet?
  Dan brengen ze je in contact met de juiste organisatie."
- The site also carries a "Spilcentrum Boschdijk" entry ("Hier zitten de Buurtinfowinkel en een gymzaal die
  je kunt huren") and a "Buurtwerkkamer 360" and "KLUPhuis 70/65".
- History page (N8) places the platform in an institutional lineage, verbatim: "2009 — De Buurtonderneming
  begint. De Buurtonderneming Woensel-West gaat van start: een eigen organisatie die samen met bewoners
  activiteiten opzet en coördineert. Vanaf hier loopt bijna alles wat er in de wijk gebeurt."

**[I]** So the "community platform" is operated by a foundation that also runs the neighbourhood information
desk inside a municipal/corporation SPIL centre, and that descends from a neighbourhood enterprise set up in
the wijkvernieuwing. It is an *instrument with an institutional position*, not a neutral observer.

### 3.2 Institutional members in the directory (verbatim entries, N9)

The directory page reports: **47 results**, filter counts "Organisaties 17 / Ruimtes 15 / Buurtgroepen 9 /
Minibiebs 3 / Weggeefkasten 1 / AED 2". Named entries include:

- "**Gemeente Eindhoven**" — listed as an *Organisatie*, with **no description text**.
- "**Trudo** — Trudo verhuurt veel woningen en bedrijfsruimtes in Woensel-West. We zorgen voor het onderhoud
  van onze woningen en helpen huurders bij vragen over wonen, huur, betalingen, reparaties en overlast. We
  werken ook samen met bewoners en organisaties aan een fijne buurt. Bijvoorbeeld door sociale projecten en
  buurtactiviteiten te ondersteunen. Want een goede buurt gaat niet alleen…" (first-person corporation voice).
- "**WIJeindhoven** — Woon je in Eindhoven? En heb je (tijdelijk) ondersteuning nodig op het gebied van wonen,
  werken, ontmoeten, opvoeden, vervoer of inkomen? Neem dan contact op met WIJeindhoven."
- "**Woonbedrijf**" — listed as an *Organisatie*, **no description text**.
- Also present: Basisschool 't Palet, Korein Speelleercentrum Boschdijk, Wijk GGD, Medisch Centrum Boschdijk,
  Tante Netty, De KLUP, Stichting Woensel-West, Buurtvereniging WIJvredeoord.

So **municipality, both large housing corporations and the social district team are directory members** —
three of them with a bare name and no description. **[I]** The platform's "who is in the neighbourhood"
view is co-produced by the institutions themselves (self-registration: "Mis je jouw organisatie of plek?
Registreer jouw organisatie of locatie bij de buurtgemeenschap…").

### 3.3 Aggregation of other producers' copy

- Nieuws page (N10) has **18 results** and a category "**In de media**" (8 items) whose titles are third-party
  headlines, e.g. "Geen bos of hei voor deze wandelaars maar volksbuurten: 'Pareltjes'" (28 Sep 2026);
  "VPRO Tegenlicht: betaalbaar wonen in ruil voor vrijwilligerswerk" (18 Mar 2022); "Archined over het
  erfgoed van een krachtwijk" (15 Mar 2018).
- Retrieved item (N11): <https://woensel-west.com/nieuws/platform31-lessen-uit-de-buurtonderneming/>,
  category "In de media", byline "**Redactie Woensel-West**", body ends "**Bron: Platform31, 2023.**"
  Verbatim: "Platform31, het kennisplatform voor stad en regio, publiceerde een praktijkvoorbeeld over de
  Buurtonderneming Woensel-West. Die is sinds 2009 in de wijk actief."

**Read depth and classification:** this is a **rewritten summary with source attribution**, not a verbatim
republication and not the original. It is a **derivative witness** — one witness, not two. I did **not**
retrieve the underlying Platform31 original.

### 3.4 Are the "Verhalen" empty? — NO (correction to the earlier assumption)

The Verhalen/resident-stories feed is populated. N7/N8 list, with dates: "Bedankt Sanne!" (13 Oct 2026),
"Niemand kent Woensel-West zo goed als Arie (82), de beheerder van het buurthuis" (31 Aug 2026),
"Kindervakantieweek: bijna honderd kinderen en een wijk vol helpende handen" (19 Aug 2026, marked
*Initiatief*), "Elke week 350 kinderen bij De Klup" (27 Jun 2026), "Mo van Chomicha, de motor achter de
wijkiftar" (17 Mar 2026), "Groep 8 van 't Palet ontdekt de oorlogservhalen van de wijk" (16 May 2025),
"Studio Woensel-West: jonge makers ontdekken hun talent" (20 Mar 2025). Each is "1 min leestijd".
**So "Verhalen is empty" is false as of 2026-11-26.**

What *is* empty: the newsletter ("Er is op dit moment nog geen nieuwsbrief") and, on the Nieuws page, one
category with "Geen verhalen in deze categorie."

### 3.5 Producer claims without method (verbatim, N8)

Counter block on "Over de wijk": "**5.900** Bewoners in de wijk · **200+** Actieve vrijwilligers ·
**100+** Jaar geschiedenis · **12** Buurtinitiatieven". And verbatim: "Wat de wijk bijzonder maakt, is dat
bewoners zelf het verschil maken… De laatste jaren is er veel gebeurd: oude straten kregen een opknapbeurt en
**buurtinitiatieven schieten als paddenstoelen uit de grond**."

No definition, denominator, date or method is given for 200+ volunteers or 12 initiatives. **These are
producer claims (a foundation's self-presentation), not measurements.** The "12 Buurtinitiatieven" figure does
not match the directory's own filter counts (Buurtgroepen 9 + Organisaties 17 = 26).

---

## 4. Dutch municipal participation instruments — the formal grammar of "who speaks"

### 4.1 Verordening inwonersparticipatie Eindhoven (consolidated, in force 30-06-2026)

Source N12: <https://lokaleregelgeving.overheid.nl/CVDR706200> — header "**Geldend van 30-06-2026 t/m heden**",
with new Hoofdstuk 3 "Uitdaagrecht". Amendment proposed in N14 (raadsvoorstel, B&W 20 Jan 2026, dossier
26.04.551); the legal driver is the *Wet versterking participatie op decentraal niveau* (in force 1 Jan 2025),
which obliges municipalities to regulate the uitdaagrecht **before 1 January 2027**.

**Who may initiate — the decisive definition (Art. 1, verbatim):**

> "**inwonersparticipatie**: het op initiatief van een bestuursorgaan betrekken van inwoners, bezoekers,
> bedrijven, maatschappelijke organisaties, overheidsorganisaties of belanghebbenden bij de voorbereiding,
> uitvoering of evaluatie van gemeentelijk beleid"
> "**inwoners**: ingezetenen als bedoeld in artikel 2 van de Gemeentewet;"
> "**uitdaagrecht**: het recht van inwoners en maatschappelijke partijen om de feitelijke uitvoering van een
> gemeentelijke taak over te nemen als bedoeld in artikel 150, derde lid, van de Gemeentewet."

**[I]** This is the formal grammar the researcher needs: in Eindhoven's ordinance, "participatie" is by
definition **something a public body initiates**. Residents who act on their own initiative are not doing
"inwonersparticipatie"; they are exercising the *uitdaagrecht* (or applying for a subsidy). The two are
different legal tracks with different rights. Residency ("ingezetenen") — not ownership — is the qualification,
so **renters qualify as inwoners**.

**Art. 5 lid 1 (who may submit an uitdaagverzoek):** "Inwoners en maatschappelijke organisaties kunnen bij
burgemeester en wethouders een verzoek om toepassing van het uitdaagrecht indienen."
Art. 5 lid 3 requires the applicant to state "wat de betrokkenheid, kennis en ervaring van de indiener met de
taak is", costs, quality assurance, and "een indicatie van het draagvlak onder belanghebbenden".

**The ladder (meeweten / meedenken / meewerken / meebeslissen) — located precisely:** the four terms are
**not in the articles**; they appear in the **Toelichting** on Art. 3 lid 1 onder d ("beïnvloedingsruimte"),
verbatim:

> "Bij beïnvloedingsruimte kan in de praktijk een keuze worden gemaakt uit: meeweten, meedenken, meewerken,
> meebeslissen of een combinatie hiervan. Deze termen zijn afkomstig van het op rijksniveau ontwikkelde
> Factor C … - meeweten: de deelnemers hebben geen actieve rol, maar worden wel op de hoogte gehouden;
> - meedenken: de deelnemers leveren een bepaalde inhoudelijke inbreng; - meewerken: de deelnemers werken
> daadwerkelijk mee aan het voorbereiden, uitvoeren of evalueren van gemeentelijke beleid; - meebeslissen:
> deelnemers zijn vanuit hun rol weliswaar niet formeel bevoegd om besluiten tot nemen, maar hebben een
> doorslaggevende invloed op de besluitvorming."

So the ladder is **explanatory guidance (Factor C), not a binding norm**; the binding duty is only to *state
the beïnvloedingsruimte in advance* (Art. 3 lid 1 d). **[I]** Any claim that "Eindhoven works with the
meeweten–meebeslissen ladder" should be phrased as "the ordinance's explanatory note borrows the Factor C
ladder to describe the beïnvloedingsruimte that must be fixed in advance".

**Eight-week deadline (Art. 6 lid 5–6, verbatim):** "Het bestuursorgaan reageert binnen acht weken op het
verzoek. Het bestuursorgaan kan deze termijn met acht weken verdagen." / "Het bestuursorgaan onderbouwt de
reactie op het verzoek en maakt de reactie en de onderbouwing binnen twee weken openbaar."

**Refusal grounds (Art. 6 lid 3 — mandatory, verbatim):** "wijst het bestuursorgaan een verzoek af als:
a. het verzoek ziet op een taak waarvan de aard zich tegen toepassing van het uitdaagrecht verzet;
b. het verzoek in strijd is met door de gemeente vastgesteld beleid; c. het verzoek niet voldoet aan de in
artikel 5, derde lid gestelde eisen."
**Art. 6 lid 4 — discretionary:** "kan een verzoek afwijzen als: a. het bestuursorgaan van oordeel is dat de
taak met de toepassing van het uitdaagrecht niet beter wordt uitgevoerd of de kosten hoger zijn; b. als de
opdrachtwaarde boven de Europese drempelwaarde … uitkomt; c. als sprake is van een lopend contract voor de
uitvoering van de betreffende taak bij een externe partij".

**Exclusions (Art. 2 lid 3)** include: statutory exclusion; "uitvoering van hogere regelgeving waarbij het
bestuursorgaan geen of nauwelijks beleidsruimte heeft"; budget/taxes; urgency; and "als het belang van
inwonersparticipatie of uitdaagrecht niet opweegt tegen het belang van de verantwoordelijkheid van de
gemeente voor kwetsbare groepen in de samenleving."

**Note the trap in 6 lid 3 b + 6 lid 4 c:** "in strijd met door de gemeente vastgesteld beleid" is a
mandatory refusal ground, and an existing contract with an external party is a discretionary one.
**[I]** A residents' group challenging municipal green management runs straight into the *Beleidsregel*
(section 4.2), which forbids exactly that for medium/high-value green.

**Art. 8 Evaluatie (verbatim):** "De uitvoering van deze verordening wordt vierjaarlijks geëvalueerd.
Burgemeester en wethouders zenden na afronding van deze evaluatie aan de raad een verslag over de
doeltreffendheid en de effecten van deze verordening in de praktijk."

How the municipality will know: the Art. 8 explanatory note states it collects information "op basis van de evaluatie van individuele participatietrajecten, het afleggen van interviews met deelnemers en organisaties, het uitzetten van enquêtes of het steekproefsgewijs bekijken van dossiers waarbij inwonersparticipatie is toegepast" — i.e. the evaluative evidence base is *participants and dossiers*, the two populations that are already inside the process. **[I]** Nobody outside the process is sampled by design; absence is not measured.

### 4.2 Beleidsregel groen en water bij ruimtelijke ontwikkelingen 2026 — Art. 10 (CVDR 766778)

Source N13: <https://lokaleregelgeving.overheid.nl/CVDR766778/1> (requested the decentrale.regelgeving
`Historie/766778` URL; final URL is the canonical versioned one). Header: "**Geldend van 23-09-2026 t/m
heden**". `groenwaarde` is defined (Art. 1 onder l) as "de waarde (basis, middel of hoog) die is toegekend aan
de groenstructuur in een gebied, zoals aangewezen op de groenwaardenkaart, opgenomen in bijlage 2."

**Artikel 10. Beheer gemeentelijk groen (verbatim, in full):**

> "1. Een verzoek tot beheer van gebieden met groenwaarde basis op de groenwaardenkaart (bijlage 2) kan worden
> gehonoreerd als: a. de functie/bestemming/gebruiksdoel 'groen' behouden blijft, zoals beschreven in het
> groenbeleidsplan 2017 of diens rechtsopvolger en het omgevingsplan; en b. de afspraken worden geborgd in een
> beheerovereenkomst.
> 2. Een verzoek tot beheer van gebieden met groenwaarde middel of hoog op de groenwaardenkaart (bijlage 2)
> wordt afgewezen, behalve als: a. het gaat om overdracht van beheer aan natuur- en terreinbeherende
> instanties of partijen voor wie de groen- en natuurwaarde vooropstaat en de kwaliteit van het beheer
> aantoonbaar gewaarborgd is; en b. de functie/bestemming/gebruiksdoel 'groen' behouden blijft; en c. de
> afspraken worden geborgd in een beheerovereenkomst.
> 3. Het eerste en tweede lid van dit artikel zijn overeenkomstig van toepassing op een gelijkwaardige
> functie/bestemming/gebruiksdoel zoals 'bos' en 'natuur'."

**[I]** This is the pivotal legal asymmetry for a voedselbos/citizen green-management ambition: community
management is *possible by right* on "basis" green, and *refused by default* on "middel/hoog" green, with an
exception only for "natuur- en terreinbeherende instanties of partijen voor wie de groen- en natuurwaarde
vooropstaat" whose management quality is "aantoonbaar gewaarborgd". The test is institutional capability, not
residency or local benefit. Whether an emergent citizens' group can satisfy it is **not established** by the
text.

### 4.3 Area coordinators ("gebiedscoördinatoren" / "geco")

Established across two independent producers' texts:
- Dataset field definition (N1): "`geco` = gebiedscoordinator".
- Gemeenteblad 2026 nr. 343211 (N15), Art. 1, verbatim: "**Gebiedscommissie**: een commissie bestaande uit
  **een gebiedscoördinator aangevuld met minimaal twee professionele partners en/of bewoners**, die het college
  adviseert bij waardebonaanvragen." And: "**Professionele partners**: in het gebied werkzame instanties, die
  zich bezighouden met de leefbaarheid, zoals politie, woningcorporaties, welzijnswerk en scholen."
  Art. 8 lid 1 c obliges subsidy recipients to "desgevraagd samen met de gebiedscoördinator een tussentijdse
  evaluatie te houden".

**Not established:** I found no municipal document that *defines the gebiedscoördinator's role in the intake of
residents' wishes* (i.e. the process that produces `binnengekomen_via = geco`, 39 of 124 records). The role is
visible only as (a) an intake code, (b) a seat/chair of the waardebon advisory committee, and (c) a
co-evaluator. **[I]** That the largest single channel into the greening-wishes register is a municipal area
coordinator — not a resident — is the single most consequential finding of this line, and its procedure is
undocumented publicly.

### 4.4 Does the municipality publish an evaluation of its own participation?

- **Of the verordening: no.** Art. 8 schedules a four-yearly evaluation; the ordinance is in force since
  2024 (amended 30-06-2026), so no evaluation report can yet exist, and I found none. **Explicitly: not found.**
- **Of individual participation processes: yes, at project level, externally commissioned.** N19:
  "Stadhuisplein in samenspraak — Evaluatie van het samenspraakproces rond de ontwikkeling van het integraal
  gebiedskader Stadhuisplein", Movisie (J. Dermaux, D. de Bruijn), 22 April 2022, hosted on
  openeindhoven.nl. Verbatim: "Deze notitie is door Movisie gemaakt op verzoek van het interne projectteam
  dat verantwoordelijk was voor het samenspraakproces." It contains an internal evaluation plus external
  evaluation with klankbordgroepen, intermediairs and the gemeenteraad.
- The uitdaagrecht amendment itself came with a "Participatieverslag" (listed in N14 and found in search
  results as a bijlage; not retrieved — see access log).

### 4.5 Residents' initiative subsidy instrument: "Subsidieregeling gebiedsgericht werken in actiegebieden"

Source N15: Gemeenteblad 2026 nr. 343211, 17 juli 2026, besluit 23 juni 2026 (N15 is the PDF of the
publication). This is the current area-based instrument (waardebon + annual subsidies).

**Eligibility — who may apply (Art. 3, verbatim):** "Subsidie in het kader van deze regeling kan worden
aangevraagd door **natuurlijke- en rechtspersonen**."

**[I]** So **no legal entity, no KvK number and no bank-account requirement appears in the regeling**: a
natural person can apply. I searched the retrieved text for `KvK`, `kamer van koophandel`, `bankrekening` —
**no hits**. Caveat: the ASV Eindhoven (general subsidy ordinance) applies "in aanvulling op", and I did not
retrieve the ASV, so a general requirement there cannot be excluded → **not established**.

**Residents / tenants (Art. 1, verbatim):** "**Bewoners**: inwoners van het actiegebied die als zodanig staan
ingeschreven in de Basisregistratie Personen (BRP)"; "**Bewonersorganisatie**: een stichting of vereniging van
vrijwillige bewoners binnen het actiegebied die de belangen van de bewoners van dat gebied vertegenwoordigt".
**Tenure-neutral by construction: registration in the BRP, not ownership, defines a bewoner → renters are
eligible.** For an *organisation* the legal form is prescribed (stichting or vereniging).

**What is funded:** "**Waardebon**: een subsidie voor initiatieven voor behoud en verbetering van de
leefbaarheid in een actiegebied"; annual subsidies for buurtinfowinkel housing costs, organisation costs
(max €10.000 for a bewonersorganisatie; €500 for an ondernemersorganisatie), buurtpreventieteams, and
opstart/notary costs. **Initiatieven** must (verbatim) "geen betrekking hebben op particuliere belangen" and
"het beheer en onderhoud van de voorgestelde fysieke verbeteringen in de openbare ruimte kunnen waarborgen" —
i.e. **the scheme requires applicants to be able to guarantee maintenance of physical improvements.** That is
a capacity test that a loose group of neighbours may fail.

**Accountability / draagvlak (Art. 8 lid 1, verbatim):** for subsidies above €15.000 the recipient must
"desgevraagd samen met de gebiedscoördinator een tussentijdse evaluatie te houden…", keep materials available
to "bewonersorganisatie en initiatieven in de statistische buurt", and — decisive for "who speaks" —
"**op verzoek van het college een wijkraadpleging te houden op basis waarvan het draagvlak voor de
bewonersorganisatie of bewonersinitiatief bepaald kan worden.**"

**[I]** Representation is therefore *tested by the municipality on demand*: a funded residents' organisation
can be required to demonstrate draagvlak through a neighbourhood consultation. Legitimate voice is
institutionally conditional, not simply asserted.

**Access note:** the waardebon route runs through the **Gebiedscommissie** and a recorded **Presentatie**:
"een moment waarop bewoners, een collectief van bewoners of ondernemers hun aanvraag voor een waardebon
presenteren aan de gebiedscommissie, dat op beeld wordt opgenomen." **[I]** Applicants must perform their case
before a committee of professionals and residents, on camera — a format with real literacy and language
barriers.

---

## 5. Who is structurally absent — what national/provincial statistics can say

**These are national (or national-sample) figures, not Eindhoven-specific.** No Eindhoven-specific breakdown of
volunteering by tenure/income/migration background was found.

### 5.1 Overall volunteering

N17 (De Staat van Volksgezondheid en Zorg, kerncijfer, source CBS "Onderzoek Sociale samenhang en welzijn",
verslagjaar **2025**, last updated 26 May 2026): "**47,0 procent** van de bevolking van 15 jaar en ouder doet
vrijwilligerswerk" — defined as persons 15+ who "zich naar eigen zeggen in het afgelopen jaar ten minste één
keer heeft ingezet als vrijwilliger". Breakdowns offered: geslacht, leeftijd, opleidingstype, soort
vrijwilligerswerk (charts; **I did not extract the underlying percentages** — the page renders charts, not
tables). Regional figures come from a *different* instrument (Gezondheidsmonitor 2024, GGD'en/CBS/RIVM) and
the source itself warns "Dit kan voor een verschil in percentages zorgen."

### 5.2 Green/nature volunteering — the strongest quantified selection effect

N16: Mattijssen, de Boer, Michels & Van Wonderen (2024), *De inzet van burgers voor natuur en groen in
Nederland; Een representatieve enquête onder groene vrijwilligers*, WOT-rapport 162, Wageningen (WOT Natuur &
Milieu), november 2024, DOI 10.18174/677293, commissioned by PBL, funded by LNV.

- Headline (verbatim, Referaat): "Zo'n **34%** van de **10.779** respondenten heeft de afgelopen twaalf maanden
  vrijwillig activiteiten ondernomen voor natuur en groen." Groups: individuele vrijwilligers 22%,
  organisatie-vrijwilligers 4%, initiatief-vrijwilligers 8%, niet-vrijwilligers 66%.
- **Education (verbatim, §3.1.3):** "Mensen met een hoog opleidingsniveau zijn oververtegenwoordigd in alle
  drie de groepen vrijwilligers… **Het percentage laagopgeleiden is voor alle groepen vrijwilligers 5% en bij
  de niet-vrijwilligers 38%; voor de gehele Nederlandse bevolking is dit 26% (CBS, 2023).**"
  [I] That is a ~7× under-representation of lower-educated people among green volunteers relative to
  non-volunteers (5% vs 38%), and ~5× relative to the population (5% vs 26%). Unit: % of respondents in each
  group; period 2023–2024; producer WOT/WUR; national sample.
- **Housing/green environment (verbatim):** "Als we kijken naar de woonomgeving, dan zien we dat vrijwilligers
  vaker grotere tuinen hebben, en meer groen in hun straat." — a *garden/greenness* differential, **not** a
  tenure (owner/renter) breakdown.
- **Income (verbatim):** "Mogelijk is het inkomen een verklarende factor voor deze gevonden verbanden, dit is op
  basis van onze gegevens echter niet hard te maken."
- **Explicit non-coverage (verbatim):** "Factoren die wij niet hebben meegenomen zijn de sociaaleconomische
  achtergrond van respondenten (het inkomen of vermogen), evenals een eventuele migratieachtergrond. Op deze
  vlakken kunnen wij geen uitspraak doen over de demografie van vrijwilligers, al weten we natuurlijk wel dat
  **de enquête niet is ingevuld door mensen die de Nederlandse taal niet machtig zijn**."
- Activities (verbatim): "De meest voorkomende activiteit die vrijwilligers verrichten is het opruimen van
  afval in natuur en groen (**75%**). Ook deelname aan natuurtellingen (**27%**) en aanleg/onderhoud van
  openbaar groen (**25%**) scoren relatief hoog." — the last is the closest national proxy for
  voedselbos-type work.
- Age nuance (verbatim): "…op dat de niet-vrijwilligers in ons onderzoek gemiddeld genomen ouder zijn dan de
  mensen die wel vrijwillig actief zijn – iets wat het beeld van de 'vergrijsde' vrijwilliger in het groen toch
  wel tegenspreekt."

**So: for green volunteering, the education gradient is documented and large; a tenure (owner/renter)
breakdown is NOT available in this source; income and migration background are explicitly not measured; and
people not fluent in Dutch are structurally excluded from the survey frame itself.** Absence of a breakdown is
recorded here as a finding, not filled.

### 5.3 Self-selection in Dutch participatory processes

N18: De Bruijn & Noordewier (2023), *Ruimte voor invloed — Verkenning van mogelijkheden voor meerstemmigheid
in lokaal beleid*, Movisie, april 2023, funded by VWS.

- Verbatim (§3.4): "In de praktijk blijken bij deliberatieve vormen van inspraak **hoger opgeleiden vaak
  oververtegenwoordigd en dominerend in de discussies, ondanks loting**."
- Verbatim (§3.5 "De participatieparadox"): "Zoals we in het voorgaande hebben geconstateerd zijn **hoger
  opgeleide burgers, vaak ook met een hoger inkomen en veelal zonder migratieachtergrond, hierin
  oververtegenwoordigd**. Daarmee ontstaat er feitelijk een invloedskloof tussen verschillende groepen
  burgers."
- The report explicitly names the mechanism and the counter-image: "Het versterkt beelden dat bepaalde groepen
  – vertegenwoordigd door de 'gevestigde stemmen' – het voor het zeggen hebben."
- Directly relevant Eindhoven material inside N18: a hybrid-democracy case "Buurtbudgettraject Oud-Woensel":
  "In 2021 kon iedereen in Hemelrijken en de Gildebuurt beslissen waar het Buurtbudget van €50.000 naartoe moest
  gaan." (Two of the nine groenarme buurten — Hemelrijken and Gildebuurt — are the same neighbourhoods.)

**[I]** Note the careful wording: N18 says higher-educated residents are over-represented *despite* loting and
cites secondary literature (Voermans & Waling 2017; Driessen et al. 2018). The term "usual suspects" is **not**
used in N18 — I found no retrieved Dutch source using that exact phrase; that framing should not be attributed.

### 5.4 What is missing at city level

- No Eindhoven-specific volunteering breakdown by tenure, income, migration background or disability was found.
- No CBS/SCP breakdown of *green* volunteering by **housing tenure** was found (the WOT study measures garden
  size/greenness, not tenure).
- Disability/chronic illness: not established in any retrieved source for green volunteering.

---

## 6. Investigation and access log

| # | URL | status | outcome |
|---|---|---|---|
| 1 | data.eindhoven.nl …/vergroeningsprojecten/exports/json (v2.1) | 200 | full 124-record export, 81,786 bytes, sha256 9ba8b9b2…; used for all counts |
| 2 | …/records?select=status,count(*)&group_by=status | 200 | independent status counts; identical to my recount |
| 3 | …/records?select=count(*)&where=datum_ingediend is not null | 200 | 90 dated records confirmed via API |
| 4 | …/catalog/datasets/vergroeningsprojecten (v2.1 metadata) | 200 | field definitions + description + `modified` timestamp |
| 5 | data.overheid.nl/dataset/45600-vergroeningsprojecten | 200 | national registry: Bijgewerkt 21-11-2026, Toegang Beperkt, Onbekende licentie; lists 5 exports |
| 6 | …/catalog/datasets/vergroenen-groenarme-buurten | 200 | 75 m²/woning definition, nine buurten |
| 7 | …/vergroenen-groenarme-buurten/exports/json | 200 | 70 records; Limbeek-Zuid natuurwerkgroep record |
| 8 | decentrale.regelgeving.overheid.nl/cvdr/xhtmloutput/Historie/766778/766778_1.html | 200 → final `lokaleregelgeving.overheid.nl/CVDR766778/1` | old CVDR URL pattern redirects fine; Article 10 verbatim |
| 9 | eindhoven.raadsinformatie.nl/document/16508776/1/…Uitdaagrecht | 200 (PDF) | raadsvoorstel: policy rationale, "groenbeheer" as example, participatietraject |
| 10 | lokaleregelgeving.overheid.nl/CVDR706200 | 200 | consolidated verordening, "Geldend van 30-06-2026" |
| 11 | zoek.officielebekendmakingen.nl/gmb-2026-343211.pdf | 200 (PDF) | subsidieregeling gebiedsgericht werken, 17 juli 2026 |
| 12 | vrijwilligerswerk.nl/api/documents/downloadfile?…fileid=1753343 | 200 (PDF, 7.1 MB) | WOT-rapport 162 full text |
| 13 | staatvenz.nl/kerncijfers/vrijwilligerswerk | 200 | 47.0% (CBS 2025) |
| 14 | movisie.nl/…/Ruimte-invloed-bewoners.pdf | 200 (PDF) | participatieparadox, Oud-Woensel buurtbudget case |
| 15 | openeindhoven.nl/…Evaluatienotitie Samenspraakproces Stadhuisplein DEF_.pdf | 200 (PDF) | municipal project-level participation evaluation (Movisie 2022) |
| 16 | woensel-west.com/ (www → apex redirect) | 200 | Stichting Woensel-West footer; Verhalen populated |
| 17 | woensel-west.com/over-de-wijk/ | 200 | counters 5.900 / 200+ / 12; history |
| 18 | woensel-west.com/in-de-buurt/ | 200 | 47 results; Gemeente Eindhoven, Trudo, Woonbedrijf, WIJeindhoven, Stichting Woensel-West |
| 19 | woensel-west.com/nieuws/ | 200 | 18 results, 8 "In de media" |
| 20 | woensel-west.com/nieuws/platform31-lessen-uit-de-buurtonderneming/ | 200 | "Bron: Platform31, 2023.", byline Redactie Woensel-West |
| 21 | woensel-west.com/wp-sitemap.xml → sitemap_index.xml; post-sitemap.xml | 200 (XML) | used to obtain exact post URLs instead of guessing |
| 22 | **publicaties.eindhoven.nl/…/participatie-niveau_20260108.pdf.pdf** | **404** | **FAILED** — municipal document on participation "niveau" (8 Jan 2026) is gone at that URL; no alternative found in the time available. Would have been the best candidate for a municipal definition of participation levels/gebiedscoördinatie. |
| 23 | gisservice.eindhoven.nl/arcgis/rest/services/GRN_Wensen_Groeninitiatieven_Extern/MapServer | not retrieved | listed as related source on N4; not needed since the ODS export was machine-readable |
| 24 | lokaleregelgeving.overheid.nl/zoeken?q=…&aanbieder=Eindhoven | 200 but no results | the search endpoint needs POST/other params; worked around by web search → direct CVDR ids |
| 25 | Participatieverslag Uitdaagrecht (bijlage bij N14) | not retrieved | listed in search results (document/16508777); would document which organisations/residents were consulted on the amendment |
| 26 | ASV Eindhoven (general subsidy ordinance) | not retrieved | needed to fully exclude a KvK/bank-account requirement |

No robots.txt exclusion was relied upon for any source in this note; no source was behind a login, paywall or
Cloudflare challenge. No 403s encountered. One 404 (row 22). No personal data was collected; no closed
Facebook/WhatsApp group was accessed or sought. Two sources listed in search results but not retrieved are
flagged above rather than cited.

**Witness discipline:** the Vergroeningsprojecten description is one witness appearing twice (portal metadata +
national registry); the Woensel-West Platform31 item is a *derivative summary* of a Platform31 original I did
not read; the 47.0% figure is CBS data republished by Staat VenZ (one witness, quoted at second hand); the WOT
education figures are primary survey results (one witness).

---

## 7. What is not established

1. The **definition of `bewonersi`, `buitenBet`, `collega`, `anders`, `bouwteam`** — only `geco` is
   documented. The mapping "bewonersi = inwoner/resident" is an inference from the token, not a published
   definition.
2. **Who actually typed any given record** and whether residents self-submitted or staff transcribed.
3. Any **count of unique residents, households or initiatives** behind the 124 records.
4. The **procedure by which a `geco` enters a wish** and how a resident reaches a geco.
5. Whether a **stand-alone "Groenarm" indicator dataset** (with its own geography/period) exists beyond the
   "Vergroenen groenarme buurten" project dataset and the 75 m²/woning definition.
6. Whether the **Limbeek-Zuid natuurwerkgroep initiated** its project or was named as a partner; whether it
   still exists; its size, name or composition.
7. Whether an **evaluation of the Verordening inwonersparticipatie** exists (Art. 8 schedules it four-yearly;
   none found).
8. Whether the **ASV Eindhoven** adds a KvK/bank-account requirement to the gebiedsgericht subsidy.
9. Any **Eindhoven-specific breakdown** of participation by tenure, income, migration background, disability.
10. Any CBS/SCP **green-volunteering breakdown by housing tenure** (national).
11. The contents of the **Participatieverslag Uitdaagrecht** (who was consulted).
12. Whether "**de usual suspects**" appears as a term in any retrievable Dutch source — not found; do not attribute.

## 8. What would change the answer

- A municipal *process* document defining `binnengekomen_via` codes and the geco intake route (would move §1.6
  from inference to fact).
- The ASV Eindhoven text (would settle the legal-entity question in §4.5).
- A CBS/SCP table cross-tabulating volunteering with **housing tenure** (would fill the biggest gap in §5).
- The Participatieverslag Uitvoeringsregeling Uitdaagrecht (would show which residents were heard while the
  ordinance was written).
- Any WOO/openbaarheid request for the Wensenkaart back-office (would give requester identity — but that is
  personal data and would itself raise the research-ethics question this issue is about).

## 9. Adjacent questions noticed, not researched

- De Wielewaal estate management arrangements (who holds the beheerovereenkomst under Art. 10 of the
  Beleidsregel — "natuur- en terreinbeherende instanties").
- Whether Wasven/Bij Albrecht/Phood hold any of the 39 `geco` records.
- The "Actief Ontharden" programme's own participation method (13 records here; the Eindhovenduurzaam page was
  linked from the dataset description but not retrieved).
- Stadsdeel-level budget allocations (wijkbudget) vs the gebiedsgericht subsidy.

---

## 10. Sources (ids, metadata, read depth)

All retrieved 2026-11-26 via `source_read`; sha256 as reported by the tool.

- **N1** — *Vergroeningsprojecten* (dataset metadata, API v2.1). Producer: Gemeente Eindhoven. Edition:
  `modified` 2026-11-20T23:01:46+00:00, `records_count` 124, `license` null.
  URL <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroeningsprojecten>; retrieved
  2026-11-26T22:03:19Z; sha256 `891c96673e5166514111e3eb107f5a7acbf8a7bc00abaaf7891ae1e188cd501d`;
  read depth: **full metadata + all field definitions** (14,612 bytes; first 12,000 chars inline + spill).
- **N2** — *Vergroeningsprojecten* (machine-readable JSON export, all records). Publisher: Gemeente
  Eindhoven. URL <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroeningsprojecten/exports/json>;
  retrieved 2026-11-26T22:03:06Z; sha256 `9ba8b9b25af0bfc21b7a99a152a9e574c0afb0ba5edf79701a0eb0d47e3fa5fb`;
  **full text** (81,786 bytes; parsed locally, 124 records).
- **N3** — *Vergroeningsprojecten* status group-by (API aggregation). URL
  <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroeningsprojecten/records?select=status%2C%20count(*)%20as%20n&group_by=status&limit=100>;
  retrieved 2026-11-26T22:03:10Z; sha256 `85fcd9a2b304657bf6ac3a6fb0ae5e27c487c7c8278e05bba4c3b37591a1b342`;
  **full text** (225 bytes).
- **N4** — *Vergroeningsprojecten* (national open-data registry record). Producer: data.overheid.nl /
  Gemeente Eindhoven. Edition: "Bijgewerkt 21-11-2026". URL <https://data.overheid.nl/dataset/45600-vergroeningsprojecten>;
  retrieved 2026-11-26T22:03:19Z; sha256 `f8cb586f0cb05f7f36f17d3f851c58fca206d8bae5d992f7a70f8ccba14c6e34`;
  read depth: **full text** (50,374 bytes HTML → 6,009 chars).
- **N5** — *Vergroenen groenarme buurten* (dataset metadata). Producer: Gemeente Eindhoven.
  URL <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroenen-groenarme-buurten>;
  retrieved 2026-11-26T22:03:25Z; sha256 `e9f40f7007ea1e4752e651c0e5c4c835bb0058f8bcaf912525afc23acc5c4f57`;
  read depth: **full metadata + field definitions** (11,243 bytes).
- **N6** — *Vergroenen groenarme buurten* (JSON export). URL
  <https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroenen-groenarme-buurten/exports/json>;
  retrieved 2026-11-26T22:03:28Z; sha256 `ea2cfc76e575dfac7ae325d68bcbbe84254a62dd27056f977c82b636577c37d2`;
  **full text** (32,523 bytes; 70 records parsed).
- **N7** — *Home – Woensel-West*. Producer: Stichting Woensel-West. URL <https://woensel-west.com/>
  (requested www., redirected to apex); retrieved 2026-11-26T22:03:29Z; sha256
  `bf5b3a164d04f528cca462c06b37ff08bf82773510e8605bbc95c926fe7c4a6a`; **full text** (4,081 chars).
- **N8** — *Over de wijk – Woensel-West*. URL <https://woensel-west.com/over-de-wijk/>; retrieved
  2026-11-26T22:03:35Z; sha256 `275352155680c0c689f557f8371fa90c5fc454487363af8b0334826567202433`;
  **full text** (9,447 chars).
- **N9** — *In de buurt – Woensel-West* (directory, 47 results). URL <https://woensel-west.com/in-de-buurt/>;
  retrieved 2026-11-26T22:03:39Z; sha256 `458b71796aab1f3faa21abf1ba51174bbc3b52d4f330817f08e01268137a311d`;
  **full text** (8,508 chars).
- **N10** — *Nieuws – Woensel-West* (18 results, 8 "In de media"). URL <https://woensel-west.com/nieuws/>;
  retrieved 2026-11-26T22:04:55Z; sha256 `1848a7163d8fa6c7afdde48d025c6457390dd5b40ddc44cc6fd1ff84169ff82f`;
  **full text** (4,573 chars).
- **N11** — *Platform31 beschrijft de lessen uit de Buurtonderneming*. Producer: Redactie Woensel-West
  (derivative of Platform31, 2023). URL
  <https://woensel-west.com/nieuws/platform31-lessen-uit-de-buurtonderneming/>; retrieved 2026-11-26T22:05:10Z;
  sha256 `9582e0adfc9c25529f4e4fb54d757affe9ff52d63fd910adefdbdb3d13b4f43c`; **full text** (3,494 chars).
- **N12** — *Verordening inwonersparticipatie Eindhoven*, CVDR 706200, "Geldend van 30-06-2026 t/m heden".
  Producer: gemeente Eindhoven (raad). URL <https://lokaleregelgeving.overheid.nl/CVDR706200>; retrieved
  2026-11-26T22:04:05Z; sha256 `e42637cfee1c0a4c36f92e44796a919781fb5b37379399c4aab2ecc110cd2da6`;
  read depth: **full text** (49,964 chars; articles + toelichting consulted).
- **N13** — *Beleidsregel groen en water bij ruimtelijke ontwikkelingen gemeente Eindhoven 2026*, CVDR 766778,
  "Geldend van 23-09-2026 t/m heden". Producer: college van B&W Eindhoven.
  URL <https://lokaleregelgeving.overheid.nl/CVDR766778/1> (via decentrale.regelgeving redirect); retrieved
  2026-11-26T22:03:51Z; sha256 `3f21a3f49595b04f769187e2b3a5f8e25e38b277a9898263f7c07b0e86f3582f`;
  read depth: **full text** (108,375 chars; Art. 1, 10, 11 and definitions read in full).
- **N14** — *Raadsvoorstel Uitbreiding Verordening inwonersparticipatie Eindhoven met Uitdaagrecht*
  (Inboeknummer 8107621_02, dossier 26.04.551, B&W 20-01-2026). Producer: gemeente Eindhoven.
  URL <https://eindhoven.raadsinformatie.nl/document/16508776/1/8107621_02+Raadsvoorstel+Uitbreiding+Verordening+inwonersparticipatie+Eindhoven+met+Uitdaagrecht>;
  retrieved 2026-11-26T22:03:52Z; sha256 `f772b709692c05d8cdd2ab15df6bd8d2d9d4310c213608da09c6a21359abd468`;
  read depth: **substantial PDF text** (26,359 chars; first 6,000 read inline).
- **N15** — *Subsidieregeling gebiedsgericht werken in actiegebieden gemeente Eindhoven*, Gemeenteblad 2026
  nr. 343211, 17 juli 2026. Producer: college van B&W Eindhoven (besluit 23-06-2026).
  URL <https://zoek.officielebekendmakingen.nl/gmb-2026-343211.pdf>; retrieved 2026-11-26T22:04:17Z;
  sha256 `80f6c3d27af3a286123289beed6dcadd21912f43300e9fc0695db8966adc427b`;
  read depth: **full text** (14,468 chars).
- **N16** — Mattijssen, T.J.M., de Boer, T.A., Michels, R., van Wonderen, D. (2024). *De inzet van burgers
  voor natuur en groen in Nederland; Een representatieve enquête onder groene vrijwilligers*. WOT-rapport 162,
  Wageningen (WOT Natuur & Milieu), november 2024, DOI 10.18174/677293, n=10.779.
  URL <https://vrijwilligerswerk.nl/api/documents/downloadfile?sectionid=165830&fileid=1753343&forcedownload=true>;
  retrieved 2026-11-26T22:04:42Z; sha256 `0591b27ebd66350ac73a3f655a820bf5d8c68af6d39866627a621b878745cafe`;
  read depth: **full text** (411,613 chars; §3.1.3, §5.1, §8.7, §9 and referaat read).
- **N17** — *Vrijwilligerswerk* (kerncijfer). Producer: De Staat van Volksgezondheid en Zorg (CBS-bron:
  Onderzoek Sociale samenhang en welzijn), verslagjaar 2025, update 26-05-2026.
  URL <https://www.staatvenz.nl/kerncijfers/vrijwilligerswerk>; retrieved 2026-11-26T22:04:44Z;
  sha256 `7c30ccc453c528bed874c1afda3c5cce624c907c059825a4496f2e74c6a27638`;
  read depth: **full text** (3,556 chars; **chart values not extracted**).
- **N18** — De Bruijn, D. & Noordewier, Y. (2023). *Ruimte voor invloed — Verkenning van mogelijkheden voor
  meerstemmigheid in lokaal beleid*. Movisie, april 2023 (financiering VWS).
  URL <https://www.movisie.nl/sites/movisie.nl/files/2023-05/Ruimte-invloed-bewoners.pdf>; retrieved
  2026-11-26T22:04:48Z; sha256 `dfea0c11b01eef880d3608691b3e605ff88110da5587a07bfa5622bd78f37d7b`;
  read depth: **full text** (124,760 chars; §3.4, §3.5, Oud-Woensel case read).
- **N19** — Dermaux, J. & de Bruijn, D. (2022). *Stadhuisplein in samenspraak — Evaluatie van het
  samenspraakproces rond de ontwikkeling van het integraal gebiedskader Stadhuisplein*. Movisie, 22 april 2022,
  in opdracht van gemeente Eindhoven.
  URL <https://www.openeindhoven.nl/sites/default/files/2022-10/20220408%20Evaluatienotitie%20Samenspraakproces%20Stadhuisplein%20DEF_.pdf>;
  retrieved 2026-11-26T22:05:10Z; sha256 `0363587ddd139ddd9fc48b00a6a2730be4be9fd487116532b8d9a20a202a85a1`;
  read depth: **partial** (109,351 chars; colofon, inhoudsopgave, §1 read; findings sections not read).
- **N20** — *sitemap_index.xml* / *post-sitemap.xml*, woensel-west.com (used only to obtain exact post URLs).
  Retrieved 2026-11-26T22:04:59Z and 22:05:07Z; sha256 `c86fb9883a940ddc1459decbbfda10037118577dde67689e37256e414155c6fc` and
  `e53ee7038a22e3b742058b8919557ebfb992c47beb345b5807a6074bccec0cc2`; read depth: **full** (technical).

**Failed / not retrieved:** `https://publicaties.eindhoven.nl/sites/default/files/genetics/participatie-niveau_20260108.pdf.pdf`
(HTTP **404**, retrieved 2026-11-26T22:05:07Z, sha256 `3513ab6936f61c0f0ae5134396eda194716a4ecaf1621c3a22385fea0a52ddd3`);
Participatieverslag Uitdaagrecht; ASV Eindhoven; ArcGIS GRN_Wensen_Groeninitiatieven_Extern service.
