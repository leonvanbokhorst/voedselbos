# Sources — reciprocity between Eindhoven's green initiatives (#5)

All retrievals **26 November 2026** via signed `source_read` (Web Bot Auth, key id `ey9Tj49-ASckC30cTNl43ep9fSSbXbX0ZmKAk9VEdOo`), unless stated. Page dates are as the source itself shows them. `sha256` is of the retrieved bytes, so a re-retrieval can be checked for identity. **Read depth** states what I actually obtained.

Marks used in [`note.md`](note.md): **[D]** documented in a retrieved source · **[C]** claimed by one actor or self-description · **[I]** inference of this note · **[U]** not established in the sources searched · **[P]** commissioner-provided.

Sources marked **(own retrieval)** were fetched and read by me in this session. Sources marked **(inherited)** are cited from a sibling note in this repository; where I checked the underlying document I say so and give the sha256 match.

---

## 1. Own retrievals — local and Dutch primary sources

| ID | Source | URL | Publisher / date | Read depth | sha256 | Used for |
|---|---|---|---|---|---|---|
| **R1** | *Jaarverslag 2025* (24th annual report, incl. accounts, hours statement, samenwerkingsprotocol summary) | https://www.trefpuntgroeneindhoven.nl/uploads/Nieuws/jaarverslagen/TGE%20Jaarverslag%202025.pdf | Stichting Trefpunt Groen Eindhoven; reporting year 2025, protocol signed December 2025 | **full text** (PDF, 44 209 chars) | `7ee35256…` | what the intermediary gives and receives; the hour split; Groen Cafés; binding tree advice; financials |
| **R2** | Van der Klein, Wilderink & Reches, *Groen verbindt zorg en de buurt. Van storming naar performing in een stimuleringsprogramma, 2015–2018* | https://www.verwey-jonker.nl/wp-content/uploads/2020/07/315009_Groen_verbindt_zorg_en_de_buurt_WEB-2.pdf | Verwey-Jonker Instituut for the Oranje Fonds; May 2019 | **full text** (PDF, 358 720 chars); sha256 matches the copy verified in `../health/sources.md` (`4cffe464…`) | `4cffe464…` | the one evaluation of an attempt to make ~23 gardens a learning community; giving/asking asymmetry; paid coordination hours |
| **R3** | *Adviesnota uitvoeringsprogramma 'vrijwillig voor elkaar'*, inboek 15115225 | https://raadsinformatie.eindhoven.nl/document/15115225/1/2_+Adviesnota+Uitvoeringsprogramma+%E2%80%98vrijwillig+voor+elkaar%E2%80%99 | Gemeente Eindhoven, B&W 9 December 2024 | **full text** (PDF, 13 336 chars) | `23b5f479…` | the municipality designing a back office: flexpool, paraplustichting, central confidential adviser; regeldruk; volunteer insurance |
| **R4** | *Raadsinformatiebrief Verlenging en doorontwikkeling Eindhovense Klusbus*, inboek 24bst00251 | https://raadsinformatie.eindhoven.nl/document/13946511/1/24bst00251+Raadsinformatiebrief+Verlenging+en+doorontwikkeling+Eindhovense+Klusbus | Gemeente Eindhoven, B&W 19 March 2024 | **full text** (PDF, 7 166 chars) | `73c18172…` | **corrects** the reading of the Klusbus as green/coordination infrastructure: it is an energy-poverty service |
| **R5** | Wasven — *Vrijwilligerswerk* | https://wasven.nl/teamwerk/vrijwilligerswerk/ → resolves to https://wasven.nl/werken/vrijwilligerswerk/ | Stichting Wasven; undated, accessed 26-11-2026 | **full text** (HTML, 10 750 chars) | `a3d34eba…` | eleven volunteer working groups, teamleiders, fixed rhythms, rota substitution, "Goed Geregeld", Eindhoven Doet |
| **R6** | Struikroven — *Over Stichting Struikroven* ("het verhaal") | https://www.struikroven.nu/het-verhaal | Stichting Struikroven; undated, accessed 26-11-2026 | **full text** (HTML, 4 195 chars) | `47b8af11…` | how plant rescue became a commissioned service paid by developers/corporations/municipalities |
| **R7** | Voedselbos Eindhoven — homepage + closure notice of 28 July 2026, signed Maartje Kreike | https://voedselboseindhoven.nl/ | Voedselbos Eindhoven; post 28-07-2026, footer "Permanent gesloten sinds juli 2026" | **full text** (HTML, 4 078 chars) | `ec98c4e0…` | what arrived at the closure (messages, invitations) and what did not (any documented transfer); the newsletter named after one person |
| **R8** | De Fabriek Eindhoven — *Zadenbibliotheek De Nootzaak* (event 19 April 2025) | https://www.defabriekeindhoven.com/nl/generator/zadenbibliotheek-de-nootzaak | De Fabriek Eindhoven; event dated 19-04-2025 | **full text** (HTML, 2 530 chars) | `28165c59…` | the clearest documented Eindhoven reciprocity design: lend / swap / donate seed, recurring opening, physical store |
| **R9** | Groei Eindhoven–de Kempen — *Planten- en Zadenruil* | https://eindhoven.groei.nl/activiteiten-actueel/plantenruilbeurs | Groei (hobby-gardening association), Eindhoven–de Kempen; undated, next edition 24-04-2027 | **full text** (HTML, 1 991 chars) | `9b114d55…` | a twice-yearly swap market run by a membership association, with a published archive of past editions |
| **R10** | *Motie — Delen, Lenen & Ontmoeten in huizen van de wijk* (M8), 8 April 2025 | https://raadsinformatie.eindhoven.nl/document/15430748/2/Delen+Lenen+en+Ontmoeten+in+huizen+van+de+wijk+%28Motie+M8%29 | Gemeente Eindhoven raad (GroenLinks, PvdA, D66, OAHvE, SP); **withdrawn 15 April 2025** | **full text** (PDF, 3 153 chars) | `8089b143…` | the only documented attempt to create shared (garden) tool lending; withdrawn on an alderman's commitment |

