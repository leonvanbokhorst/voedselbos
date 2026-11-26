# Line A — source register: the Dutch-language money-and-positioning record

Retrieval date for every source below: **26 November 2026** (all retrievals between 22:02 and 22:06 UTC).
Retrieval channel: `source_read` only (Web Bot Auth signed; unsigned for web.archive.org fetches, as reported).
Marks used in the findings file: [D] documented · [C] claimed by an actor · [I] inference · [U] not established.

Convention: "sha256" is the digest `source_read` reported for the exact retrieved bytes.

---

## A1 — Wasven, "Verantwoording"
- Publisher: Stichting Wasven (wasven.nl)
- Date: undated page (sitemap lastmod 2026-05-13)
- URL: https://wasven.nl/verantwoording/
- Obtained: full page text (HTML→text)
- sha256: `25e29490422f1ad05fdba198a5ea2f5a8f33a4cfb3cd5b24ba3f205723e2cb86`
- Access: 200

Verbatim:
> "Het Wasven is organisatorisch en financieel zelfstandig. De drie stichtingen vormen tezamen een fiscale eenheid voor de omzetbelasting. Financiële rapportage vindt plaats per stichting."

> "De kwaliteit van zorg is verankerd in de raad van toezicht via de Governancecode Zorg en geborgd in het keurmerk 'Kwaliteit laat je zien'."

Read depth: full page. Note: HTML→text extraction **stripped all hrefs**, so the three document links named on the page ("Jaarverslag publicatie ANBI", "Maatschappelijk jaaroverzicht", "Kwaliteitszorg Jaarverslag") could not be resolved from this page alone. Resolved instead via A3/A4 (see recovery ladder in the findings file, §d).

---

## A2 — Wasven, "Jaarverslag publicatie ANBI"
- URL: https://wasven.nl/financieel-jaarverslag/
- Date: undated page (sitemap lastmod 2026-07-03)
- Obtained: full page text (HTML→text)
- sha256: `17cdbc688d905c8c2638a4edf0d3c8bfbeccd4d0e7ca404b911b9e113f8520c0`
- Access: 200

Verbatim (the entire body of the page):
> "Publicatiebericht ANBI
> Publicatie ANBI stichting Wasvenboerderij 2025
> Publicatie ANBI stichting Groendomein Wasven 2025
> Publicatie ANBI stichting Wasvenzorg 2025"

Read depth: full page. Links stripped by extraction → resolved via A3.

---

