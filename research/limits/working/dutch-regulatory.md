# Dutch and Eindhoven municipal instruments that constrain activity in green space

**Question (bounded).** What do Dutch and Eindhoven municipal public sources document about the legal and policy instruments that constrain human activity, access, events, foraging, tree work and small-scale green initiatives in and around Eindhoven? Eight named sub-questions: SMP, natuurpuntenkaart, Omgevingswet/omgevingsplan/APV, Natura 2000, NNB, municipal green policy, carrying capacity, Groene Woud/Regiodeal.

**Line.** One of two independent lines. No subagents were spawned. No person or organisation was contacted. No `git` command was run. This is not legal advice: it records what public instruments say, at the level needed to know what constrains activity. I do not assess whether any specific initiative would be permitted.

**Retrieval date.** All sources retrieved 2026-11-26 (UTC). Read-depth marks: **FT** = full text retrieved and read; **FT-part** = full text retrieved but only part read/grepped; **ABS** = landing page only; **SNIP** = search snippet only.

**Robots.txt.** I did **not** rely on the robots.txt exception for any source in this report. Every source below was retrieved through ordinary public HTTP with the signed retrieval identity; no control was challenged, and no access boundary was bypassed.

**Method note on a label.** SOURCE → EVIDENCE → INTERPRETATION are kept distinct. Sentences marked *Interpretation* are mine and are not in the sources.

---

## Access log

| Target | Status / failure | Class | Recovery attempted | Outcome |
|---|---|---|---|---|
| `raadsinformatie.eindhoven.nl/document/15539396/2/…Collegebrief SMP` | 200, PDF, 12,458 chars | — | — | **FT** (`N1`) |
| `smpcheck.nl/gemeente/eindhoven` | 200, HTML | — | — | **FT** (`N2`), third-party aggregator |
| `raadsinformatie.eindhoven.nl/document/13615815/1?connection_type=16&connection_id=902797` (2022 "Soortmanagementplan gebouwbewoonende soorten Eindhoven en Geldrop", bijlage 13) | `Error: the connection was aborted before the body completed` (twice: http and https, with and without params) | Transient / unknown | Re-requested twice (scheme and parameter variant) | **Not retrieved.** Content unknown; only a search snippet (`SNIP`) |
| `brabant.nl/.../natuurdoelanalyse_leenderbos_groote_heide_amp_de_plateux.pdf` and `.../n2000_beheerplan_leenderbos_groote_heide_en_de_plateaux_2021.pdf` | `connection aborted before the body completed` on every attempt | Transient / size / unknown | Direct request ×3 (incl. a reduced `maxChars` variant) + 1 Wayback attempt | **Not retrieved** — the beheerplan's recreation/`verstoring` passage is therefore **unavailable** |
| `eindhovenduurzaam.nl/natuurpuntenkaart` | 200, HTML | — | — | **FT** (`N4`) |
| `eindhovenduurzaam.nl/…/DT_Biodiversiteits verslag_2862024.pdf` (Plan van aanpak biodiversiteit) | 200, PDF, 96,398 chars | — | — | **FT** (`N3`), large parts read/grepped |
| `lokaleregelgeving.overheid.nl/CVDR766778/1` | 200, HTML, 108,375 chars (truncated at 100k) | — | — | **FT-part** (`N7`); omitted tail is Bijlage 1 tables |
| `lokaleregelgeving.overheid.nl/CVDR415534/18` (APV) | 200, HTML, 162,623 chars | — | — | **FT** (`N5`); key articles read verbatim from spill |
| `lokaleregelgeving.overheid.nl/CVDR762747/2` (Verordening bomen 2026) | 200, HTML, 40,968 chars | — | — | **FT** (`N8`) |
| `lokaleregelgeving.overheid.nl/CVDR719903/1` (Verordening bomen 2024) | 200, HTML, 17,341 chars | — | — | **FT** (`N9`) |
| `lokaleregelgeving.overheid.nl/CVDR657211/1` — the CVDR id named in our brief | 200 — resolves to **Verordening bomen 2021**, `Regeling vervallen per 18-05-2024` | — | Checked the id as given | **FT** (`N10`); **the brief's id is a superseded instrument** |
| `zoek.officielebekendmakingen.nl/prb-2025-13146.html` (Omgevingsverordening Noord-Brabant) | 200, HTML, 1,132,004 chars, read first 200,000 | — | — | **FT-part** (`N11`); NNB arts. 5.30–5.34 read verbatim |
| `zoek.officielebekendmakingen.nl/stcrt-2026-2565.pdf` (aanwijzingsbesluit Leenderbos) | 200, PDF, 232,315 chars | — | — | **FT-part** (`N12`); grepped in full |
| `publicaties.eindhoven.nl/…/B14_Voortoets_0.pdf` | 200, PDF, 363,823 chars, read first 100k | — | — | **FT-part** (`N13`) |
| `eindhoven.nl/…/Definitief rapport Monitoren druk en dynamiek in Genneper Parken.pdf` | 200, PDF, 65,878 chars | — | — | **FT** (`N14`) |
| `raadsinformatie.eindhoven.nl/document/15711867/1/…Besluit aanwijzing gebieden aanlijnplicht honden 2025` | 200, PDF | — | — | **FT** (`N6`) |
| `raadsinformatie.eindhoven.nl/document/14638368/1/24bst01157 Raadsvoorstel Omgevingsvisie` | 200, PDF | — | — | **FT** (`N15`) — the *voorstel*, not the Omgevingsvisie itself |

No Cloudflare challenge, paywall, login or CAPTCHA was encountered. Both failure families are connection-level aborts at the origin, not access controls.

---

## Instrument by instrument

### 1. Soortenmanagementplan (SMP) Eindhoven

**Exists? No — not yet. A plan is being prepared; no area-based exemption is in force.** Both a municipal council letter and an independent status register agree, with a date conflict noted below.

The council letter (`N1`, FT) states the legal frame and the third-party use:

> "In Eindhoven komen beschermde diersoorten voor. Alle vleermuissoorten en veel vogelsoorten zijn beschermd. Het is op grond van de Omgevingswet niet toegestaan om beschermde dieren te verstoren of te doden. De provincie is hiervoor het bevoegd gezag."

> "Op basis van een SMP kan een gebiedsgerichte omgevingsvergunning Flora en Fauna bij provincie Noord-Brabant worden aangevraagd. Deze vergunning kan, naast gemeente, ook door derden (particulieren en organisaties) worden gebruikt om zonder ecologisch onderzoek en zonder vergunning te isoleren en te (ver)bouwen. Dit kan omdat het (ecologisch) onderzoek al door de gemeente is gedaan."
> *(Gloss: an area-based flora-and-fauna permit can be applied for at the province; it can be used by third parties — private persons and organisations — to insulate and to build/renovate without their own ecological survey or permit.)*

What the document covers and how it is scoped:

> "Het SMP beschrijft waar populaties beschermde diersoorten aanwezig zijn, hoe deze worden beschermd en hoe wordt geborgd dat werkzaamheden niet leiden tot het verstoring of sterfte. Afhankelijk van de omstandigheden kan wel aanvullend onderzoek nodig zijn of moeten er maatregelen getroffen worden om verblijfplaatsen die verdwijnen te compenseren."

> "Het SMP is ingestoken om in een bepaald gebied voor bepaalde werkzaamheden van particuliere activiteiten (zoals spouwmuurisolatie en verbouwingen) een vergunning te verkrijgen. Het SMP is nog in ontwikkeling en de werkzaamheden die er onder gaan vallen zijn nog niet volledig ingekaderd."