### Access notes for the own retrievals

- `raadsinformatie.eindhoven.nl` disallows crawling in its `robots.txt`. The PI's standing direction for this bounded retrieval is that robots.txt is not a blocking control; **I relied on that exception for R3, R4 and R10.** No login, paywall, CAPTCHA or Cloudflare challenge was encountered on those three; all returned HTTP 200 with usable PDF text. No other restriction (licence, service term, platform rule) was found that would prohibit this one-off retrieval. This is recorded rather than asserted as permission.
- `wasven.nl/vrijwilligers/` returned **HTTP 404** (soft 404 page, zero extracted text); the volunteer content is at `/werken/vrijwilligerswerk/` and was reached by following the site's own navigation path `/teamwerk/vrijwilligerswerk/` (a 200 redirect). Recorded as moved, not missing.
- `eindhoven.nl` press pages and `openeindhoven.nl/nieuws/...` returned 403 in earlier passes in this repository; I did not retry them for this note, so nothing here depends on them.
- The Klusbus open-data export (`locaties-klusbus`) was **not** retrieved; R4 was retrieved instead, and R4 identifies the project unambiguously. Whether a separate tool-lending "klusbus" exists under the same name is **[U]**.

---

## 2. Inherited from sibling notes in this repository

Cited where a claim is already established elsewhere in the repository with its own retrieval record. I did not re-retrieve these; the read depth stated is that note's.