## A3 — WordPress REST API: page object for `financieel-jaarverslag`
- Publisher: wasven.nl (site's own API)
- URL: https://wasven.nl/wp-json/wp/v2/pages?slug=financieel-jaarverslag&_fields=id,slug,link,modified,content
- Obtained: JSON, full rendered page content **including href values**
- sha256: `537d9dfc81f71096cf78bc2e5b02d6e38dbf0ab15257984a4c82643e75945808`
- Access: 200

This is the methodological key that unlocked the PDFs. Verbatim fragments of the `href` attributes:
> `https:\/\/wasven.nl\/wp-content\/uploads\/2026\/07\/ANBI-Wasvenboerderij-2025-juni-2026-def.pdf`
> `https:\/\/wasven.nl\/wp-content\/uploads\/2026\/07\/ANBI-Groendomein-Wasven-2025-juni-2026-def.pdf`
> `https:\/\/wasven.nl\/wp-content\/uploads\/2026\/07\/ANBI-Wasvenzorg-2025-juni-2026-def.pdf`

Read depth: full JSON (3,162 bytes).

---

## A4 — WordPress media API: search "ANBI"
- URL: https://wasven.nl/wp-json/wp/v2/media?search=ANBI&per_page=20&_fields=id,date,source_url,title
- Obtained: JSON inventory of 12 media items
- sha256: `226ac705bd20c2d07a6a06ad26de6d98f98909631e034ddb2088becbf6598ca2`
- Access: 200

Establishes the document series and its publication dates (not just the current year):
> `{"date":"2026-07-03T20:04:46","title":{"rendered":"ANBI Wasvenzorg 2025 juni 2026 def"}, ...}`
> 2024 series: `ANBI-Publicatie-2024-{Wasvenzorg,Wasvenboerderij,Groendomein-Wasven}-def-nw.pdf`, dated 2025-12-11
> Beleidsplannen: `ANBI-Beleidsplan-{Wasvenzorg,Wasvenboerderij,Groendomein-Wasven}-2021-2026-V05.pdf`, dated 2025-12-09

Read depth: full JSON.

---

## A5 — "Standaardformulier publicatieplicht ANBI Algemeen" — Stichting Wasvenboerderij, boekjaar 2025
- Publisher: Stichting Wasvenboerderij (self-published ANBI form, Belastingdienst template)
- Date: PDF uploaded 2026-07-03; balance date 31-12-2025
- URL: https://wasven.nl/wp-content/uploads/2026/07/ANBI-Wasvenboerderij-2025-juni-2026-def.pdf
- Obtained: **full PDF text, 6 pages** (pdftotext)
- sha256: `346b578b3bf07259b2a97206582103148876e01fb5b3baca60415f937f959c19`
- Access: 200

Identity: KvK 17198973; RSIN 817342539; Celebeslaan 30, 5641 AG Eindhoven; sectors "Natuur en milieu" + "Welzijn - Overig welzijnswerk".

Staffing (p.1):
> "Aantal medewerkers (*) 1 5 — Betaalde personeelsleden in gemiddeld aantal fte gedurende het boekjaar."
> "Aantal vrijwilligers (*) 3 0 — Vrijwilligers die zich regelmatig (meer dan 3 keer per jaar) inzetten voor uw instelling."

Statutory purpose and activities (pp.2–3):
> "a) het huren van de Wasvenboerderij en exploiteren als gasterij met zaalverhuur, bakkerij en koffiebranderij met winkel en tuinderij met natuurakkers,"
> "Het accent ligt in financieel opzicht op de werkzaamheden a en b en in organisatorisch opzicht bij de werkzaamheden c, d en e."

Income sources declared (p.2):
> "Het vermogen van de stichting wordt gevormd door: a) project- en evenementensubsidies, b) donaties en giften, c) inkomsten uit maatschappelijke exploitatie en d) netto inkomsten uit activiteiten."

Staat van baten en lasten (p.5), boekjaar 2025 with 2024 comparative:
> "Baten als tegenprestatie voor levering van producten en/of diensten (omzet) € 1.192.085 | € 1.042.519"
> "Som van alle baten € 1192085 | € 1042519"
> "Subsidies van overheden € [blank] | € 0"
> "Baten sponsorbijdragen € [blank] | € 0"; "Giften … € [blank]"
> "Inkoopwaarde van geleverde producten (kostprijs) € 440.846"; "Personeelskosten € 524.408"; "Huisvestingskosten € 183.580"; "Som van de lasten € 1.177.528"
> "Saldo van baten en lasten € 14.557 | € 6.803"

Read depth: **full document**. All figures above are from the complete statement, not a fragment.

---

## A6 — ANBI-formulier — Stichting Groendomein Wasven, boekjaar 2025
- URL: https://wasven.nl/wp-content/uploads/2026/07/ANBI-Groendomein-Wasven-2025-juni-2026-def.pdf
- Obtained: full PDF text, 6 pages
- sha256: `536b174941adf40c20499ce7b425ffb3bf15f133c16144cafe9d8283a18e0568`
- Access: 200

Identity: KvK 17176851; RSIN 814421635.

Staffing (p.1):
> "Aantal medewerkers (*) 0 — Betaalde personeelsleden in gemiddeld aantal fte gedurende het boekjaar."
> "Aantal vrijwilligers (*) 1 5 0"

**The pivotal sentence on land and the municipality** (p.2, "Welke werkzaamheden verricht de instelling?"):
> "b) het beheren en onderhouden van de opstallen en het groen conform de beheerovereenkomst met de gemeente Eindhoven,"

Full activity list:
> "a) het verhuren van de Wasvenboerderij aan stichting Wasvenboerderij en stichting Wasvenzorg en de woning aan de boerderijmeester (beheerder), b) het beheren en onderhouden van de opstallen en het groen conform de beheerovereenkomst met de gemeente Eindhoven, c) het uitvoeren van verbeterprojecten in het Wasven vanuit een duurzame, toekomstgerichte visie op het groendomein Wasven, d) het organiseren van maatschappelijke activiteiten die de sociale en fysieke leefbaarheid van de omgeving vergroten, e) het aangaan van wederkerige relaties en samenwerking met leveranciers, vrijwilligers en lokale organisaties waardoor sociale netwerken worden versterkt."

Staat van baten en lasten (p.5):
> "Giften en donaties van particulieren € 997 | € 441"; "Overige giften € 27.600 | € 2.940"; "Giften € 28.597 | € 3.381"
> "Baten als tegenprestatie voor levering van producten en/of diensten (omzet) € 385.500 | € 307.612"
> "Baten van subsidies € 0 | € 0"
> "Personeelskosten € 136.548 | € 105.026"; "Som van de lasten € 400.406"
> "Saldo van baten en lasten € 13.691 | € -40.790"

Balance (p.4): "Materiële vaste activa € 1.473.904"; "Langlopende schulden € 1.202.413"; "Continuïteitsreserve € 268.068"; totaal € 1.560.178.

Read depth: **full document**.

---

## A7 — ANBI-formulier "Zorginstellingen" — Stichting Wasvenzorg, boekjaar 2025
- URL: https://wasven.nl/wp-content/uploads/2026/07/ANBI-Wasvenzorg-2025-juni-2026-def.pdf
- Obtained: full PDF text, 6 pages
- sha256: `22793210facfdfbc0e665088c41e05587803a4a00da923a9d1f217a1dd54c295`
- Access: 200

Identity: KvK 62086839; RSIN 854641051.

> "Aantal medewerkers (*) 0 — Betaalde personeelsleden in gemiddeld aantal fte gedurende het boekjaar."

The dependence on the municipal/Wmo care market is stated in the foundation's own words (p.2):
> "Gezien de te verwachte marktschommelingen in deelnemers als gevolg van de WMO streeft de stichting naar een eigen vermogen van maximaal een halfjaaromzet."

Staat van baten en lasten (p.5):
> "Opbrengsten zorgprestaties en maatschappelijke ondersteuning € 457.610 | € 407.574"
> "Subsidies € 0 | € 0"; "Overige bedrijfsopbrengsten € 0"
> "Totaal baten € 457.610 | € 407.574"
> "Personeelskosten € 353.388 | € 322.846"; "Huisvestingslasten € 54.246"; "Overige bedrijfskosten € 49.876"; "Som der bedrijfslasten € 457.510"
> "Resultaat € 610 | € -15.634"

Read depth: **full document**.

---

## A8 — "Jaaroverzicht 2025" (Wasven maatschappelijk jaaroverzicht)
- Publisher: Stichting Wasven
- Date: PDF uploaded 2026-01-04
- URL: https://wasven.nl/wp-content/uploads/2026/01/Jaaroverzicht-2025.pdf
- Obtained: full PDF text (a designed, magazine-style document)
- sha256: `9d33abf56c16cbf189cb3bc3e81f6538f36e6ba0197f74bb8c808dd8ccfa140b`
- Access: 200

The 2025 activity narrative. Named collaborators/counterparties in 2025 (all quoted verbatim):
> "Op de vrije akker zijn fruitbomen en struiken aangeplant volgens de bos-landbouw methode Agroforestry."
> "Op de laatste dag kon je met stichting Wereldboom de boom in en leerden designers je anders kijken naar de natuur."
> "Als blijk van dank trakteerde NH1816 en lokale verzekeraars alle deelnemers en vrijwilligers op een vrijkaartje voor Van Gogh Village Nuenen."
> "Terwijl vrijwilligers op zaterdagochtend de handen uit de mouwen steken maken de sporters van Get Running zich op voor hun work-out in het groen. Terloops ontstond het idee voor de Wasvenloop; een halve marathon door het Ecotopisch Dommeldal"
> "Studenten van de TUe brachten een bezoek voor het vak duurzame bedrijfsmodellen."
> "Het programma Binnenste Buiten maakte een aflevering met onze deelnemer Nick in de hoofdrol."

Read depth: full document. **Note:** the word "voedselbos" does not occur anywhere in this document; the Wasven describes its own tree-based production as "agroforestry" and "notengaard".

---

## A9 — "Beleidsplan 2021 – 2026", Stichting Groendomein Wasven (V05)
- Author/date: Alfred van Kempen, January 2021 (uploaded 2025-12-09)
- URL: https://wasven.nl/wp-content/uploads/2025/12/ANBI-Beleidsplan-Groendomein-Wasven-2021-2026-V05.pdf
- Obtained: full PDF text, 7 pages
- sha256: `966349eadb0fafd52ec541a515675c9728a6325b5b1a38dc754b6c8e1fc3518d`
- Access: 200

On ownership (p.2):
> "Het Wasven wordt gevormd door drie organisaties: stichting Groendomein Wasven is eigenaar en beheerder van het groendomein Wasven, stichting Wasvenboerderij exploiteert de voorzieningen en stichting Wasvenzorg begeleid mensen met een zorgvraag vanuit de Wasvenboerderij."

Governance self-description (p.2):
> "Gezien de wederkerige relaties is een Raad van Toezicht benoemd, zodat de balans tussen de stichtingen financieel en beleidsmatig gewaarborgd blijft."

Intercompany lending (p.5):
> "Vanaf de opstart zijn leningen verstrekt aan stichting Wasvenboerderij en stichting Wasvenzorg. Deze zijn van tijdelijke aard en noodzakelijk om een duurzame exploitatie te kunnen realiseren. De leningen zijn aangegaan tegen een marktconforme, zakelijke rente en verkeren in afbouwfase."

Read depth: full document.

---

## A10 — Wasven, "Partners" (index page)
- URL: https://wasven.nl/partners/
- Obtained: full page text — **but body content is empty in the text extraction** (partner entries are logo images in a grid)
- sha256: `115e6a14352bd7cdc46979de455714b91bb32171c714a1107d731ffb86bba707`
- Access: 200

Read depth: page read; the substantive content is not recoverable as text. The partner *identities* were recovered from A11 (sitemap) instead. This is a read-depth limitation and is flagged as such: **A10 itself yields no usable text.**

---

## A11 — Wasven page sitemap
- URL: https://wasven.nl/wp-sitemap.xml → redirected to https://wasven.nl/sitemap_index.xml, then read https://wasven.nl/page-sitemap.xml
- Obtained: full XML (20,999 bytes)
- sha256: `89c46ab9101546625ea3c4729c71fbb653ed5edbd3ba006c96d53fc185650c5b`
- Access: 200 (redirect followed)

Enumerates the partner pages, i.e. Wasven's own published list of its affiliations/keurmerken:
> `/partners/eko-restaurant-zilver/`, `/partners/ongehinderd/`, `/partners/fietsers-welkom/`, `/partners/skal/`, `/partners/kwaliteit-laat-je-zien/`, `/partners/governancecode-zorg/`, `/partners/anbi/`, `/partners/wereldboom/`, `/partners/trefpunt-groen-eindhoven/`, `/partners/green-key-goud/`, `/partners/sustainable-development-goals/`, `/partners/social-return/`, `/partners/goed-geregeld/`, `/partners/kern-met-pit/`, `/partners/geluksplek/`, `/partners/erkend-leerbedrijf/`, `/partners/samen-voor-eindhoven/`

Read depth: full.

---

## A12 — Wasven, "Trefpunt Groen Eindhoven" (partner page)
- URL: https://wasven.nl/partners/trefpunt-groen-eindhoven/
- Obtained: full page text
- sha256: `08d721397b1d360091611f8712f235b1e0ac528dbd6b3817e8ac9829866e2a3f`
- Access: 200

Verbatim, in full — the single most quotable positioning statement retrieved in this line:
> "Trefpunt Groen Eindhoven is de waakhond van de groene leefomgeving in Eindhoven. Het Trefpunt zit vanaf de planvorming met de gemeente om tafel en geeft advies over natuur, milieu, ecologie, duurzaamheid en cultuurhistorie. Bij Trefpunt Groen Eindhoven zijn ruim honderd groepen aangesloten, waaronder het Wasven. Al sinds de oprichting in 2002 werken we samen om de kwaliteit van de leefomgeving te verbeteren."

Read depth: full.

---

## A13 — Wasven, "Samen voor Eindhoven" (partner page)
- URL: https://wasven.nl/partners/samen-voor-eindhoven/
- Obtained: full page text
- sha256: `caf7f3ee36fe30a423052429bcc2ba50d8342cdd8c83c89a033306e3921295be`
- Access: 200

> "'Samen voor Eindhoven' biedt bedrijven in de Brainportregio de mogelijkheid om hun medewerkers in te zetten als vrijwilliger. Andersom ondersteunt de stichting maatschappelijke organisaties bij het opzetten van partnerschappen met bedrijven.
> Het Wasven is één van de maatschappelijke partners waar medewerkers van bedrijven kunnen meehelpen op onze akkers of in het groen. Dit kan door het organiseren van een teamdag onder de noemer 'Groene Daden' of door deel te nemen aan de jaarlijkse NL Doet of de Natuurwerkdag."

Read depth: full.

---

## A14 — Wasven, "Groen" (groendomein landing page)
- URL: https://wasven.nl/groendomein/
- Obtained: full page text
- sha256: `4479543d9e82aead06032b15937ba7815faa42d7f04fa729829b109929df6979`
- Access: 200

> "Het groendomein Wasven is een combinatie van landgoed en landbouw, waar mens, dier en plant al eeuwen samenleven."
> "Landschap — Groene oase, ecologisch beheerd door vrijwilligers. Onderdeel van natuurwerk Brabant"
> "Erfgoed — Gemeenschappelijk bezit, voor en door buurtbewoners die de verantwoordelijkheid nemen."

Read depth: full. **No hectare figure appears on this page** — relevant to the "~24 ha" question (see findings §d).

---

## A15 — Wasven, "Basisdagbesteding"
- URL: https://wasven.nl/zorg/basisdagbesteding/
- Obtained: full page text
- sha256: `d79fbbf043e8e5c2407f758bb577e866c0a71ab92259778a86fe13857712ace2`
- Access: 200

> "De basisdagbesteding is gericht op sociale interactie. Door doen en meedoen, vanuit de eigen mogelijkheden en interesses. In de tuinderij en het groene domein van het Wasven. De basisdagbesteding is laagdrempelig en voor alle inwoners van Eindhoven met een ondersteuningsvraag. Een verwijzing vanuit Wij Eindhoven is gewenst."

Read depth: full.

---

## A16 — Gemeente Eindhoven, "Groensubsidie aanvragen"
- Publisher: gemeente Eindhoven (eindhovenduurzaam.nl)
- Date: undated page, © 2026
- URL: https://www.eindhovenduurzaam.nl/groensubsidie-aanvragen
- Obtained: full page text
- sha256: `279c3b3addfab1c6ee110133221c589e29703c405dbad3d229326bb0234b1408`
- Access: 200

The decisive characterisation — this is a **private-property** scheme, not an initiative-funding scheme:
> "Wil je je tuin groener maken, een groen dak aanleggen of regenwater beter afvoeren? Met de groensubsidie helpt de gemeente Eindhoven je daarbij. Ben je eigenaar van een woning of (bedrijfs)pand van minimaal 5 jaar oud? Dan kun je een subsidie krijgen voor maatregelen die zorgen voor meer groen en minder wateroverlast."

Three measures with unit rates and per-applicant ceilings:
> "1. Tegels eruit, groen erin … € 5 per m². Je kan maximaal € 2.500 in totaal krijgen. Minimaal 20 m²."
> "2. Aanleggen van een groen dak … € 25 per m². Je kan maximaal € 25.000 in totaal krijgen. Minimaal 10 m²."
> "3. Afkoppelen van de riolering … € 10 per m² dat je afkoppelt. Je kan maximaal € 10.000 in totaal krijgen."

Eligibility conditions: "De werkzaamheden zijn uitgevoerd vanaf 1 januari 2019. Je bent eigenaar van een bestaand terrein dat minstens 5 jaar oud is."

Read depth: full. **No list of recipients is published on this page**, and the scheme is not addressed to organisations running green/community initiatives.

---

## A17 — Gemeenteblad 2025, 87805 — "Voornemen tot uitgifte van grond aan Groendomein Wasven"
- Publisher: Gemeente Eindhoven, Officiële bekendmakingen
- Date: 3 March 2025, 09:00
- URL: https://zoek.officielebekendmakingen.nl/gmb-2025-87805.html (authentieke PDF also linked; extern bijlage `exb-2025-7754` "Inventarisatietekening")
- Obtained: full document text (HTML)
- sha256: `d32e27c426475f95c1ac34ed723b8e001ea33b10d3b94a6a516c9b56681e4637`
- Access: 200

The lease terms:
> "De gemeente en stichting Groendomein Wasven beogen een huurovereenkomst voor de uitgifte van de betreffende grond, groot circa 7.306 m2, kadastraal bekend als het perceel Tongelre, sectie D, nummer 712, gelegen tegenover Celebeslaan 30 te Eindhoven. De overeenkomst zal ingaan na het verkrijgen van de Omgevingsvergunning en wordt aangegaan voor een periode van 15 jaar, met de mogelijkheid tot verlenging."

Purpose of the parcel:
> "Binnen het bestaande gebruik heeft de stichting Groendomein Wasven het plan om een klein deel van de grond in te richten als zonneakker, voor ecologisch natuurbeheer en biologische landbouw volgens agroforestry met daarbij teeltondersteunende voorzieningen in de vorm van zonnepanelen."

Sole-candidate award:
> "Op basis van deze argumenten beschouwt de gemeente stichting Groendomein Wasven, volgens objectieve en redelijke criteria, als de enige geschikte kandidaat voor de uitgifte van de grond."

Legal remedy window:
> "Gegadigden die het niet eens zijn met dit gunningsvoornemen kunnen binnen 28 (achtentwintig) dagen, ingaande op de dag na de publicatiedatum van dit voornemen, een kort gedingprocedure starten bij de rechtbank Oost-Brabant"

Read depth: full.

---

## A18 — Gemeenteblad 2026, 14748 — "Voornemen ingebruikgeving grond"
- Date: 15 January 2026
- URL: https://zoek.officielebekendmakingen.nl/gmb-2026-14748.pdf
- Obtained: full PDF text (2 pages)
- sha256: `72714337943f254a5935efa36acadb31080f731385e0d0c4f1b0f500066faa21`
- Access: 200

> "De gemeente Eindhoven maakt hierbij bekend voornemens te zijn om bovengenoemd perceel in gebruik te geven aan Stichting Groendomein Wasven, door middel van een gebruiksovereenkomst. Het perceel vormt onderdeel van het Groendomein Wasven en is gelegen in de zogenoemde Warande. Het gebruik is gericht op ecologisch natuurbeheer, biologische landbouw (agroforestry) en maatschappelijke doeleinden zoals dagbesteding, re-integratie en vrijwilligerswerk."

> "De gemeente is van oordeel dat in dit geval slechts één serieuze gegadigde in aanmerking komt voor de uitgifte van de grond."

Five numbered grounds follow (continuity of management; care/reintegration/volunteer functions not transferable without disruption; part of the ecotopes and the historic Warande; specific expertise; fragmentation risk).

Read depth: full. **Note:** this document refers to "bovengenoemd perceel" without defining the parcel — it is internally incomplete, which is exactly what A19 corrects.

---

## A19 — Gemeenteblad 2026, 24138 — "Rectificatie voornemen ingebruikgeving grond"
- Date: 20 January 2026
- URL: https://zoek.officielebekendmakingen.nl/gmb-2026-24138.pdf
- Obtained: full PDF text (2 pages)
- sha256: `d4c9dd1b47333b0d4fc786c547a3587bcc51f8ade3859cbf78ae0c77d8c9b21f`
- Access: 200

> "Op 15 januari 2026 is er een kennisgeving gepubliceerd (Gemeenteblad 2026, 14748) met betrekking tot het voornemen om een perceel grond in gebruik te geven aan Stichting Groendomein Wasven door middel van een gebruiksovereenkomst. De tekst in de kennisgeving was niet compleet, daarom volgt de kennisgeving hieronder opnieuw."

The parcel (only stated here):
> "betreffende het perceel kadastraal bekend gemeente Tongelre, sectie D, nummer 1121 (gedeeltelijk), ter grootte van circa 9.355 m2, gelegen in het verlengde van de Ceramlaan te Eindhoven."

The legal basis for sole-candidate award:
> "Gelet op het arrest van de Hoge Raad van 26 november 2021, ECLI:NL:HR:2021:1778 (het zogenoemde Didam-arrest) en de daaruit voortvloeiende verplichting voor gemeenten om, ter waarborging van het gelijkheidsbeginsel, voorafgaand aan een gronduitgifte openbaar te motiveren waarom een selectieprocedure wel of niet wordt gehouden."

Read depth: full. **Documented internal discrepancy, recorded as found:** the rectification cites the college decision as "besluit d.d. 13 januari 2025" while the publication is dated January 2026 and concerns the 15 January 2026 notice. I do not resolve this; it is presumably a typo for 2026, but that is [I], not [D].

---

## A20 — Raadsbrief "DAEB-aanwijsbesluit Stichting Groendomein Wasven"
- Publisher: Gemeente Eindhoven, college van B&W
- Date: B&W beslisdatum 10 March 2026; inboeknummer 8136290_03; dossiernummer 26.11.209
- URL: https://raadsinformatie.eindhoven.nl/document/16714650/1/8136290_03+Raadsbrief+DAEB-aanwijsbesluit+Stichting+Groendomein+Wasven?connection_type=17&connection_id=13101216
- Obtained: full PDF text (2 pages)
- sha256: `4afe2d208cae37bbe85a5916b80e7c16920d40e60936d0db241455dcddccc8db`
- Access: 200

The decision:
> "Het college van burgemeester en wethouders heeft besloten het ecologisch beheer van de gemeentelijke gronden van Groendomein Wasven, in samenhang met de daaraan functioneel verbonden collectieve activiteiten van inwoners, aan te wijzen als Dienst van Algemeen Economisch Belang (DAEB) voor de periode 2026–2035."

Continuity framing:
> "Met dit besluit wordt een bestaande samenwerking juridisch en bestuurlijk geborgd. Groendomein Wasven voert al geruime tijd ecologisch beheer uit op gemeentelijke gronden en levert daarmee een bijdrage aan biodiversiteit, klimaatadaptatie en maatschappelijke betrokkenheid in de stad."

The money clause:
> "De DAEB-aanwijzing maakt het mogelijk deze publieke taken rechtmatig te ondersteunen binnen het Europese staatssteunkader. De ondersteuning betreft uitsluitend ecologisch beheer en collectieve, laagdrempelige maatschappelijke activiteiten.
> Voor de uitvoering van de DAEB-taken stelt het college structureel middelen beschikbaar binnen de gemeentelijke begroting. Daarnaast wordt een eenmalige incidentele bijdrage verstrekt voor inrichtingskosten. De afspraken over uitvoering, monitoring en verantwoording worden vastgelegd in een gebruiks- en beheerovereenkomst. Jaarlijks vindt verantwoording plaats; eens per vijf jaar wordt de DAEB-aanwijzing integraal geëvalueerd."

Governance:
> "Er is geen besluitvorming door de raad vereist."

Read depth: full. **No amount is stated anywhere in this document** — "structureel middelen" is unquantified.

---

## A21 — Raadsbrief "Samenwerkingsprotocol gemeente Eindhoven met Trefpunt Groen Eindhoven"
- Date: B&W beslisdatum 11 November 2025; inboeknummer 8022031_03; dossiernummer 25.46.205
- URL: https://raadsinformatie.eindhoven.nl/document/16214623/1/8022031_+03+Raadsbrief+Samenwerkingsprotocol+gemeente+EHV+-+Trefpunt+Groen+Eindhoven?connection_type=17&connection_id=12575893
- Obtained: full PDF text (3 pages)
- sha256: `ff427fb75450a3e932c8867b039a35e5f7744d7719b9c68014f0ba2a2fb4afac`
- Access: 200

Founding purpose and function:
> "In 2001 is Trefpunt Groen Eindhoven (TGE) opgericht met een meerledig doel: het kwalitatief verbeteren van voorliggende plannen op het gebied van groen en natuur, het vergroten van het maatschappelijk draagvlak en de kans op bezwaarprocedures verkleinen."

> "TGE vertegenwoordigt een groot aantal belangenverenigingen in Eindhoven op het gebied van groen en natuur. TGE geeft gevraagd en ongevraagd advies aan de gemeente bijvoorbeeld over ruimtelijke plannen, projecten en kapvergunningen. Dit gebeurt zowel op ambtelijk als bestuurlijk niveau. TGE speelt als koepelorganisatie van groen en milieubelangen in de stad een belangrijke rol in de gemeentelijke democratie, brengt zaken die bij burgers spelen in de stad gecoördineerd naar voren richting gemeente, en andersom speelt TGE een aanvullende rol bij de communicatie naar buiten van zaken die in de gemeente spelen. **Jaarlijks ontvangt TGE subsidie van de gemeente op basis van een ingediend werkplan.**"

> "Het college heeft het samenwerkingsprotocol op 23 september 2025 vastgesteld."

Read depth: full. Note: the annexes to this raadsbrief (the protocol itself, "Werkafspraken", "Centraal Milieu Overleg", "Was-wordt-tabel") were **not obtained** — see A22′/failures F1.

---

## A22 — "Subsidies in Eindhoven – 2025" (Woo-publication of outgoing subsidies)
- Publisher: Gemeente Eindhoven
- Date: publication file dated 2025-05; dataset frozen at awards up to 6 March 2025 for subsidy year 2025
- URL: https://www.eindhoven.nl/sites/default/files/2025-05/Subsidies%20in%20Eindhoven%20%E2%80%93%202025.pdf
- Obtained: **full PDF text, 55+ pages** (the largest single document in this line; ~153,000 characters extracted)
- sha256: `9d0a0221dfdcd1c20646c562955bf37030252fd722190b94125b6c54a58dc942`
- Access: 200

Purpose and scope of the publication:
> "In het kader van de Wet open overheid (Woo) maakt gemeente Eindhoven haar uitgaande subsidies, evenals eerdere jaren, inzichtelijk door middel van deze publicatie."
> "Per verleende subsidie wordt in deze publicatie aangegeven wie de subsidie ontvangt, voor welk project/welke activiteiten, en de hoogte van het subsidiebedrag."
> "Deze publicatie is een momentopname. Alleen subsidies zijn opgenomen die tot 6 maart 2025 zijn verleend en die betrekking hebben op het subsidiejaar 2025."
> "Ongeveer 12% van alle uitgaven van de gemeente Eindhoven zijn uitgaande subsidies."
> "De jaarlijkse publicaties zijn onderling niet goed te vergelijken als gevolg van veranderingen op het gebied van de subsidieregelingen en/of financiële kaders."

### A22.1 — The only green-sector budget subsidy in the entire publication
Tabel 5, "Begrotingssubsidies Ruimtelijk domein" (p.7) — **one line, and it is Trefpunt Groen Eindhoven**:
> "Trefpunt Groen Eindhoven | Netwerkorganisatie voor gemeente Eindhoven en haar inwoners om de lokale groene leefomgeving te bewaken en te versterken | 232.000"
> Totaal Ruimtelijk domein begrotingssubsidies: "232.000"

The only *regeling* under Ruimtelijk domein is "Subsidieregeling sloop brommers en scooters" (p.20), €800 total. There is **no green/nature/voedselbos subsidy scheme anywhere in the publication** (verified by full-text search for "natuur", "milieu", "landschap", "groen", "voedselbos").

### A22.2 — Wasven in the subsidy record (three separate grants, three different schemes)
- Tabel 16, "Subsidieontvangers Basisdagbesteding volwassenen" (p.22):
> "Stichting Groendomein Wasven | Organiseren indicatievrije basisdagbesteding Locatie Wasven | 148.394"
- Tabel 20, "Subsidieontvangers Global Goals" (p.31):
> "Stichting Groendomein Wasven | Programma Samen Waarderen | 24.300"
- Tabel 8, "Subsidieontvangers Evenementen" (p.10):
> "Stichting Groendomein Wasven | Organiseren Evenementen Wasven | 3.900"

Note the recipient legal entity: **Stichting Groendomein Wasven**, not Wasvenzorg, for the dagbesteding subsidy.

### A22.3 — Phood Farm in the subsidy record (two locations, one scheme)
Tabel 16 (pp.22–23):
> "Stichting Phood Farm | Organiseren indicatievrije basisdagbesteding buitenlocatie de Rielse Erven | 22.450"
> "Stichting Phood Farm | Organiseren indicatievrije basisdagbesteding locatie De Caai | 48.990"

### A22.4 — The capped pot both organisations draw on
Tabel 38, "Financieel overzicht subsidieregelingen Sociaal domein" (p.49):
> "Basisdagbesteding volwassenen | Plafond 2025 € 5.272.000 | Subsidie 2025 € 5.272.000 | Restant € 0"

Tabel 16 closes at exactly the same figure: "Totaal 5.272.000" (p.23). So the ceiling was **fully allocated** — residual zero.

Regeling definition (p.21), which shows this is a Wmo instrument:
> "Alle inwoners met een ondersteuningsbehoefte op het gebied van dagbesteding kunnen zo lang dat wenselijk en mogelijk is terecht bij een, voor hen passende, laagdrempelige voorziening in hun eigen omgeving (indicatievrij)."
> "Wmo brede doelgroep"
> "Zowel rechtspersonen als natuurlijke personen kunnen subsidie aanvragen."

Tabel 16 contains **38 location rows** (counted from the full extracted text); the 38 amounts sum to €5,272,003 against the stated total of €5,272,000 — a €3 rounding difference, recorded as found.

Read depth: **full document**; all figures above read from the complete tables, not fragments.

---

## A23 — Phood Farm homepage
- Publisher: Stichting Phood Farm (phoodfarm.org)
- Date: undated (page modified 2025-11-05)
- URL: https://phoodfarm.org/
- Obtained: full page text
- sha256: `cc812b40db848390cbd3e7d3183063d1c5154871147444d259b1a36c6fac409b`
- Access: 200

> "Phood Farm is dé urban farm die de stad inspireert om regeneratief, zorgzaam en community based te produceren en consumeren. Onze innovatieve aquaponic zorgboerderij en Phood Farm Pluktuin zijn inmiddels uitgegroeid tot een hyperlokale farming communities."

Footer identity: "Stichting Phood Farm, Hugo van der Goeslaan 2-01, 5613 LG Eindhoven"; "KVK:81106505 | BTW: NL861933783B01".

Read depth: full. **No funder named on the homepage.**

---

## A24 — Phood Farm, "Over ons"
- URL: https://phoodfarm.org/over-ons/
- Obtained: full page text
- sha256: `a3bf382e9f392463b0e0adb76f33c573a4fd98782ab90ddc7f199acffb516fa4`
- Access: 200

Care-partner claim:
> "Daarbij werken we ook samen met professionele zorg instanties en partners in de zorg. Futuris en Unitio zijn hierin onze care-heroes!"

The stated partner list, verbatim as listed on the page (heading "Partners."):
> "Een goede connectie met onze partners is voor ons als sociale en ecologisch georienteerde stichting van groot belang. Zonder deze mooie connecties, de hulp die we krijgen en de diensten die we afnemen was de uitdaging een stuk groter. Wie zijn die verborgen helden?"
> "Futuris Zorg & Werk / BPD Bouwfonds en Gebiedsontwikkeling / Eindhoven Doet & Alle vrijwilligers / Unitio / Rabobank Foundation / Stichting Doen / Anton Jurgens Fonds"

**Critical read-depth caveat:** the page presents these seven in a single undifferentiated list. It does **not** say who gave money, who lends, who refers participants, who is a landlord, or who is a volunteer broker. Any claim that "Stichting Doen funds Phood Farm" is therefore an inference from list membership, not a documented funder relationship — except for Rabobank Foundation, which is separately documented in A26.

Scale and founding (self-reported, no fte figure given):
> "Het team omvat inmiddels 12 actieve zorgdeelnemers, met in totaal 40 die we al hebben mogen herintegreren, 42 betrokken Community Farmers/-klanten en inspirerende farm-leads."
> "Phood Farm is in 2019 opgericht door Sabine Feron, Tim Elfring, Liza Disselhorst, Robin Meulen en Roy Peeters."

Read depth: full.

---

## A25 — Phood Farm, "Phood Care"
- URL: https://phoodfarm.org/phood-care/
- Obtained: full page text
- sha256: `0649cc75c30b713e231f0a60c8daa469f594642f1e9a5d72dcfbbcde7ca24a62`
- Access: 200

The two care routes, and the municipal one named explicitly:
> "Een daarvan is 'maatwerk dagbesteding', waarin we direct samenwerken met onze partner Futuris Zorg & Werk."
> "Een tweede mogelijkheid is het zogenoemde 'basis dagbesteding', mogelijk gemaakt door de gemeente Eindhoven. Dit is bedoeld om alle inwoners van Eindhoven die daar baat bij hebben, een plek te kunnen bieden waar ze kunnen meewerken, groeien en bloeien. Een verwijzing is niet nodig, alleen een bereidheid om te leren en groeien samen met anderen."

Staffing claim:
> "We hebben een werkbegeleider, psycholoog en Tai Chi Chi Kung coaches in dienst."

Read depth: full.

---

## A26 — Rabobank, "Het groeien van mogelijkheden: De reis van Phood Farm" (Rabo Foundation project page)
- Publisher: Rabobank / Rabo Foundation — **an independent producer** (not Phood Farm)
- Date: 27 June 2024, 11:46
- Direct URL: https://www.rabobank.nl/over-ons/rabofoundation/project/011433263/het-groeien-van-mogelijkheden-de-reis-van-phood-farm — **403 on direct retrieval**
- Recovered via Wayback Machine: http://web.archive.org/web/20260410151645/https://www.rabobank.nl/over-ons/rabofoundation/project/011433263/het-groeien-van-mogelijkheden-de-reis-van-phood-farm
- Obtained: full archived page text (9,102 chars)
- sha256: `9304baffd4c29271ab822966247b1be32c2560051813dbd63c9ae8f7d869e537` (of the Wayback rendering)
- Access: 200 via archive; unsigned request (web.archive.org)

The funding relationship, in Rabobank's own words:
> "Ook al ben je nog zo veerkrachtig en positief, als onderneming heb je uiteindelijk wel geld nodig. Sinds vorig jaar is er samenwerking tussen de Phood Farm en de Rabo Foundation. Ze startte met een gift en hebben nu een sociale lening."

> "Uiteindelijk willen wij op eigen benen staan, maar het is heel fijn dat we deze kans nu hebben." (Phood founder, quoted by Rabobank)

Ambition, attributed to the founders:
> "Zo komt er over anderhalf jaar een permanente Phood locatie op De Caai. Hier kunnen voor ca. 700 huishoudens en horeca bladgroenten verbouwd worden. Tegelijkertijd is daar ruimte om 40 jongeren van werk te voorzien."

Land acquisition mentioned without terms:
> "Een van de laatste stappen in het groeiproces was het verkrijgen van een stuk land. Hier verbouwen ze nu ook producten met behulp van permacultuur"

Founding/expansion narrative:
> "In 2021 kregen ze dan ook de kans om de gehele urban farm over te nemen."

Read depth: full archived page. **No amounts are stated** (neither gift nor loan).

---

## A27 — Phood Farm page sitemap
- URL: https://phoodfarm.org/wp-sitemap.xml → https://phoodfarm.org/sitemap_index.xml (redirect); page sitemap at https://phoodfarm.org/page-sitemap.xml
- sha256: `1f58439c434ada34ac4014c2fc49a53745f014d7065675d60ffb774fe51052a1` (index)
- Access: 200

Used to enumerate pages: `/over-ons/`, `/phood-care/`, `/corporate-sponsoring/`, `/plant-een-boom/`, `/fruitboom/`, `/slaplant/`, `/microgreen/`, `/stage-lopen/`, `/tours/`, `/bedrijven/`, `/producten/`, `/contact/`, `/gender-policy/`, `/aqua-entomo-ponics-voor-circulaire-productie/`.
Relevant negative: **there is no annual report, no ANBI publication and no jaarrekening page in Phood Farm's sitemap.**

---

# Access failures and recovery ladder

## F1 — notubiz: Samenwerkingsprotocol TGE–gemeente (annex 1a)
- URL attempted: https://eindhoven.notubiz.nl/document/16214622/1/8022031_+03+Bijlage+1a+-+Samenwerkingsprotocol+TGE-Gemeente+Ehv?connection_type=16&connection_id=1101320
- Result: **HTTP 403, Cloudflare access challenge**, `cf-ray a60c30ce9c43fff2-AMS`; signed request, keyid `ey9Tj49-ASckC30cTNl43ep9fSSbXbX0ZmKAk9VEdOo`.
- Action: recorded, not bypassed. No attempt to solve, replay, rotate identity or retry-to-pass.
- Mitigation: the governing raadsbrief for the same dossier was retrieved from the parallel system raadsinformatie.eindhoven.nl (A21), which supplied the substance (purpose, koepel role, annual work-plan subsidy). The protocol text itself, its "Werkafspraken", the "Centraal Milieu Overleg" annex and the "Was-wordt-tabel" remain **unobtained**.

## F2 — eindhovendoet.nl
- URL attempted: https://www.eindhovendoet.nl/
- Result: **HTTP 403, Cloudflare challenge**, `cf-ray a60c3177a8fdf2bb-AMS`. This matches the 403 previously recorded for an eindhovendoet.nl vacancy page, so the block appears to be site-wide rather than page-specific.
- Action: recorded; route abandoned per instruction. The volunteer-recruitment side-by-side comparison was therefore **not established**. Eindhoven Doet appears only as a *named partner* in A24 and (indirectly, via a partner-page image filename) on the Wasven site — not as a retrievable listing.

## F3 — rabobank.nl direct
- Result: HTTP 403 on the canonical URL; no cf-ray reported.
- Recovery: Wayback availability API confirmed a 200 snapshot; retrieved A26 from web.archive.org. This is the one place where the archive route carried a pivotal claim (the gift-then-social-loan relationship), and it did so fully.

## F4 — Officiële bekendmakingen search endpoints
- `https://zoek.officielebekendmakingen.nl/resultaten?q=Wasven&sorttype=1&sortorder=4` → **HTTP 400**
- `https://zoek.officielebekendmakingen.nl/resultaten?q=Wasven` → **HTTP 400**
- SRU API `https://zoekservice.overheid.nl/sru/Search?operation=searchRetrieve&version=1.2&maximumRecords=20&query=...` → HTTP 200 but SRU diagnostic: `"Mandatory parameter not supplied"`, details `x-connection`.
- Recovery: document identifiers were located by external search, then each document was retrieved and verified directly by its canonical `.html`/`.pdf` URL (A17, A18, A19). All three verified 200 with full text. The search *interface* was unusable; the documents were not.

## F5 — Wayback CDX API
- `http://web.archive.org/cdx/search/cdx?url=wasven.nl*&...&filter=mimetype:application/pdf` → **HTTP 503**.
- Recovery: not needed. The PDF inventory was obtained more reliably from the site's own media API (A4), which additionally gave publication dates.

## F6 — Wasven "Kwaliteitszorg Jaarverslag"
- The third document named on A1 was never located: it is not in the ANBI media search (A4), not in the page sitemap (A11), and the A1 page's hrefs were stripped. Status: **not obtained, and its URL not established.**

---

# Producers and witness counts (anti-corroboration note)

- **Wasven financial figures**: single producer, the three stichtingen themselves (A5/A6/A7). The 2024 comparative columns are produced by the same author. One witness, three times.
- **Wasven municipal income**: *two* producers — the municipality (A20, A22) and Wasven's own ANBI forms (A5–A7). These do not simply repeat each other; they disagree in classification (see findings §a, "subsidy line anomaly"). That disagreement is itself evidence.
- **Phood Farm funding**: two producers — Phood's own partner list (A24) and Rabobank's own account (A26). Rabobank is a party to the transaction describing its own grant, so it is a confirming but not disinterested witness. Stichting Doen, Anton Jurgens Fonds, BPD and Unitio have **no independent confirmation** in the sources retrieved: for those, the only witness is Phood Farm's list.
- **Trefpunt Groen's municipal subsidy**: two producers — the municipal subsidy publication (A22: €232,000) and the municipal raadsbrief (A21: "Jaarlijks ontvangt TGE subsidie ... op basis van een ingediend werkplan"). Same author (gemeente Eindhoven) in both, so one institutional witness, not two independent ones.
- **Wasven membership of Trefpunt Groen**: single producer — Wasven's own partner page (A12). Not independently confirmed from the TGE side in any retrieved document.