**The 2027 timeline in our brief is confirmed, in the municipality's own words:**

> "Eindhoven is bezig met het opstellen van een SMP. De planning is dat medio juli 2027 het SMP wordt opgeleverd en vergunning bij provincie Noord-Brabant kan worden aangevraagd. Verwachting is dat we in de loop van het derde kwartaal 2027 met het SMP kunnen werken. Een SMP kent een geldigheidsduur van 10 jaar."

> "Het opstellen van een SMP neemt zo’n drie jaar in beslag."

Project steps (`N1`, FT, table): Definitiefase Jan–Mar 2025; Ontwerpfase Apr–Jun 2025; **Uitvoeringsfase (ecologisch onderzoek) Jul 2025 – Okt 2026**; **Realisatiefase (maken SMP, krijgen vergunning) Aug 2026 – Sep 2027**; **Nazorgfase Sep 2027 – Dec 2037**.

Budget (`N1`, FT): "In de begroting 2025 is voor het opstellen SMP en bijkomende maatregelen een bedrag van € 1.500.000 opgenomen", with a provincial subsidy request totalling € 832.549.

Species groups named in `N1`: four bat species (gewone dwergvleermuis, laatvlieger, baardvleermuis, gewone grootoorvleermuis), plus "veel vogelsoorten" generally; the NVI route compensates "alternatieve verblijfplaatsen voor vier soorten vleermuizen". **Which area** the SMP covers is *not* stated in `N1`: only "in een bepaald gebied" — **not established**.

Independent register (`N2`, FT, third party — Ecosprong/SMPcheck, not the municipality):

> "In voorbereiding … Er is nog geen gebiedsgerichte vergunning verleend; doorgaans loopt er meerjarig ecologisch (veld)onderzoek."

> "18 september 2026 Status: SMP in voorbereiding / eind 2027 SMP verwacht"; "Ecologisch bureau: EcoGroen"; "Bevoegd gezag Provincie Noord-Brabant (Gedeputeerde Staten)"; "Uitvoering Omgevingsdienst Zuidoost-Brabant"; "Laatst gecontroleerd op actualiteit: 11 oktober 2026".

**Tension 1 (date).** `N1` (13 May 2025) expects to *work with* the SMP in Q3 2027; `N2` (checked 11 Oct 2026) says "eind 2027". Both put the instrument after mid-2027; they differ by roughly a quarter. Recorded, not reconciled.

**Tension 2 (status of the national insulation route).** `N1`: "De landelijke aanpak geldt voor maximaal drie jaar", with a 6% cap "verdeeld over de looptijd van medio 2024 tot medio 2027: 3% voor 2024/2025, 2% voor 2025/2026 en 1% voor 2026/2027". `N2`: "De landelijke werkwijze om zonder SMP te isoleren is in 2025 gestopt." These are not compatible as stated. `N2` is a secondary aggregator; `N1` is the municipality. **Not established** which is correct; the primary national instrument was not retrieved.

**Tension 3 (an earlier SMP-like document).** A search result (`SNIP`, unretrieved) describes "Soortmanagementplan gebouwbewoonende soorten Eindhoven en Geldrop (bijlage 13)" as drawn up "In 2022", on `raadsinformatie.eindhoven.nl/document/13615815/1`. I could not retrieve that document (two connection aborts). Possible readings — an ecological annex to a specific project, or an earlier joint initiative — cannot be distinguished without the file. `N1`'s "Eindhoven is bezig met het opstellen van een SMP" (2025) is not necessarily contradicted by a 2022 document, but the relationship is **not established**.

**What it constrains in practice.** *Interpretation.* For green space, essentially nothing directly. The SMP is scoped to building-related private works (insulation, renovation, construction) and its payoff is the removal of a survey burden for those works. It creates no rule about walking, dogs, events, foraging, planting or tree work in parks. What *does* bear on green space is the underlying norm `N1` states — protected animals may not be disturbed or killed, province as bevoegd gezag — which applies to hedge cutting, mowing and tree work independently of the SMP. Note also what an SMP *obliges*: compensation for lost roosts is a municipal duty in the NVI track ("Gemeente moet alternatieve verblijfplaatsen realiseren"), discharged in Eindhoven ahead of the 1 May 2025 deadline for 80% and 1 April 2026 for 100% (`N1`, FT).

**Not established.** The SMP document itself; its exact area; its final species list; whether a *gebiedsgerichte vrijstelling* (as opposed to a *vergunning*) is the intended instrument — `N1` says "gebiedsgerichte omgevingsvergunning Flora en Fauna", not a vrijstelling; any provincial register entry; and whether any part of a future SMP would cover green-space (as opposed to building) works.

### 2. Natuurpuntenkaart

**Producer: the municipality, with Sweco; method: a "natuurpuntencalculator"; unit: score per buurt (neighbourhood)** — not per hectare, and with no threshold attached.

`N4` (FT, municipal page):

> "Om er achter te komen hoe het zit met de biodiversiteit in Eindhoven hebben we natuurpuntenkaarten laten maken in samenwerking met adviesbureau Sweco. Op deze kaarten is per buurt te zien hoe het ervoor staat met de biodiversiteit."

> "Het aantal natuurpunten in Eindhoven is berekend met de natuurpuntencalculator. Dit is gedaan met de informatie die nu beschikbaar is, zoals verschillende kaarten en waarnemingen van planten en dieren. Eerst is het natuurtype voor heel Eindhoven vastgesteld. Daarna is per gebied gekeken welke planten en dieren aanwezig zijn, omdat deze informatie iets zegt over de kwaliteit van het natuurtype."

> "In de komende jaren worden er nieuwe berekeningen gemaakt van natuurpunten."

The design intent and baseline date are in the biodiversity plan (`N3`, FT):

> "Dit kan met een natuurpuntensysteem waarbij gebruik wordt gemaakt van genoemde monitoringsgegevens (database) en van bestaande GIS data zoals bijvoorbeeld de buurtindeling. Buurten krijgen een score, met als resultaat eenvoudig te interpreteren kaarten die met elkaar vergeleken kunnen worden." … "Doel: eerste natuurpuntenkaart (nulmeting) in H1 2024."

The score is layered on a separate, older monitoring series (`N3`, FT, Bijlage 1): "Om de natuurwaarden in de gemeente Eindhoven te kunnen monitoren zijn in 2009 veldonderzoeken gestart voor een structurele monitoring", with quality classes "van 0 tot 5, waarbij 0 de hoogste natuurwaarde weergeeft en 5 de laagste", across "22 natuurdoeltypen en 5 landschapsdoeltypen".

**Distinguishing the two things.** *Interpretation.* "Natuurpunten" here is a **municipal communication and monitoring index for Eindhoven, produced by Sweco on a municipal commission, scored per buurt**. I found **no** provincial Noord-Brabant "natuurpunten methodiek" in the retrieved record, and no indication that Eindhoven's calculator is the provincial method. A Rijkswaterstaat publication titled "pilot natuurpunten als kpi voor biodiversiteit" appeared in search results but was **not read** (`SNIP` only) and is not relied on.

**Is the underlying map or dataset public? Not established.** The municipal page describes the maps and their purpose but the retrieved text contains no dataset or map link, no GIS service, and no downloadable file. Repeated calculation is announced for "de komende jaren" without a publication channel.

**What it constrains.** *Interpretation.* Nothing. It is a measurement and communication instrument with no norm, no threshold and no legal consequence attached in any retrieved source. Crucially, **it is not a carrying-capacity measure**: it scores biodiversity state per neighbourhood, not visitor load.

### 3. Omgevingswet, omgevingsplan and the APV