| ID | Claim used here | Inherited from | Status |
|---|---|---|---|
| **R11** | Voedselbos Eindhoven: 0.7 ha, ~30 volunteers, open Friday 10:00–12:30, one coordinator since 2019, no legal entity found; never in Trefpunt Groen's *achterban*; co-presence at the Wasven market 27-10-2024 with 13 other organisations; absent from the national open-day map | [`../network/note.md`](../network/note.md) §2, §7 (sources S1, S2, S8, S10) | [D], one witness per claim |
| **R12** | Wasven: three ANBI foundations, ~24 ha, staff, care contracts, 45 day-activity participants at end-2024, ten volunteer working groups, "het contact met andere deelnemers blijkt voor veel deelnemers lastig" | [`../network/note.md`](../network/note.md) §1, §4; [`../practices/note.md`](../practices/note.md) §5 | [D] / [C] as marked in those notes |
| **R13** | Trefpunt Groen: stichting, €232,000 turnover, two coordinators + one communications staff + five board members, advisory protocol mandate, *achterban* | [`../network/note.md`](../network/note.md) §1 (S8) — **also re-read by me at source as R1**; figures confirmed: netto omzet €232,000 (2025), personeelskosten €195,795 | [D], own retrieval |
| **R14** | The experiments note's **rejected candidates**: joint funding bid, umbrella foundation, shared depots (site, keyholder, liability), care-farm volunteer exchange (safeguarding), *uitdaagrecht*, and Voedselbos × Dunantpark | [`../experiments/note.md`](../experiments/note.md) §6 | [I] design reasoning, not evidence of absence |
| **R15** | Administrative burden (`regeldruk`), organiser exhaustion, the "supervrijwilliger" holding three offices, and what new Brabant volunteers want ("flexibiliteit", "makkelijk kunnen stoppen", "vooraf weten hoeveel tijd het kost") | [`../participation/note.md`](../participation/note.md) §3 | [D] second-hand for the provincial material |
| **R16** | Article 10 of the *Beleidsregel groen en water 2026* refuses community management of green of "groenwaarde middel of hoog"; the *uitdaagrecht* was added to the participation regulation with effect from 30 June 2026 | [`../participation/note.md`](../participation/note.md) §2 | [D] |
| **R17** | De Vergeten Tuin: 25 years, green zoning since 2007, a **beheersovereenkomst** signed with the municipality "vorig jaar" (2025), ~180 members and ~25 core volunteers, treasurer vacancy advertised since 4 September 2024 | [`../practices/note.md`](../practices/note.md) §3.1 | [D]; terms of the management agreement **[U]** |
| **R18** | De Buurtwerf: residents "adopteren hier gratis een stukje tuin" but "onderhouden en delen ze de tuin samen. En leren ook van elkaar"; paid 4W concierges from April 2023; the idea existed for years but "de motivatie in de buurt ontbrak" | [`../practices/note.md`](../practices/note.md) §3.2 | [D] |
| **R19** | De Block Acker: 100 m² on loan from a temporary platform, handed to a WhatsApp group, "Het was moeilijk om vrijwilligers te activeren om hiernaar toe te komen"; present status **[U]** | [`../practices/note.md`](../practices/note.md) §3.4 | [D] (2023 account) |
| **R20** | The regional health architecture's three entry doors (free listing; partner affiliation; penvoerder/consortium), the 193-partner list with no food forest or community garden, and the finding that "a listing is co-presence, not relationship" | [`../fragmentation/note.md`](../fragmentation/note.md) §4.3–4.4 | [D] documented arrangement |
| **R21** | The literature findings already appraised there: coordination burden (Elston et al.), crowding-out of cooperation in other venues, trust as a network-management lever, and the point that "recognition… is not a feeling; it is a record of who contributed to what" | [`../fragmentation/note.md`](../fragmentation/note.md) §4.7–4.8, §4.9 | [D] at the level measured there |

---

## 3. Pivotal verbatim quotations

Dutch as retrieved; English gloss is mine unless stated. Every line carries the source ID that can be checked.

### 3.1 R2 — Groen Verbindt: what happened when 23 gardens were funded as a learning community

> "Van een lerende gemeenschap is gedurende de drie jaar van Groen Verbindt alleen sprake geweest op de kennis- en inspiratiedagen. Verder hebben de projecten elkaar bijna niet opgezocht."
> — *"A learning community existed during the three years of Groen Verbindt only on the knowledge and inspiration days. Beyond that, the projects hardly sought each other out."* (R2, ch. 8, p. 67 of the PDF)

> "Op de Kennisdag van het Oranje Fonds op 30 maart 2017 bleek dat de projecten in hun enthousiasme vooral hun eigen successen delen op de pagina, leren is toch ingewikkelder in het openbaar. Projectleiders delen foto's van geslaagde dagen. Inhoudelijke vragen die een aantal projectleiders stellen, sneeuwen onder in de veelheid aan foto's van geslaagde evenementen."
> — *"At the Oranje Fonds Kennisdag of 30 March 2017 it turned out that the projects, in their enthusiasm, mainly share their own successes on the page; learning is more complicated in public. Project leaders share photos of successful days. Substantive questions that some project leaders ask get buried in the mass of photos of successful events."* (R2, p. 66–67)