Two structural facts first. The Omgevingsvisie is expressly non-binding (`N15`, FT): "Het is een richtinggevend document voor de gemeente, maar niet juridisch bindend voor de inwoners." And the municipal green rules operate through a *tijdelijke* omgevingsplan made of the old bestemmingsplannen (`N7`, FT, toelichting): "De bestemmingsplannen zijn van rechtswege zijn overgegaan in het tijdelijke deel van het omgevingsplan gemeente Eindhoven."

**The single most consequential APV article for green-space activity is art. 2:45** (`N5`, FT, APV Eindhoven, `Geldend van 26-09-2025 t/m heden`):

> "Artikel 2:45 Betreden van plantsoenen en dergelijke
> 1. Het is verboden zonder ontheffing van het college zich te bevinden in of op bij de gemeente in onderhoud zijnde parken, wandelplaatsen, plantsoenen, groenstroken, grasperken of buiten de daarin gelegen wegen of paden.
> 2. Het verbod is niet van toepassing voor zover in opdracht van een bestuursorgaan of openbaar lichaam werkzaamheden worden verricht."
> *(Gloss: being in municipal parks, walks, plantings, green strips or lawns — or off the paths within them — is prohibited without a college exemption; the exemption-free carve-out is for work commissioned by a public body.)*

**Dogs** — art. 2:57(1) (`N5`, FT):

> "b. binnen de bebouwde kom op een openbare plaats indien de hond fysiek niet is aangelijnd;
> c. buiten de bebouwde kom op een door burgemeester en wethouders aangewezen plaats indien de hond niet fysiek is aangelijnd"

The designation is real and recent (`N6`, FT, B&W 20 June 2025, "Aanwijzing gebieden aanlijnplicht honden 2025"):

> "De navolgende gebieden aan te wijzen als gebieden waar het elke dag van de week, gedurende de gehele dag verboden is om honden te laten lopen zonder dat deze fysiek aangelijnd te zijn: … **B. Landgoed de Wielewaal; begrensd door de Oirschotsedijk, de Elburglaan, de Tilburgseweg en de Anthony Fokkerweg**;"

Eight areas are designated (A Klotputten; B Wielewaal; C ecologische verbindingszone Ekkersrijt; D Boktse Beemden; E Wandelpark Eckart (partly); F Eisenhowerlaan–spoor; G Urkhoven; H weidevogelterrein Gijzenrooi), on the stated ground that "Om de biodiversiteit in een aantal gebieden te beschermen dit wel noodzakelijk wordt geacht". *Interpretation:* De Wielewaal — pillar 1 of our brief — is a year-round, all-day leash area. That is a documented, enforceable constraint on the estate's most common public use.

**Smoking and fire in nature** — art. 2:18(1) (`N5`, FT):

> "Het is verboden in bossen, op heide- of veengronden of binnen een afstand van dertig meter daarvan: a. te roken gedurende de periode 1 januari tot en met 31 december; b. voor zover het de open lucht betreft, brandende of smeulende voorwerpen te laten vallen, weg te werpen of te laten liggen."

Note the wording: the smoking ban runs **all year**, not only in a fire-risk season — unlike the model APV. And art. 5:34(1)–(2) (`N5`, FT):

> "1. Het is verboden in de openlucht afvalstoffen te verbranden … of anderszins vuur aan te leggen, te stoken of te hebben.
> 2. Het verbod is niet van toepassing op: … b. sfeervuren zoals terrashaarden en vuurkorven, indien geen afvalstoffen worden verbrand; c. vuur voor koken, bakken en braden, mits er geen sprake is van gevaar, overlast, hinder voor of schade aan de omgeving."

Lid 3 allows B&W to grant an ontheffing; lid 4 allows nadere regels "voor het aanleggen van vuren en het gebruik van verlichting als bedoeld in het lid 2".

**Events** — art. 2:25(1) and 2:25(3)(d) (`N5`, FT):

> "1. Het is verboden zonder vergunning van de burgemeester een evenement te organiseren."
> "3. Daarnaast kan de burgemeester een evenementenvergunning weigeren indien: … d. de aard van het evenement zich niet verdraagt met het karakter of de bestemming van de gevraagde locatie of het evenement niet voldoet aan het locatieprofiel dat het college voor die locatie heeft vastgesteld."

So **locatieprofielen** exist as an instrument in the APV text. **No locatieprofiel document was retrieved** (see §Searched and not found). Decision term is 16 weeks (art. 2:25a).

**Other use of public space and green.** Art. 2:10(1) (`N5`, FT): "Het is verboden zonder vergunning van burgemeester en wethouders de weg anders te gebruiken dan overeenkomstig de publieke functie daarvan." Art. 1:1 defines "weg" to include "voor het publiek toegankelijke … parken, plantsoenen, speelweiden, bossen en andere natuurterreinen". Art. 5:11(1) prohibits driving a vehicle "door een park of plantsoen of een van gemeentewege aangelegde beplanting of groenstrook", and art. 5:33(1) lets B&W restrict motor vehicles, bicycles and horses in designated public nature areas, parks and plantsoenen at designated times, with an ontheffing in lid 4.

**Trees are *not* in the APV.** Art. 4:10 (Begripsbepaling), 4:11 (Omgevingsvergunning voor het vellen van houtopstanden) and 4:12 are all marked **"[gereserveerd]"** in the current consolidated text (`N5`, FT). Tree work is governed by the separate Verordening bomen — see §6.

**Wild animals, bees, pigeons**: art. 2:61 (Wilde dieren), 2:62 (Loslopend vee), 2:63 (Duiven), 2:64 (Bijen) are all **"[gereserveerd]"** (`N5`, FT). Noise: art. 4:6(1) prohibits operating equipment or performing acts outside an inrichting "dat voor een omwonende of voor de omgeving geluidshinder wordt veroorzaakt", with an ontheffing in lid 2.

**Not established in the APV.** No article on picking/plucking/harvesting plants or produce (full-text search of the consolidated APV for *pluk*, *oogst*, *gewassen* returned only art. 2:15 "Hinderlijke beplanting" and art. 5:11). No article on drones or unmanned aircraft (search for *drone*, *onbemand*, *luchtvaartuig* returned nothing). No article restricting lighting in public green beyond the festiviteiten/verlichting provisions of afdeling 4.1 and art. 4:16 lichtreclame ("[gereserveerd]"); art. 2:21 concerns the duty to tolerate public-lighting provisions on one's building, not park lighting.

### 4. Natura 2000 in and near Noord-Brabant

**A Natura 2000 area lies partly *inside* the municipality of Eindhoven.** `N12` (FT-part, aanwijzingsbesluit new text, Stcrt. 2026, 2565, 26 Jan 2026):

> "Het Natura 2000-gebied Leenderbos, Groote Heide & De Plateaux ligt in de provincie Noord-Brabant en behoort tot het grondgebied van de gemeenten Bergeijk, Cranendonck, Eersel, **Eindhoven**, Geldrop-Mierlo, Heeze-Leende, Valkenswaard, Veldhoven en Waalre."

Same document: "landelijk gebiedsnummer 136"; Vogelrichtlijngebied known to the Commission as "NL3009014"; the two special protection zones were merged into one Natura 2000 area by the 4 July 2013 designation.

Distances from a point inside the city (Philips Stadion, Frederiklaan 10A, within the Ring) are documented in a 2026 voortoets (`N13`, FT-part, Kragten, 9 Oct 2026, annex to ontwerp-omgevingsvergunning EHV-DP2026-173548):