> "Het Oranje Fonds heeft voor de projectleiders van de initiatieven een gezamenlijke Facebookgroep aangemaakt, wel uitdrukkelijk alleen voor leden."
> — *"The Oranje Fonds created a joint Facebook group for the initiatives' project leaders, expressly members-only."* (R2, p. 66)

> "Sinds het afgelopen jaar durf ik meer mensen om hulp te vragen: 4/10 waar." … "Sinds het afgelopen jaar sta ik eerder voor andere mensen klaar: 5/10 waar." … "Ik heb het afgelopen jaar nieuwe mensen leren kennen in de buurt: 9/10 waar."
> — the three retrospective change items, period average (R2, Samenvatting p. 4). **Note the internal inconsistency:** the body text says "Ongeveer een derde van de vrijwilligers geeft elk jaar aan meer mensen om hulp te durven vragen" (~a third each year), against the 4/10 period average in the summary. Reported as the source gives it; the direction is the same.

> "Om hulp vragen is altijd moeilijker dan hulp bieden, zeker voor vrijwilligers. Dat blijkt in ons onderzoek naar Groen Verbindt, maar ook andere onderzoeken laten zien dat zelf hulp vragen voor vrijwilligers altijd ingewikkeld is."
> — *"Asking for help is always harder than offering help, certainly for volunteers. That is evident in our research on Groen Verbindt, but other studies also show that asking for help oneself is always complicated for volunteers."* (R2, p. 37 area; the report's own interpretation of its own numbers)

> "Gemiddeld zijn per project drie à vier betaalde medewerkers werkzaam geweest de afgelopen periode (2016: 3,6, 2017: 3,8, 2018: 3,2) die samen ongeveer 12 uur per week aan het project besteedden."
> — *"On average three to four paid staff worked on each project over the period, together spending about 12 hours a week on it."* (R2, §4.1)

> "Zeker gecombineerd met de prognose die projectleiders geven van het aantal betaalde uren dat over zal blijven voor de projectvoering nu het programma Groen Verbindt afloopt en het Oranje Fonds de ondersteuning stopt. In veel gevallen komen er minder betaalde uren beschikbaar voor de coördinatie van het project."
> — *"Especially combined with the forecast project leaders give of the paid hours that will remain for running the project now that the Groen Verbindt programme is ending and the Oranje Fonds is stopping its support. In many cases fewer paid hours become available for coordinating the project."* (R2, §4.1)

> "Als coördinator [en] kartrekker kun je je uitgeblust en eenzaam voelen als het niet lekker loopt. Je voelt je verantwoordelijk voor zaken waarop je geen invloed hebt."
> — *"As coordinator and driving force you can feel exhausted and lonely when things are not going well. You feel responsible for things you have no influence over."* (R2, quoted coordinator, on the coaching it received)

> "In twaalf van de 23 projecten die gebruik maakten van de coaching van Van de Bunt ging de coaching over de samenwerking tussen de coalitiepartners." … coordinators rated the coaching 8.3 (2017) and 8.6 (2018).
> — *"In twelve of the 23 projects that used Van de Bunt's coaching, the coaching was about cooperation between the coalition partners."* (R2, §8.4) — i.e. what helped was **advice about a specific partnership**, not a peer network.

### 3.2 R1 — Trefpunt Groen's own account of what it gives and receives

> "Wij coördineren de inspraak van lokale natuur- en milieugroepen en andere betrokkenen uit onze achterban, die allen een vitale bijdrage leveren aan de kwaliteit van het advies."
> — *"We coordinate the input of local nature and environmental groups and other stakeholders from our achterban, who all make a vital contribution to the quality of the advice."* (R1, p. 25)

> "TGE coördineert de inbreng, meningen en adviezen van natuur-, groen-, en andere aangesloten groeperingen die in Eindhoven actief zijn en is verantwoordelijk voor een goede communicatie met haar achterban en om binnen de afgesproken termijnen advies naar de gemeente uit te brengen."
> — *"TGE coordinates the input, opinions and advice of nature, green and other affiliated groups active in Eindhoven, and is responsible for good communication with its achterban and for delivering advice to the municipality within the agreed deadlines."* (R1, p. 26, summary of the samenwerkingsprotocol)

> "De samenwerking heeft een meerledig doel; het kwalitatief verbeteren van de voorliggende plannen … het vergroten van het maatschappelijk draagvlak en de kans op bezwaarprocedures verkleinen."
> — *"The cooperation has a multi-part aim: improving the quality of the plans … increasing public support and reducing the chance of objection procedures."* (R1, p. 26) — the city's side of the exchange is stated as **reduced objection risk**.

> "De kapadviezen van TGE zijn bindende adviezen."
> — *"TGE's tree-felling advices are binding advices."* (R1, p. 9)

> "Mede dankzij de samenwerking tussen Trefpunt Groen Eindhoven, Bibliotheek Eindhoven, KNNV Eindhoven, het Wasven en IVN Veldhoven Eindhoven Vessem zijn er in 2025 acht drukbezochte Groen Cafés georganiseerd" … "Tijdens deze meetings wisselden we ideeën uit en inspireerden we elkaar om samen te werken aan een groener en gezonder Eindhoven."
> — *"Partly thanks to the cooperation between [five named organisations], eight well-attended Groen Cafés were organised in 2025 … During these meetings we exchanged ideas and inspired each other to work together."* (R1, p. 10–11)

> Urenverantwoording 2025 (hours statement): *afstemming achterban* **15%**, *netwerk intensiveren* **5%**, communicatie 20%, kapaanvragen adviseren 20%, omgevingsplannen adviseren 25%, overige projecten 10%, management en administratie 5%.
> — (R1, p. 22) i.e. **one fifth of a paid intermediary's time is the relational work itself.**

> "Het aantal leden in onze achterban neemt toe en we hebben nieuwe contacten gelegd met enkele groene groepen die actief zijn in verschillende wijken in Eindhoven."
> — *"The number of members in our achterban is growing and we have made new contacts with some green groups active in various neighbourhoods."* (R1, p. 17) — [C], its own claim, with no list published.

> Financials: netto omzet 2025 **€232,000**; personeelskosten **€195,795**; two coordinators and one communications staff (R1, p. 20, 25).

### 3.3 R3 — the municipality designing a back office

> "Er wordt onderzocht of een paraplustichting (een stichting die het besturen en de lasten van rechtspersonen voor een groot deel overneemt) uitkomst kan bieden."
> — *"It is being investigated whether an umbrella foundation (a foundation that takes over much of the governing and the burdens of legal persons) can help."* (R3, §1.1)

> "Het opzetten van een 'flexpool' voor vrijwilligers. Het wordt zo eenvoudiger om je flexibel in te zetten als vrijwilliger. Zowel in tijd als in de plek waar het werk wordt gedaan."
> — *"Setting up a 'flexpool' for volunteers. That makes it easier to deploy yourself flexibly as a volunteer, both in time and in the place where the work is done."* (R3, §1.1)

> "vrijwilligersorganisaties ervaren veel regeldruk … het aantal Eindhovenaren dat zich vrijwilliger noemt neemt al jaren af terwijl de vraag naar vrijwilligers toeneemt."
> — *"volunteer organisations experience a lot of administrative burden … the number of Eindhoven residents who call themselves volunteers has been falling for years while demand for volunteers is rising."* (R3, §1.1)

> "Er wordt onderzocht welke mogelijkheden er zijn voor een centrale vertrouwenspersoon en/ of vertrouwenscontactpersoon voor vrijwilligers."
> — *"Possibilities are being investigated for a central confidential adviser and/or confidential contact person for volunteers."* (R3, §1.1)

> Money: VSB volunteer ceiling **€1,420,000**, of which the *vrijwillige inzet* theme **€1,369,000**; **€300,000** GALA ceiling for the one-off items (flexpool, paraplustichting, confidential adviser); **vrijwilligersverzekering €32,000** (R3, §Financiële consequenties). First visible results "in Q3 en Q4 van 2025"; evaluation 2026.

### 3.4 R4 — the Klusbus, correctly identified

> "Gemeente Eindhoven kreeg op 6 juli 2023 van het ministerie van BZK een specifieke uitkering (SpUk) van € 3.699.000,- voor de aanpak van energiearmoede." … "Een groot deel van de middelen wordt nu besteed aan de Eindhovense Klusbus (22bst01094). Dit project wordt samen met de woningcorporaties in het Duurzaamheidspact uitgevoerd."
> — *"The municipality received a specific grant for tackling energy poverty … A large part of the funds is now spent on the Eindhoven Klusbus. This project is carried out together with the housing corporations in the Duurzaamheidspact."* (R4, p. 1)

> "In 2023 zijn er ruim 9.000 huishoudens voorzien van kleine energiebesparende maatregelen" … "Het is het juiste moment om te verlengen en door te ontwikkelen"
> — (R4, p. 2) The Klusbus is a **mobile energy-saving service to households**, not a tool library and not green-initiative infrastructure. See `note.md` §7 for the correction this forces on a sibling note.

### 3.5 R5 — Wasven's internal mutual-support architecture

> "Onze vrijwilligers zijn georganiseerd in werkgroepen. We werken samen onder deskundige leiding en je steekt er wat van op." … "De vrijwilligers in het Wasven zijn actief in vele werkgroepen, ondersteund en begeleid door teamleiders."
> — *"Our volunteers are organised in working groups. We work together under expert guidance and you learn something from it." … "supported and supervised by team leaders."* (R5)

> "Als chauffeur van het Wasven is de flexibiliteit super fijn. Als iemand een keer niet kan, staat er gelijk een ander klaar om jouw dienst over te nemen. Hierdoor is er ruimte om je eigen tijd in te delen. Een van ons rijdt bijvoorbeeld één keer in de 14 dagen zijn rit en een ander rijdt wel 5 keer per week."
> — *"As a Wasven driver the flexibility is great. If someone can't make it, someone else is immediately ready to take over your shift. That leaves room to arrange your own time. One of us drives once a fortnight and another drives five times a week."* (R5, volunteer quoted on the site) — **unequal contribution inside a rota that absorbs it.**

> "We werken samen met Eindhoven Doet en streven naar het certificaat 'Goed Geregeld'."
> — *"We work with Eindhoven Doet and aim for the 'Goed Geregeld' certificate."* (R5) — the matching platform is **volunteer-to-organisation**, and the certification is a quality mark for volunteer management.

> Rhythm examples: Natuurbeheer "iedere maandagavond en de eerste en derde zaterdag van de maand … In de wintermaanden iedere zaterdagochtend"; Tuinderij "maandag, woensdag en vrijdag en eenmaal in de twee weken op zaterdagochtend"; Winkel "Vast schema" (R5).

### 3.6 R6 — Struikroven: reciprocity with a third party paying the bill

> "Struikroven begon als buurtinitiatief in Eindhoven in 2017 en groeide uit tot een landelijke stichting in 2020." … "Ons team van ca 50 lokale Struikrovers uit heel Nederland, zet zich in voor een groenere toekomst, ondersteund door onze landelijke organisatie."

> "Alle opbrengsten van de Struikroofacties investeren we in onze missie." … "Struikroven inhuren" (site navigation) … "Struikroven sluit naadloos aan bij duurzaamheidsdoelen én gemeentelijke eisen rondom buurtparticipatie, zoals verplicht vanuit de Omgevingswet."
> — *"We invest all proceeds of Struikroof actions in our mission." … "Hire Struikroven" … "fits seamlessly with sustainability goals and municipal requirements around neighbourhood participation, as required by the Environment Act."* (R6) — the plants go free to residents; the **commissioning developer or corporation pays**; the participation obligation is the demand.

### 3.7 R7 — what arrived at the closure, and what did not

> "Met pijn in mijn hart moet ik laten weten dat Voedselbos Eindhoven met onmiddellijke ingang gesloten is. Na meer dan 12 jaar … Dit had nooit gekund zonder alle vrijwilligers die iedere vrijdag hebben meegebouwd aan een volwassen voedselbos vol fruit, noten, bloemen en eetbaar groen."
> — (R7, post 28-07-2026)

> "De afgelopen dagen stroomt mijn mailbox over met lieve en hartverwarmende berichten, steun, herinneringen én uitnodigingen om op nieuwe plekken voedselbossen te ontwikkelen en samen verder te bouwen aan een gezonde en duurzame toekomst."
> — *"In recent days my mailbox has been overflowing with kind and heartwarming messages, support, memories and invitations to develop food forests in new places and to keep building together."* (R7) — offers **to** the closing party; the record shows no documented transfer **from** it.

> "Samenwerken staat voorop in ons voedselbos" … "elkaar kunnen ontmoeten, van elkaar kunnen leren" (R7, mission statement, undated) — an ambition, not a documented practice.

> The closure post links "Nieuwsbrief november 2026 over Voedselbos Eindhoven: **Nieuws van Natuurlijk Maartje**" — the audience continuation is **named after one person** (R7). [I] The one asset that survived the place is held individually, not collectively.

### 3.8 R8 — the seed library: the clearest documented reciprocity design in the city

> "Kom langs om zaden en plantjes te ruilen, lenen en/of te doneren. Breng je eigen zaden, plantjes of stekjes mee of als je die niet hebt, iets anders wat je zou willen ruilen."
> — *"Come and swap, borrow and/or donate seeds and plants. Bring your own seeds, plants or cuttings, or if you don't have any, something else you would like to swap."* (R8)

> "Zadenbibliotheek De Nootzaak is een initiatief om de tuinen en tuinmensen van Eindhoven met elkaar te verbinden. In de kelder van De Fabriek kunnen de gedeelde zaden koel en droog worden bewaard. Een aantal keer per jaar gaat de zadenbibliotheek open, en kunnen zaden worden geleend of teruggebracht. Op die dagen zorgen we ook voor een workshop, een lezing, een proeverij of een film."
> — *"…an initiative to connect the gardens and gardeners of Eindhoven. In De Fabriek's cellar the shared seeds can be kept cool and dry. A few times a year the seed library opens and seeds can be borrowed or returned. On those days we also provide a workshop, a lecture, a tasting or a film."* (R8)

> "Deelname aan het programma is gratis." (R8). Host: **De Fabriek**, an art/creative venue, not a green initiative. Present status in 2026 is **[U]** — the retrieved page is the 19 April 2025 opening event.

### 3.9 R9 — a twice-yearly swap market with an archive

> "Elk voorjaar en najaar organiseren we een ruilbeurs voor plantjes, stekken, zaden." … "De volgende ruilbeurs is gepland voor 24 april 2027."
> — *"Every spring and autumn we organise a swap market for plants, cuttings, seeds … The next is planned for 24 April 2027."* (R9) Runner: a membership association ("Word lid", "bestuur"), with a "Terugblikken" archive of past editions.

### 3.10 R10 — the one attempt at shared tool lending, withdrawn

> "Er in Zweden veelvuldig gebruik wordt gemaakt van 'spullen bibliotheken' waar zaken zoals speelgoed, maar ook **(tuin)gereedschap**, kampeerartikelen en muziekinstrumenten geleend kunnen worden" … "De raad roept het college op om: 1. Daar waar mogelijk in de nieuw te ontwikkelen 'Huizen van de Wijk' ruimte te zoeken waar spullen kunnen worden opgeslagen en uitgeleend".
> — (R10, p. 1)

> "**Deze motie is ingetrokken (toezegging wethouder) in de vergadering van 15 april 2025.**"
> — *"This motion was withdrawn (on an alderman's commitment) in the meeting of 15 April 2025."* (R10, closing line, emphasis in the document) — the outcome of the commitment is **[U]**.

---

## 4. Searches and retrievals that produced nothing usable (negative evidence, 26-11-2026)

- No retrieved source documents **tool or equipment lending between Eindhoven green initiatives**, or between an initiative and a municipal facility. The only garden-tool lending proposal found (R10) was withdrawn.
- No retrieved source documents a **volunteer swap between two named Eindhoven green initiatives**, in either direction. Experiment A in [`../experiments/note.md`](../experiments/note.md) exists precisely because it is not documented.
- No retrieved source documents **joint purchasing or a joint funding application** by two named Eindhoven green initiatives.
- No retrieved source documents a **shared back office** actually in operation between initiatives; the umbrella foundation is at the stage of being "onderzocht" (R3).
- No retrieved source documents an initiative **refusing** to share something, or being refused by a peer. See `note.md` §6 for why that absence should not be read as harmony.
- No retrieved first-person account by a member of Trefpunt Groen's *achterban* of what that relationship costs or gives them. The relation is documented entirely from the intermediary's side (R1).
- `wasven.nl/vrijwilligers/` 404; `thenewblock.nl` parked; `groenbennekel.nl` a shell; Facebook/Instagram groups login-walled — inherited from the sibling notes and not retried here.