| Natura 2000-gebied | Afstand excl. mobiliteitshubs (ca. km) | incl. hubs (ca. km) |
|---|---|---|
| Leenderbos, Groote Heide & De Plateaux | 4,7 | 1,6 |
| Strabrechtse Heide & Beuven | 7,8 | 6,1 |
| Kempenland-West | 9,8 | 5,8 |
| Hageven met Dommelvallei e.a. (België) | 15,6 | 11,9 |
| Kampina & Oisterwijkse Vennen | 17,1 | 11,7 |
| Weerter- en Budelerbergen & Ringselven | 19,0 | 15,7 |
| Groote Peel | 24,1 | 22,1 |

**Nitrogen sensitivity.** The same voortoets records calculated increases of at most "0,02 mol N/ha/jaar" (2027), 0,01 in later years, for Leenderbos, Strabrechtse Heide & Beuven and Kempenland-West, and states the pressure logic in one sentence:

> "Vanwege de ligging van het projectgebied en de mobiliteitshubs van meer dan 1 km ten opzichte van de relevante Natura 2000-gebieden zoals weergegeven in paragraaf 2.2 en de uitwerking van storingsfactoren opgenomen in bijlage B2 kunnen alleen significante effecten als gevolg van verzuring vanwege atmosferische stikstofdepositie mogelijk optreden als gevolg van het project. Buiten deze aspecten zijn op voorhand geen andere effecten te verwachten voor de Natura 2000-gebieden."

It also notes generally: "In de aanlegfase is verder vooral sprake van verstoring door geluid, licht, trillingen etc."

**Recreation and `verstoring` as a documented pressure: NOT ESTABLISHED.** The provincial *beheerplan* (2021) and *natuurdoelanalyse* for Leenderbos, Groote Heide & De Plateaux could not be retrieved (three connection aborts, including a Wayback attempt — see Access log). A case-insensitive search of the full pdftotext extraction of the aanwijzingsbesluit (232,315 characters, 3,740 lines) returned **no occurrence** of "recreatie" or "verstor"; because the decision is an objectives-and-boundary instrument and parts of its tables extract imperfectly, I do **not** treat that as proof of absence. What I can say: *no retrieved Natura 2000 document states recreation or visitor pressure as a knelpunt for these sites.*

**What it constrains in practice.** *Interpretation.* Inside a Natura 2000 area the constraint is the area-protection regime itself (a Natura 2000-activiteit vergunning where significant effects are possible); outside it, the practical route is nitrogen, and at 0,02 mol margins the voortoets shows how small a project's calculated contribution can be while still requiring an ecological assessment. Recreation as such is not the pressure these documents regulate; **nitrogen is**.

### 5. Provinciaal Natuurnetwerk Brabant (NNB)

**NNB is a provincial instruction to the municipal omgevingsplan, not a rule addressed to visitors or to activity.** `N11` (FT-part, Omgevingsverordening Noord-Brabant, Provinciaal blad 2025, 13146, published 11 Aug 2025), Afdeling 5.2.5:

> "Artikel 5.30 Bescherming Natuur Netwerk Brabant
> 1. Een omgevingsplan van toepassing op Natuur Netwerk Brabant:
> a. strekt tot het behoud, herstel of de duurzame ontwikkeling van de ecologische waarden en kenmerken;
> b. bevat regels gericht op de bescherming van de ecologische waarden en kenmerken en houdt daarbij ook rekening met andere aanwezige waarden en kenmerken, zoals rust, stilte, cultuurhistorische waarden en kenmerken; en
> c. staat alleen bestaande bebouwing en bestaande gebruiksactiviteiten toe zolang het Natuur Netwerk Brabant niet is gerealiseerd."

> "Artikel 5.31 Externe werking Natuur Netwerk Brabant
> 1. Een omgevingsplan dat een ontwikkeling toelaat in Stedelijk Gebied of in Landelijk Gebied, die een aantasting geeft van de ecologische waarden en kenmerken in het Natuur Netwerk Brabant, bepaalt in aanvulling op het Besluit activiteiten leefomgeving dat de negatieve effecten waar mogelijk worden beperkt en de overblijvende, negatieve effecten worden gecompenseerd, overeenkomstig artikel 5.37 Compensatie."

The one provision that speaks to small structures and recreation is art. 5.33(1):

> "Een omgevingsplan ter plaatse van Natuur Netwerk Brabant kan, in afwijking van Artikel 5.8, eerste lid, onder a, bepalen dat het is toegestaan kleinschalige bebouwing en bouwwerken ten behoeve van de natuurfunctie of het recreatieve medegebruik op te richten, als dat geen aantasting geeft van de ecologische waarden en kenmerken van het Natuur Netwerk Brabant."

with lid 3: any "verstoring of tijdelijke verstoring" that does occur must be limited where possible and the remainder compensated under art. 5.37. Art. 5.32(2) excludes Natura 2000 from the maatwerk route. Art. 5.34 sets out the "Nee, tenzij"-principle: groot openbaar belang, no alternative location outside NNB, no other solution, limiting, and compensation.

**Is Eindhoven inside/adjacent?** Established only indirectly and negatively. `N3` (FT): "Rondom de stad liggen (landbouw)gronden die niet horen bij het Natuurnetwerk Brabant en die beheerd worden door de gemeente Eindhoven (Stadsbeheer)." *Interpretation:* the municipal landholding around the city is characterised in that plan as **outside** NNB — i.e. the city is adjacent to NNB, and municipal farmland is not itself NNB. A definitive NNB boundary map for Eindhoven was **not retrieved** (a `publicaties.eindhoven.nl` "kaartaanpassingen NNB" document appeared in search results but was not read).

The municipal green beleidsregel states the relationship plainly (`N7`, FT, toelichting): "Buiten stedelijk gebied is op grond van de provinciale Omgevingsverordening Noord Brabant sprake gebieden die zijn aangewezen als ‘Landelijk gebied’ of ‘Natuur Netwerk Brabant’. Hiervoor gelden provinciale (instructie)regels zoals gesteld in de Omgevingsverordening Noord-Brabant. De groenopgave geldt niet bovenop deze provinciale regeling."

Adjacent instrument: stiltegebied. Art. 5.28 requires the omgevingsplan to preserve "stilte en rust"; art. 5.29(b) sets, for an Attentiezone stiltegebied, "een grenswaarde van 50 dB(A) LAeq, 24 uur, op 1,5 m hoogte, op de grens van het Stiltegebied" for events. Which Eindhoven-area stiltegebieden exist was **not established**.

### 6. Municipal green policy

**6a. Beleidsregel groen en water bij ruimtelijke ontwikkelingen gemeente Eindhoven 2026** (`N7`, FT-part, CVDR766778, `Geldend van 23-09-2026 t/m heden`).

Its reach is wider than "ruimtelijke ontwikkelingen", and that matters here — art. 3(1):

> "1. Deze beleidsregel is van toepassing: a. binnen het gehele grondgebied van de gemeente Eindhoven; **b. bij aanvragen voor beheer van gemeentelijk groen door derden**; c. bij aanvragen tot verkoop of pacht van gemeentegrond met de bestemming of functie/gebruiksdoel ‘groen’, of gelijkwaardig daaraan, of; d. bij ruimtelijke ontwikkelingen; e. bij aantasting van beschermd of aanwezig groen …"

*Interpretation:* an initiative that asks to *manage* municipal green, or to buy or lease municipal green ground, is expressly inside this beleidsregel — before any question of a "ruimtelijke ontwikkeling" arises. That is the closest thing in the retrieved record to a route-and-test for a community green initiative on municipal land.

Definitions that decide what is protected (art. 1): "beschermd groen: openbaar groen in eigendom van de Gemeente Eindhoven, of groen in eigendom van derden met de bestemming of functie/gebruiksdoel ‘groen’, of gelijkwaardig daaraan zoals ‘bos’ en ‘natuur’"; and "aanwezig groen: groen dat niet valt onder ‘beschermd groen’ maar dat aanwezig was op peildatum juli 2024".

Numeric norms, with unit and denominator:

> "5. Per toegevoegde woning wordt ter waarde van 8 m2 nieuw groen toegevoegd." (art. 4(5))
> "6. Voor elke niet-woning wordt ter waarde van 10% van het BVO aan nieuw groen toegevoegd." (art. 4(6))
> "3. De bijdrage voor het jaar 2026 is €236 per niet gerealiseerde m2 van de groenopgave." (art. 7(3))
> "2. In de groene wiggen is het invullen van de groenopgave en/of groencompensatie met een bijdrage aan het groencompensatiefonds niet toegestaan." (art. 7(2))

Green wedges are defined as "groene wig Genneper Parken, groene wig De Karpen en groene wig Brainport park" (art. 1(j)). The plan's legal anchor is stated in the toelichting: "Op 18 augustus 2024 is de Europese Natuurherstelverordening in werking getreden. Hier staat onder andere dat de stedelijke groene ruimte niet af mag nemen tot 2031."

**6b. Verordening bomen** — the brief's CVDR id is out of date. `CVDR657211` is the **Verordening bomen 2021** (`N10`, FT): "Geldend van 04-05-2021 t/m 30-12-2023", "Regeling vervallen per 18-05-2024". `CVDR719903` is the **Verordening bomen 2024** (`N9`, FT): "Geldend van 18-05-2024 t/m 11-06-2026", "Regeling vervallen per 12-06-2026". The instrument in force is the **Verordening bomen 2026** (`N8`, FT, CVDR762747, "Geldend van 12-06-2026 t/m heden").

The provisions that bear on any volunteer or community tree work on municipal ground (`N8`, FT):

> "Artikel 10 … 1. Het is verboden om een boom of houtopstand: … b. die in eigendom is van de gemeente, boven of onder de grond te beschadigen, te bekladden, te beplakken of te behangen met voorwerpen; **c. die in eigendom is van de gemeente, te snoeien, met uitzondering van door de gemeente opgedragen of toegestane boomverzorgende taken.**"

> "Artikel 2 … 1. Binnen de bebouwingscontour houtkap is het verboden zonder omgevingsvergunning van het college de volgende handelingen te verrichten of laten verrichten: a. het vellen van een boom of houtopstand met een stamomtrek van minimaal 45 centimeter op 130 centimeter hoogte …; **b. het snoeien van meer dan 30% van het kroonvolume of wortelgestel** …; c. het verplanten …; d. voor het eerst kandelaberen of kandelaren …; **e. het vellen, snoeien voor meer dan 30%, of verplanten van een boom of houtopstand, ongeacht de stamomtrek, die is aangelegd op grond van een herplant-, compensatie en/of instandhoudingsplicht**; …"

Art. 4 exempts from the permit duty "velling door of namens de gemeentelijke bomenbeheerder op grond in eigendom van de gemeente" for "beheermaatregelen, zoals maatregelen ten gunste van de natuur of te behouden bomen" and for unstable or short-lived trees. Art. 11(1): the minimum distance to a property boundary for municipal trees, shrubs and hedges is "0 meter (nihil)"; for private trees 0,5 m (art. 11(2)). Art. 7(2): a felling permit "in verband met het plaatsen of belichten van zonnepanelen, zonnecollectoren en kleine windmolens, wordt door het college geweigerd".

Two carry-overs worth noting for interpretation. First, competence splits by contour (`N8`, art. 1): "bevoegd gezag: buiten de bebouwingscontour houtkap: De provincie Noord-Brabant. binnen de bebouwingscontour houtkap: De gemeente Eindhoven." Second, a *narrowing over editions*: the 2021 verordening exempted from permit "het periodiek oogsten van hakhout voor regulier onderhoud" (`N10`, FT, art. 2(3)(c)); that wording is absent from the 2024 and 2026 texts I retrieved. *Interpretation:* a harvesting-style exemption that once existed in the tree regime is not in the current one.

**6c. Groenbeleidsplan, Groenstructuurplan, park regulations.** The Groenbeleidsplan 2017 is repeatedly named as the governing green policy (`N7` toelichting: "Het gemeentelijk groenbeleidsplan is bij inwerkingtreding van deze beleidsregel het ‘Groenbeleidsplan 2017’"; `N8` toelichting: "groene wiggen, groene dooradering, hoofdgroenstructuur, zie groenbeleidsplan 2017"; `N3` refers to "ons Groenbeleidsplan (2016-2026)"). **The plan itself was not retrieved.** Its content is therefore known only through these citations.

Also from `N8` (FT, toelichting art. 5): "Binnen deze groenstructuur zijn alle bomen op gemeentegrond waardevolle bomen"; and the only per-dwelling green-area norm I found anywhere: "In deze buurten is het groenareaal per woning beneden de landelijke norm van 75 m2 per woning ligt" (definition of *groenarme gebieden*).

**No park-specific regulation was retrieved** for Stratumse Heide, Genneper Parken, Philips de Jongh Wandelpark or Henri Dunantpark: no visitor rules, closing times, dog zones or event conditions as a published reglement. The instruments that in fact apply to those parks are the APV (art. 2:45 off-path; 2:57 dogs; 2:18/5:34 fire; 2:25 events), the aanwijzingsbesluit for the eight leash areas (`N6`), and the bomenverordening. **Not established** whether park-level rules exist outside the APV.

### 7. Carrying capacity, visitor pressure, "drukte"

**No carrying-capacity standard was found — and a municipal report shows the municipality was building measurement capacity in 2023, not a norm.** This is the clearest negative finding in this line.

`N14` (FT, Royal HaskoningDHV for Gemeente Eindhoven, 3 July 2023, ref. BG7775-MI-RP-230630-1603):

> "Naarmate het gebruik van en drukte in de groene ruimtes toeneemt, wordt de impact op ecologie, bezoekers ervaring, overlast en omgeving steeds groter."

> "Er is nu inzicht in de bezoekersstromen in de parken, maar nog niet of beperkt in oorzaak of type van de drukte en de gevolgen. Verder kijkend is er ook signalering nodig of er interventies moeten plaatsvinden, en waar."

The concern it was answering, and its origin in the Genneper Parken inrichtingsplan:

> "Een belangrijk onderdeel van het plan is om de (recreatieve) druk beter te verdelen en verkeersstromen (auto’s, fietsers, wandelaars) ten behoeve daarvan beter te sturen." … "Kan de flora en fauna in het gebied de toenemende druk nu en in de toekomst aan?"

Its proposed impact model is explicitly multiplicative and has no threshold: "impact = gevoeligheid * effect * hoeveelheid". The closest thing to a norm is a *future dashboard warning*: "Knelpunten waarschuwing : aangeven dat er op een bepaalde locatie door bepaald gebruik te hoge bezoekersdichtheden ontstaan." No value, unit or threshold is given anywhere in the report; it is a design document ("De hier voorgestelde opzet gaat uit van een open datamodel"), with use cases for parking, beleving, social safety and ecology, and it names a companion note I did not retrieve: "‘Notitie Borging kwaliteit ecologie Genneper Parken’ met kenmerk BG7775-MI-ME-230607-1503 d.d. 7 juni 2023".

Municipal acknowledgment that disturbance scales with population, without a norm (`N3`, FT): broedvogel decline attributed to "ruimtelijke ontwikkeling en de afname van de kwaliteit van leefgebied door verdroging, opwarming, stikstofdepositie, maar ook verstening van tuinen in het stedelijk gebied en toenemende verstoring (mede als gevolg van groeiende bevolking)". And among the plan's own remedies: "Gerichter sturen op vermindering verstoring, bijvoorbeeld door sturing/zonering van recreatiestromen (inclusief huisdieren zoals honden) en strategischer verlichting van de openbare ruimte."

**What exists instead of a carrying-capacity standard** are area-of-green norms, which are not visitor norms: 8 m² new green per added dwelling; 10% of BVO for non-residential; €236 per unrealised m²; and the 75 m² green per dwelling "landelijke norm" used to define green-poor neighbourhoods (`N7`, `N8`). *Interpretation:* these ration **green area against built programme**, not **visitors against ecological capacity**. Conflating them would be an error.

**So our brief's claim is supported, with a precise search surface.** No carrying-capacity standard was found in: the APV (full text); the 2026 groen/water beleidsregel (full text); the bomenverordeningen 2021/2024/2026; the Omgevingsverordening NNB and stiltegebied articles; the biodiversiteitsplan; the natuurpuntenkaart page; the Omgevingsvisie raadsvoorstel; and the Genneper Parken monitoring report. What the record does contain is (a) a monitoring *design* (2023), (b) intentions to steer and zone, (c) the leash designations as the one operationalised zoning measure, and (d) area norms.

### 8. Nationaal Park / Groene Woud / Regiodeal

**Nothing established.** I retrieved no source from a Nationaal Park authority, the Groene Woud cooperation, or a Regiodeal that states a constraint on recreation or access relevant to Eindhoven. One neighbouring item was seen but not read: a "Natuurbrandbeheersplan Groote Heide / Stratumse Heide / Valkenhorst, Leenderbos-Malpie en Strabrechtse Heide" appeared in search results as a document on a municipal notubiz site (`SNIP`). It plausibly bears on access during fire risk, but **I did not read it and make no claim about it.**

---

## What actually constrains an activity

Rows are activities; status is my reading of the retrieved record: **Documented** = an instrument says it in terms; **Partly** = the instrument reaches it indirectly; **Not established** = searched, not found.

| Activity | Instrument | What it says | Source | Status |
|---|---|---|---|---|
| Walking in parks | APV art. 2:45(1) | Presence off the paths in municipal green prohibited without college ontheffing; presence on the paths is not covered by this prohibition | `N5` | Documented |
| Walking in Natura 2000 / NNB | Omgevingsverordening arts. 5.30–5.33 | Rules address the omgevingsplan, not the visitor; no visitor rule found | `N11` | Partly (indirect) |
| Dogs | APV art. 2:57(1)(b) | Leash required on public places inside the built-up area | `N5` | Documented |
| Dogs — Wielewaal and 7 other areas | Aanwijzing aanlijnplicht 2025, art. 1 | Leash "elke dag van de week, gedurende de gehele dag" | `N6` | Documented |
| Dogs — ecological effect | Plan van aanpak biodiversiteit §8 | "Loslopende honden zorgen o.a. voor verstoring en vermesting" | `N3` | Documented (policy) |
| Events | APV arts. 2:24–2:25a | Burgemeester's permit; refusal ground includes mismatch with the location's "locatieprofiel" | `N5` | Documented |
| Events — noise | APV art. 4:6 | Nuisance prohibition + ontheffing | `N5` | Documented |
| Events — stiltegebied | Omgevingsverordening art. 5.29(b) | 50 dB(A) LAeq 24h at the stiltegebied boundary | `N11` | Documented (plan-level) |
| Foraging / plucking | — | No APV article on picking plants or produce found; art. 2:45 still governs being off-path | `N5` | Not established (no rule found) |
| Lighting | APV afd. 4.1; arts. 4:2, 4:16, 5:34(4) | Festiviteiten-verlichting and lichtreclame provisions; no park-lighting rule found | `N5` | Not established (no rule found) |
| Fires / cooking | APV art. 5:34(1)–(2)(b)(c) | Open-air fire prohibited; sfeervuren and cooking fires excepted absent gevaar/overlast/hinder/schade; ontheffing possible | `N5` | Documented |
| Smoking on heath / in woods | APV art. 2:18(1)(a) | Prohibited, and within 30 m, all year (1 Jan–31 Dec) | `N5` | Documented |
| Tree work — own/municipal trees | Verordening bomen 2026 art. 10(1)(b)(c) | Municipal trees may not be damaged, or pruned except as commissioned/permitted by the municipality | `N8` | Documented |
| Tree work — felling/pruning | Verordening bomen 2026 art. 2(1) | Permit for ≥45 cm girth, >30% crown/root pruning, replanting, first kandelaberen; and for compensation-planted trees regardless of size | `N8` | Documented |
| Tree work — competence | Verordening bomen 2026 art. 1 | Inside contour: municipality; outside: province | `N8` | Documented |
| Drone use | — | No APV provision found; national rules not retrieved | `N5` | Not established |
| New planting on municipal green | Beleidsregel 2026 art. 3(1)(b)(c) | Applications for management by third parties, and for sale/lease of green ground, fall inside the beleidsregel | `N7` | Documented (procedural) |
| New planting — protected/compensation trees | Verordening bomen 2026 art. 2(1)(e) | Trees planted under a replant/compensation/maintenance duty need a permit to fell, prune >30% or move, regardless of size | `N8` | Documented |
| New planting — area norms | Beleidsregel 2026 arts. 4(5), 4(6), 7(3) | 8 m²/woning; 10% BVO; €236 per unrealised m² | `N7` | Documented |
| Small structures | APV art. 2:10(1) | Using the "weg" (incl. parks) other than per its public function requires a B&W permit | `N5` | Partly |
| Small structures in NNB | Omgevingsverordening art. 5.33(1) | Small buildings for the nature function or "recreatief medegebruik" may be allowed only if no aantasting | `N11` | Partly (plan-level) |
| Objects on municipal trees | Verordening bomen 2026 arts. 10(1)(b), 10(3) | Damaging/affixing objects prohibited; excepted with written college consent | `N8` | Documented |
| Vehicles in green | APV art. 5:11(1) | Driving through park/planting prohibited except on the road and for public works | `N5` | Documented |
| Illegal use of municipal ground | Plan van aanpak biodiversiteit §3.4.2 | Enforcement announced; focus on nature-development areas | `N3` | Documented (policy) |
| Visitor volume / "drukte" | — | Monitoring design only; no threshold | `N14` | Not established (no standard found) |

---

## Searched and not found

This section is the negative evidence. Each item states what I looked for and where.

1. **A carrying-capacity or visitor-density standard.** Searched: APV Eindhoven full text; Beleidsregel groen en water 2026 full text; Verordening bomen 2021/2024/2026; Omgevingsverordening Noord-Brabant chapters 3 and 5; Plan van aanpak biodiversiteit; natuurpuntenkaart page; Omgevingsvisie raadsvoorstel; Genneper Parken monitoring report; web searches for `"bezoekersdruk" OR "drukte"` with Eindhoven, `nota recreatie`, `Wielewaal Lichtbos bezoekers verwachting aantal`. **Result: none.** The only "te hoge bezoekersdichtheden" phrasing is a *planned dashboard warning* in `N14`, with no value.
2. **A municipal recreation note ("nota recreatie").** Searched as above; no such document retrieved or referenced.
3. **The Omgevingsvisie Eindhoven 2040 itself.** Only the raadsvoorstel (`N15`) was retrieved; the visie is a separate registratienummer (7784858) not retrieved. Any statement on green/visitor pressure inside the visie itself is **unread**.
4. **The Groenbeleidsplan 2017.** Named repeatedly as governing policy (`N3`, `N7`, `N8`); the document itself not retrieved.
5. **Locatieprofielen evenementen.** Referenced by APV art. 2:25(3)(d) (`N5`); no locatieprofiel document retrieved.
6. **Park-specific visitor regulations** for Stratumse Heide, Genneper Parken, Philips de Jongh Wandelpark, Henri Dunantpark. None retrieved; APV + aanwijzingsbesluit appear to be the operative layer.
7. **Any APV article on foraging, plucking or harvesting.** Full-text searches of the consolidated APV for *pluk*, *oogst*, *gewassen*: only art. 2:15 (hinderlijke beplanting) and art. 5:11 (voertuigen) matched. **No such article exists in the retrieved text.**
8. **Any APV article on drones.** Searches for *drone*, *onbemand*, *luchtvaartuig*: no match. National aviation rules were not retrieved, so the applicable drone regime is **not established** here.
9. **The SMP document, its area, its species list, and any gebiedsgerichte vergunning.** Not in the public record as retrieved; `N2` states "Er is nog geen gebiedsgerichte vergunning verleend".
10. **The 2022 "Soortmanagementplan gebouwbewoonende soorten Eindhoven en Geldrop" (bijlage 13).** Two connection aborts; content unknown; only a snippet.
11. **Natura 2000 beheerplan (2021) and natuurdoelanalyse for Leenderbos, Groote Heide & De Plateaux.** Three failed attempts including Wayback. The recreation/`verstoring` passage is therefore **unavailable**, not absent.
12. **A public natuurpunten dataset or map service.** Not found on the retrieved municipal page.
13. **A provincial "natuurpunten" methodiek** distinct from Eindhoven's Sweco calculator. Not established. A Rijkswaterstaat pilot publication on natuurpunten as biodiversity KPI was seen (`SNIP`) and not read.
14. **NNB boundary map for Eindhoven.** Not retrieved; adjacency inferred only from `N3`'s statement that municipal farmland around the city is outside NNB.
15. **Groene Woud / Nationaal Park / Regiodeal sources stating a recreation or access constraint.** None retrieved.
16. **Successor/beheerplan for the 2026 bomenverordening's "overlastmatrix"** ("De overlastmatrix wordt openbaar gemaakt", `N8`) — not retrieved.

---

## Sources

**N1** — Gemeente Eindhoven, College van B&W. *Collegebrief: Soortenmanagementplan en natuurvriendelijk isoleren.* Inboeknummer 7931804_2.2.1, dossiernummer 25.20.103, B&W-beslisdatum 13 mei 2025. `https://raadsinformatie.eindhoven.nl/document/15539396/2/7931804_2_2_1_+Collegebrief+aan+de+raad+over+Soortenmanagementplan+en+natuurvriendelijk+isoleren?connection_type=17&connection_id=11857567` — PDF, 12,458 chars, **FT**, retrieved 2026-11-26. Quotes: §1 above (Omgevingswet/province; third-party use of the area permit; SMP scope; "medio juli 2027"/Q3 2027/10 years; three-year duration; "nog niet volledig ingekaderd"); project-steps table; NVI 6% split "3% voor 2024/2025, 2% voor 2025/2026 en 1% voor 2026/2027"; budget € 1.500.000 and € 832.549.

**N2** — SMPcheck (Ecosprong), *Soortenmanagementplan Eindhoven.* `https://smpcheck.nl/gemeente/eindhoven` — HTML, 6,388 chars, **FT** of the page; **third-party aggregator, not an authority**; page states "Laatst gecontroleerd op actualiteit: 11 oktober 2026", retrieved 2026-11-26. Quotes: "In voorbereiding … geen gebiedsgerichte vergunning"; "18 september 2026 Status: SMP in voorbereiding"; "eind 2027 SMP verwacht"; "Ecologisch bureau: EcoGroen"; "Uitvoering Omgevingsdienst Zuidoost-Brabant"; "De landelijke werkwijze om zonder SMP te isoleren is in 2025 gestopt." Disclaimer printed on the page: "Aan dit overzicht kunnen geen rechten worden ontleend."

**N3** — Gemeente Eindhoven. *Plan van aanpak biodiversiteit in Eindhoven* (college vastgesteld 4 juli 2023 per `N1`). `https://www.eindhovenduurzaam.nl/sites/default/files/2024-07/DT_Biodiversiteits%20verslag_2862024.pdf` — PDF, 96,398 chars, **FT**, retrieved 2026-11-26. Quotes: illegal use of municipal ground and enforcement focus; "(landbouw)gronden die niet horen bij het Natuurnetwerk Brabant"; "Gerichter sturen op vermindering verstoring, bijvoorbeeld door sturing/zonering van recreatiestromen (inclusief huisdieren zoals honden) en strategischer verlichting"; "8. Honden aan de lijn: Loslopende honden zorgen o.a. voor verstoring en vermesting"; "toenemende verstoring (mede als gevolg van groeiende bevolking)"; natuurpuntensysteem passage + "Doel: eerste natuurpuntenkaart (nulmeting) in H1 2024"; monitoring since 2009 and classes 0–5.

**N4** — Gemeente Eindhoven (Eindhovenduurzaam). *Natuurpuntenkaart.* `https://www.eindhovenduurzaam.nl/natuurpuntenkaart` — HTML, 3,247 chars, **FT**, retrieved 2026-11-26. Quotes: "natuurpuntenkaarten laten maken in samenwerking met adviesbureau Sweco"; "berekend met de natuurpuntencalculator"; "per buurt"; "In de komende jaren worden er nieuwe berekeningen gemaakt".

**N5** — Gemeente Eindhoven. *Algemene plaatselijke verordening Eindhoven*, CVDR415534, versie `/18`, "Geldend van 26-09-2025 t/m heden". `https://lokaleregelgeving.overheid.nl/CVDR415534/18` — HTML, 162,623 chars, **FT**, retrieved 2026-11-26. Quotes verbatim: art. 1:1 ("weg" incl. parken); art. 2:10(1); art. 2:18(1); art. 2:24(1); art. 2:25(1),(3)(d); art. 2:25a; art. 2:45(1),(2); art. 2:57(1)(b),(c); arts. 2:61/2:62/2:63/2:64 "[gereserveerd]"; art. 4:6(1); arts. 4:10/4:11/4:12 "[gereserveerd]"; art. 4:16 "[gereserveerd]"; art. 5:11(1); art. 5:33(1),(4); art. 5:34(1),(2)(b),(c),(3),(4).

**N6** — Gemeente Eindhoven, College van B&W. *Aanwijzing gebieden aanlijnplicht honden 2025.* Inboeknummer 7949485_04, dossiernummer 25.25.201, B&W-beslisdatum 20 juni 2025. `https://raadsinformatie.eindhoven.nl/document/15711867/1/7949485_03+Bijlage+1a+-+Besluit+aanwijzing+gebieden+aanlijnplicht+honden+2025?connection_type=16&connection_id=1057349` — PDF, 3,677 chars, **FT**, retrieved 2026-11-26. Quotes: art. 1 opening and area B (Wielewaal, with its four bounding roads); grounds ("Om de biodiversiteit in een aantal gebieden te beschermen"); the eight areas A–H.

**N7** — Gemeente Eindhoven, College van B&W. *Beleidsregel groen en water bij ruimtelijke ontwikkelingen gemeente Eindhoven 2026*, CVDR766778, versie `/1`, "Geldend van 23-09-2026 t/m heden". `https://lokaleregelgeving.overheid.nl/CVDR766778/1` — HTML, 108,375 chars (**FT-part**: read to 100k), retrieved 2026-11-26. Quotes: art. 1 definitions (beschermd groen; aanwezig groen; openbaar groen; groene wiggen); art. 3(1); art. 4(5),(6); art. 7(2),(3); toelichting on the Natuurherstelverordening ("18 augustus 2024 … niet af mag nemen tot 2031"); toelichting on NNB and provincial instructieregels; toelichting "Het gemeentelijk groenbeleidsplan is bij inwerkingtreding van deze beleidsregel het ‘Groenbeleidsplan 2017’". Not read: the truncated tail (Bijlage 1 tables).

**N8** — Gemeente Eindhoven (raad). *Verordening bomen 2026*, CVDR762747, versie `/2`, "Geldend van 12-06-2026 t/m heden". `https://lokaleregelgeving.overheid.nl/CVDR762747/2` — HTML, 40,968 chars, **FT**, retrieved 2026-11-26. Quotes: art. 1 (bevoegd gezag split; houtopstand; kandelaberen/kandelaren; waardevolle boom); art. 2(1)(a)–(f); art. 3; art. 4; art. 5; art. 7(1)–(5), incl. 7(2); art. 10(1)(b),(c), 10(3); art. 11(1),(2); toelichting "Binnen deze groenstructuur zijn alle bomen op gemeentegrond waardevolle bomen"; toelichting "landelijke norm van 75 m2 per woning"; "De overlastmatrix wordt openbaar gemaakt."

**N9** — Gemeente Eindhoven (raad). *Verordening bomen 2024*, CVDR719903, versie `/1`, "Geldend van 18-05-2024 t/m 11-06-2026", "Regeling vervallen per 12-06-2026". `https://lokaleregelgeving.overheid.nl/CVDR719903/1` — HTML, 17,341 chars, **FT**, retrieved 2026-11-26. Used for the version history and art. 2(1)(b) (30% crown/root pruning) / art. 3 (outside the contour).

**N10** — Gemeente Eindhoven (raad). *Verordening bomen 2021*, CVDR657211, versie `/1` — **the CVDR id given in our brief**. "Geldend van 04-05-2021 t/m 30-12-2023", "Regeling vervallen per 18-05-2024". `https://lokaleregelgeving.overheid.nl/CVDR657211/1` — HTML, 14,516 chars, **FT**, retrieved 2026-11-26. Quote: art. 2(3)(c) "het periodiek oogsten van hakhout voor regulier onderhoud" among permit exemptions.

**N11** — Provincie Noord-Brabant. *Omgevingsverordening Noord-Brabant*, Provinciaal blad 2025, 13146, published 11-08-2025 (ondertekend 01-07-2025). `https://zoek.officielebekendmakingen.nl/prb-2025-13146.html` — HTML, 1,132,004 chars (**FT-part**: first 200,000 read), retrieved 2026-11-26. Quotes: arts. 5.28(1); 5.29(b); 5.30(1)(a)–(c); 5.31(1); 5.32(2); 5.33(1),(3); 5.34(1) opening. Context: Hoofdstuk 5 is headed "Instructieregels voor het omgevingsplan gemeenten".

**N12** — Ministerie van Landbouw, Visserij, Voedselzekerheid en Natuur. *Vaststelling nieuwe tekst aanwijzingsbesluit Leenderbos, Groote Heide & De Plateaux*, Stcrt. 2026, 2565, 26 januari 2026 (ondertekend 23 januari 2026). `https://zoek.officielebekendmakingen.nl/stcrt-2026-2565.pdf` — PDF, 232,315 chars (**FT-part**: opening read, full text grepped), retrieved 2026-11-26. Quotes: "behoort tot het grondgebied van de gemeenten … Eindhoven …"; "landelijk gebiedsnummer 136"; "NL3009014"; the gemeenten list in §4 above.

**N13** — Kragten, for PSV Stadionexploitatie B.V. *Voortoets Natura 2000*, rapport 20261009-PSV003-RAP-VRT 3.0, 9 oktober 2026; bijlage bij ontwerp-omgevingsvergunning EHV-DP2026-173548 (zaak EHV-ZP2026-009575, 27 oktober 2026). `https://publicaties.eindhoven.nl/sites/default/files/genetics/B14_Voortoets_0.pdf` — PDF, 363,823 chars (**FT-part**: first 100k read, remainder grepped), retrieved 2026-11-26. Quotes: Tabel 1 distances; "0,02 mol N/ha/jaar"; the "Vanwege de ligging … alleen significante effecten als gevolg van verzuring" passage; "In de aanlegfase is verder vooral sprake van verstoring door geluid, licht, trillingen etc."

**N14** — Royal HaskoningDHV (Bogers & Van Ruth) for Gemeente Eindhoven. *Monitoren druk en dynamiek in Genneper Parken*, ref. BG7775-MI-RP-230630-1603, Definitief/1.0, 3 juli 2023. `https://www.eindhoven.nl/sites/default/files/2023-07/Definitief%20rapport%20Monitoren%20druk%20en%20dynamiek%20in%20Genneper%20Parken.pdf` — PDF, 65,878 chars, **FT**, retrieved 2026-11-26. Quotes: "Naarmate het gebruik …"; "Er is nu inzicht …"; "(recreatieve) druk beter te verdelen"; "impact = gevoeligheid * effect * hoeveelheid"; "Knelpunten waarschuwing … te hoge bezoekersdichtheden"; reference to "Notitie Borging kwaliteit ecologie Genneper Parken" (BG7775-MI-ME-230607-1503, 7 juni 2023).

**N15** — Gemeente Eindhoven, College van B&W. *Raadsvoorstel Omgevingsvisie Eindhoven*, Inboeknummer 24bst01157, dossiernummer 24.41.451, B&W-beslisdatum 8 oktober 2024. `https://raadsinformatie.eindhoven.nl/document/14638368/1/24bst01157+Raadsvoorstel+Omgevingsvisie+Eindhoven+?connection_type=17&connection_id=11042878` — PDF, 21,995 chars, **FT**, retrieved 2026-11-26. Quotes: "Het is een richtinggevend document voor de gemeente, maar niet juridisch bindend voor de inwoners"; "De omgevingsvisie richt zich op het jaar 2040"; the attachment list (Omgevingsvisie registratienummer 7784858, not retrieved).

---

## Limits of this line

- **Two retrieved-source families failed at the origin** (raadsinformatie document 13615815; three provincial PDFs on brabant.nl including the 2021 beheerplan). Those are gaps in *my* record, not evidence that the documents do not exist. The beheerplan recreation passage is the most material of these: a PI with library access, or a direct request to Provincie Noord-Brabant, could close it.
- **One third-party source** (`N2`) is an aggregator with its own disclaimer; its date ("eind 2027") conflicts with the municipality's (`N1`) and is not treated as authoritative.
- **Two key plans were never read** — the Groenbeleidsplan 2017 and the Omgevingsvisie 2040 — so their content is known only through documents that cite them.
- **Nothing here establishes that any specific initiative is or is not permitted.** The instruments are stated; their application is not assessed.
- **Adjacent questions noticed and not researched:** the Natuurbrandbeheersplan for Groote Heide/Stratumse Heide; locatieprofielen as a zoning instrument; the provincial eDNA/pre-SMP route and its 2026 status; the "overlastmatrix" for municipal trees; the stiltegebieden actually designated around Eindhoven; whether a *gebiedsgerichte vrijstelling* (rather than vergunning) is available under the Omgevingswet for green-space works at all.
