# Recreation ecology: what is documented, with numbers, for temperate / NW-European urban and peri-urban green space

**Line:** recreation-ecology (one of two independent lines on issue #6). **Retrieved:** 26 November 2026, 22:02–22:11 UTC.
**Question:** what does the peer-reviewed and grey recreation-ecology literature *document* — with numbers, units, denominators, geography and period — about the ecological effects of twelve listed activities in temperate / NW-European urban and peri-urban green space; and where is it qualitative, contested, or silent?

**Marks.** `FT` = full text read; `ABS` = abstract/landing page only; `SNIP` = search snippet only. Every substantive sentence carries a source id (`R1`…`R26`) and a mark. Numbers without a denominator are not reported as thresholds. "Not established in the sources searched" is used as a result, not as a hedge.

**The one-line answer.** The literature documents the *mechanisms* and the *directions* well, and documents *site-specific magnitudes* moderately well for trampling, dog nutrient loading and traffic-noise thresholds. It documents **almost nothing** that converts a visitor number into an ecological effect in a small NW-European urban green space: no retrieved source gives a visitors-per-hectare carrying capacity, none gives a lux threshold for Dutch nocturnal fauna, and none quantifies harvest impact in an urban food forest or community orchard. The quantitative core of this field is (a) montane/alpine and Australasian trampling experiments, (b) one Belgian dog-nutrient census, and (c) Dutch traffic-noise bird work — none of which is a study of urban green space under recreational pressure.

---

## Access log

| Target URL | Status / failure | Class | Recovery attempted | Outcome |
|---|---|---|---|---|
| `https://besjournals.onlinelibrary.wiley.com/doi/10.1002/2688-8319.12128` (De Frenne 2022) | **403, Cloudflare challenge**, `cf-ray a60c3063ed4a44aa-AMS`; signed as `dsh-research-reader.complex-tang.workers.dev` | access-restricted | OpenAIRE API (`api.openaire.eu/search/publications?doi=…`) → returned UGent handle `1854/LU-01GQHW43B4R5VFFDE5GC598A77` and a repository file URL | **Recovered** — publisher PDF deposited by Ghent University Library, read FT (`R9`) |
| `https://onlinelibrary.wiley.com/doi/pdfdirect/10.1111/j.1365-2664.2004.00859.x` (Ticktin 2004) | Not requested — Europe PMC `fullTextUrlList` marked it "Free" via Unpaywall, but the host is the same Cloudflare-fronted Wiley domain that blocked the request above | access-restricted (inferred) | Europe PMC metadata only | **Not retrieved** — metadata only; no number from Ticktin is used anywhere in this file (`R24`) |
| `https://library.wur.nl/WebQuery/wurpubs/fulltext/211959` (Dutch recreation-capacity/"sociale capaciteit" report) | **403**, no challenge header, 199-byte body | access-restricted | Tried `edepot.wur.nl` sibling record search | **Not recovered** — unresolved. This is the most material unresolved item (see §11, §"what would change the answer") |
| `http://leopold.wilderness.net/research/recreation/pdfs/GWS_03_cole.pdf` (Cole, carrying capacity & visitor management) | **404** | missing / moved | Located the work only as a citation inside `R21` | **Not recovered** — cited second-hand only; no claim rests on it |
| `https://research.fs.usda.gov/treesearch/search?search_api_fulltext=…` | **404** | defective (wrong route for the Treesearch search API) | Web search → Treesearch record 66741 → PDF route | **Recovered** (`R20` abstract) |
| `https://lib.ugent.be/en/catalog/pug01:01GQHW43B4R5VFFDE5GC598A77` | **404** (resolver redirect to `resolver.lib.ugent.be`) | moved | `biblio.ugent.be` search → catalogue hit → OpenAIRE for the file URL | **Recovered** (`R9`) |
| Europe PMC query `TITLE:"nutrient fertilization by dogs"` | `hitCount: 0` | coverage (journal not indexed in PubMed/AGR) | Crossref bibliographic search | **Recovered** — DOI `10.1002/2688-8319.12128` confirmed |
| Europe PMC query `AUTH:"Reijnen" AND (traffic OR noise)` | 19 hits, all returned a medical-imaging author of the same name | search-quality, not access | Title search (0 hits) → web search → WUR `edepot` thesis PDF | **Recovered** (`R13`) |
| `https://iplo.nl/…/leidraad_uitvoering_motie_lichthinder_december_2020.pdf` | 200, full text (17,457 chars) | — | — | Retrieved FT; **content finding:** the string "lux" occurs **0 times** in the document (`R17`) |
| `https://edepot.wur.nl/407801` | 200, but document is a 2016 consultancy ecological assessment, not the recreation report the snippet implied | mis-snippet | — | Screened **out**; not used |

No login, paywall, CAPTCHA or Cloudflare challenge was bypassed. One Cloudflare 403 was recorded and routed around via an author-institution repository.

---

## Findings by activity

### 1. Trampling / foot traffic on vegetation and soil

**Documented.** The experimental standard is Cole's design: lanes 0.5 m × 1.5 m, five intensities, a control lane, "a pass was a one-way walk, at a natural gait", tramplers ~70 kg in lug-soled boots, measured 2 weeks and 1 year after (`FT` `R1`). Across **18 vegetation types in five mountain regions of the USA**, "Each type was trampled 0-500 times" (`FT` `R1`). Resistance (relative cover surviving 0–500 passes) ranged **85% to 10%**; resilience (recovery in the following year as a fraction of the loss) ranged **98% to −45%**; tolerance (cover one year after 0–500 passes) **99% to about 38%** (`FT` `R1`). The intensity relationship is non-linear and type-specific: in the *Dryopteris campyloptera* type "just 25 passes reduced relative cover to 33%", whereas in *Carex nigricans* "substantial cover was lost only on the 500-pass lanes" (`FT` `R1`). Resistance and resilience were negatively correlated across species (r = −0.34, P = 0.02) (`FT` `R1`).

The meta-analytic synthesis found the same heterogeneity and then qualified the headline: **304 studies were screened, only nine were randomised controlled experiments, yielding 188 recovery effect sizes**, and recovery "was not strongly dependent on the intensity of the trampling experienced" (`FT` `R2`). The dominant Raunkiaer life-form "accounts for more variation in the resilience of communities to trampling than the intensity of the trampling experienced" (`FT` `R2`).

For NW Europe the evidence thins sharply. A 2-year experimental study in **Central Belgium** forest and heath found "site structure and vegetation were already affected by low intensities of trampling, while vegetation recovery during the first year after trampling was limited in most plant communities"; mesophilous forest herb layers were more sensitive than graminoid/dwarf-shrub heath (`ABS` `R3`). In **three suburban beech forests in NW Switzerland**, repeated trampling (five days at four-week intervals) damaged ground vegetation more than a single event of equal intensity, and "Two years after experimental trampling, most vegetation characteristics still differed from those of undisturbed ground vegetation" (`ABS` `R4`).

**Contested.** Whether more visits means more damage. `R1` shows a monotonic intensity response within a vegetation type; `R2` shows intensity explains less than community composition; `R3` reports effects at "low intensities" without a threshold. There is no retrieved study that reconciles these into a dose–response usable for a site.

**Not established in the sources searched.** No tolerance threshold expressed as passes-per-season for any NW-European *urban* plant community. No long-term (>2 year) NW-European recovery data. No study of trampling on a planted food-forest ground layer.

### 2. Soil compaction

**Documented.** The only retrieved study that applies a controlled recreational pass-count *and* measures penetration resistance is a Mediterranean mountain experiment: transects in Sierra de Guadarrama National Park received differing use intensities, "Soil penetration resistance … was measured only in the 1,000 pass treatments", and the result was "significant alterations when applying a high number of passes on foot or by bicycle, but without significant differences between the two sports" (`FT` `R12`). "One year after the disturbance, in February 2025, penetration resistance decreased in all impacted transects" — partial recovery within one year, with vegetation recovering faster than compaction (`FT` `R12`).

The second link of the chain (bulk density → root growth) is documented only as an agronomic general relationship, by texture: for sandy loam/loam, ideal **<1.40 g/cm³**, root growth affected at **1.63 g/cm³**, restricted at **>1.80 g/cm³**; for silt loam 1.40 / 1.60 / >1.75; for clay (<45% clay) 1.10 / 1.39 / >1.47 (`FT` `R22`).

**Not established in the sources searched — and this is a real gap.** No retrieved source connects a *visitor load* (visitors/ha/day, or passes) to a *bulk density or penetration-resistance value* in a temperate urban green space, and none connects a recreational penetration-resistance value to a measured root-growth or infiltration effect. The frequently quoted "2.5 MPa" and "1.4–1.6 g/cm³" thresholds were **not retrieved to origin** in this session: a targeted search for `"2.5 MPa" AND "penetration resistance" AND "root growth"` returned agronomic (soybean/Oxisol) work, and the OA review retrieved (`PMC12919300`) contains no MPa value in its extracted text. No traffic/visitor-pass threshold for compaction was found.

### 3. Recreational disturbance of breeding birds and other fauna

**Documented — dogs vs no dogs.** The one experimental test retrieved manipulated dog walking at **90 woodland sites** on the urban fringe of Sydney (45 dog-walked, 45 in national parks where dog walking is prohibited), with three treatments (walker + dog on lead, walker alone, control), bird counts on 250 m transects for 10 min, sites ≥150 m from forest edge and ≥1 km apart (`FT` `R6`). Result: "dog walking in woodland leads to a **35% reduction in bird diversity and 41% reduction in abundance**, both in areas where dog walking is common and where dogs are prohibited" (`FT` `R6`). Exposure at frequented sites was "on average 10 dog walkers and 12 walkers per hour in the morning (07.30–09.30 hours)" and "Only two walkers in total were seen during all surveys of unfrequented sites" (`FT` `R6`).

**Documented — flight-initiation distance.** FID work is extensive and standardised but the retrieved study reports model structure rather than metre values: "4420 flight initiation distance observations across 68 species" in Prague, with the finding that a species' urban history, not its present-day urban abundance, predicts fear response (`FT` `R23`). **No absolute FID or buffer distance in metres was extracted** from `R23`; the metre-scale distances this line could document are noise-based, not FID-based (see §9).

**Documented — breeding success vs displacement.** A nest-survival field study, April–August 2023, in multiple green spaces in **Montreal**, on four common open-cup nesters, found "no significant influence of human activity, vegetation concealment, and seasonality on nest survival for our target species" (`FT` `R7`). This is the strongest retrieved counter-evidence to the displacement→breeding-failure inference.

**Documented — edge effects on fauna.** Across 22 landscapes, 1,673 vertebrate species: "85% of species' abundances are affected, either positively or negatively, by forest edges", and forest-core species "only reached peak abundances at sites farther than 200-400 m from sharp high-contrast forest edges" (`FT` `R19`).

**Contested.** Whether documented displacement translates into population loss. `R6` measures assemblage-level reduction at the moment of disturbance; `R7` finds no nest-survival cost in a different system; `R19` shows that edge-adapted communities are genuinely different, not merely displaced.

**Not established in the sources searched.** No NW-European study of dog-walking effects on birds in urban green space. No disturbance-distance table for pedestrians (as opposed to vehicles) in a Dutch or Belgian urban park. Whether habituated urban populations differ in *fitness* (as opposed to FID) is not established by any retrieved source.

### 4. Seasonal timing

**Documented, but only piecemeal.** Trampling experiments are applied "in early summer, after vegetative cover approached its annual peak" (`FT` `R1`) — i.e., the design deliberately standardises season rather than testing it. Swiss beech trampling compared single-day and repeated (five days at four-week intervals) events and found temporal distribution mattered (`ABS` `R4`). The Mediterranean pass experiment states that "Mediterranean seasonality strongly modulates impacts" and that recovery was measured into February 2025 (`FT` `R12`). Bird work is framed by the breeding season (`FT` `R7`, `FT` `R13`). Nitrogen from dog urine deposited in autumn "will not be taken up by the vegetation … but is prone to leaching and volatilization" (`FT` `R9`).

**Not established in the sources searched.** No retrieved source gives a documented, quantified "sensitive window" (dates or months) for recreation in NW-European urban green space, and no source gives a seasonal *effect size* (e.g. damage per 100 passes in April vs September). The Dutch legal *broedseizoen* is a regulatory convention; this line did not retrieve an ecological study quantifying it, and does not assert one. **Treat "the breeding season is the sensitive window" as expert/legal guidance, not as a measured finding, on the evidence retrieved here.**

### 5. Dogs: nutrient enrichment, disturbance, disease

**Documented — nutrient loading (the strongest quantified finding in this file).** In four peri-urban forests and nature reserves in **Belgium**, 487 direct-count censuses over 1.5 years counted 1,629 dogs; mean density "1.3 dogs ha⁻¹ day⁻¹ off leash and … 2.9 dogs ha⁻¹ day⁻¹ on leash" (`FT` `R9`). Net fertilisation: "canine N and P fertilization rates on average amount to **11 kg N** … and **5 kg P** per hectare per year" (abstract), with the results section giving "**11.5 kg N ha⁻¹ year⁻¹ across all sites, with a peak of 31.3 kg N ha⁻¹ year⁻¹** in the study site with the highest dog densities" (`FT` `R9`; the abstract rounds to 11, the results give 11.5 — reported here as both, not reconciled). "Only 3% of the total P deposited by dogs is via their urine" (`FT` `R9`).

The comparison that makes these numbers usable: atmospheric N deposition is "5–25 kg N ha⁻¹ year⁻¹ across most of Europe", and was "7 kg N ha⁻¹ year⁻¹ in 2019 in the study area (Flemish Environmental Agency, 2020)"; the critical deposition load for the studied vegetation types "is 20 kg N ha⁻¹ year⁻¹ … between 20 and 34 kg N ha⁻¹ year⁻¹" for the fourth site; and mowing-with-hay-removal P export is "2–20 kg P ha⁻¹ year⁻¹" (`FT` `R9`). Dog deposition is therefore of the same order as, or a large fraction of, both background deposition and management export — in the sites with the highest dog density, above the critical load on its own.

**Documented — disease/parasite transfer.** A Dutch survey of *Toxocara* spp. eggs in public parks and children's sandboxes in **Utrecht** found park contamination with *T. canis* "comparable with reports from other European cities", and — the load-bearing null — "**no difference between parks with or without formal exclusion of dogs**" (`ABS` `R10`).

**Documented — disturbance.** See §3 (`FT` `R6`).

**Not established in the sources searched.** Whether dog effects are *additive* to human trampling. No retrieved study separates the dog's paw load, urine/faeces chemistry and predation-cue effect from the accompanying human's trampling. `R9` estimates nutrient input per hectare but not its vegetation response; `R6` measures bird response but not nutrients. **The additivity question asked by issue #6 is, on this evidence, unstudied.**

### 6. Foraging / harvesting of wild and planted food

**Documented — almost nothing for the relevant setting.** The canonical review of harvest ecology (Ticktin 2004, *J Appl Ecol* 41:11–21) was **identified but not retrieved** (Wiley/Cloudflare; see access log) and is used here only as a pointer (`R24`). What was retrieved nearby is tropical NTFP demography, retained only as a demonstration that the *shape* of the question is answerable elsewhere: in the Brazilian savanna, harvest under traditional management "had no impact on golden-grass population dynamics", whereas earlier harvest "leads to population decline due to plant uprooting", measured by matrix models over 3 years at 9 sites (`ABS` `R25`); and in Benin, bark and foliage harvest "significantly reduced" stochastic population growth rates of *Khaya senegalensis*, but "ecological differences between regions had a greater effect on population growth rates than did harvest" (`ABS` `R26`). Neither is NW European and neither is used for any number in the thresholds table.

**Not established in the sources searched — and this is a genuine absence, not a search failure.** No retrieved study quantifies the effect of foraging or harvesting on plant populations in NW-European urban green space. None quantifies harvest impact in a food forest, community orchard or allotment. None gives a sustainable off-take rate for any species a Dutch food forest would plant. **The evidence base for "harvesting here is or is not compatible with conservation here" is, on this search, empty.** The honest formulation for the risk matrix: harvesting pressure in a small Dutch food forest is an *unquantified* risk, and the nearest evidence (tropical NTFP demography) is not transferable in either direction.

### 7. Events and "activation"

**Documented — one quantified case.** A three-day beach music festival in **Portugal, July 2022**, assessed by drone orthophoto and NDVI: "**18,500 m² of embryonic dune vegetation, which represented 35% of the existing plant community, was removed** by works on the beach and by trampling of festival attendees", with the site "a construction site over about twenty days" (`ABS` `R11`). Geomorphology recovered — "beach configuration was approximately restored to the pre-festival configuration after the event" — while vegetation did not, within the observation window (`ABS` `R11`).

**Documented — the mechanism that makes events different from steady use.** Repeated trampling events at four-week intervals did more damage than a single event of the same total intensity, and effects persisted at two years (`ABS` `R4`). Recovery time for vegetation cover after a high-pass event was under a year in a Mediterranean system, while penetration resistance was still recovering at one year (`FT` `R12`).

**Not established in the sources searched.** No retrieved study of a music festival, market or event in a **park or urban green space** in NW Europe. No post-event recovery curve in days/weeks for grass swards under compaction from staging, crowds or vehicles. No noise measurement for events in green space (see §9 — the dB literature is traffic-based). The 35%/18,500 m² figure is a single study in a dune system and should not be transferred to a lawn or woodland.

### 8. Artificial light at night

**Documented — thresholds exist, but are taxon- and species-specific, and lux is a poor metric.** Insect work: "Early light exposure experiments conducted in the laboratory demonstrated that sufficiently bright light (from **50 to 1,000 lux**) completely inhibits bioluminescent signaling in several firefly species"; field studies report effects at much lower levels, with 0.05 lux described as "similar to that produced by a quarter moon", and experimental plots lit at ~167–301 lux at centre (`FT` `R15`). The review is explicit that the unit is the problem: "Although lux is widely used by engineers and policymakers, and is easiest to measure, it poorly approximates brightness as it is perceived by non-human animals" (`FT` `R15`).

Bats: response "is highly species-specific: some species tolerate urban habitat or are even favoured by its roosting or foraging opportunities, others are affected" (`FT` `R16`). No lux threshold for bats was extracted from `R16`.

**Dutch guidance.** The national guidance document on light nuisance (`R17`) frames light as a balancing of interests: "Overheden maken, afhankelijk van de locatie en gewenste activiteiten, een belangenafweging bij het toestaan van kunstlicht" — and the **word "lux" does not appear in the document at all** (`FT` `R17`). So the Dutch national instrument is procedural, not numerical.

**Not established in the sources searched.** No NW-European lux threshold for insects, bats, birds or plants. No spectral guidance value retrieved. Any "X lux is too much" statement for a Dutch park would, on this evidence, be invented.

### 9. Noise

**Documented — the best-quantified dose–response in this file, but for traffic, not recreation.** Reijnen's Dutch thesis modelled breeding-bird density against traffic noise load (24-h L<sub>eq</sub> in dB(A)) across transects, estimating a threshold below which density does not decline (`FT` `R13`). Species thresholds (dB(A), with 90% CI where computable): mute swan 36 (NS), mallard 53 (NS), shoveler 51*, coot 60*, oystercatcher ≈27 (?–43)**, lapwing **47 (42–51)***, black-tailed godwit **43 (37–48)***, redshank 52 (NS), skylark **48 (46–56)***; all species combined **47 dB(A)** (`FT` `R13`). Transect noise loads ranged "from 59 ± 6 dB(A) in the strips adjacent to the road to 38 ± 5 dB(A) in the most remote strips" (`FT` `R13`).

Disturbance distances were then derived by converting thresholds to distance: "the estimated disturbance distance varied from **20 to 1,700 m at 5,000 cars a day** and from **75 to 3,530 m at 50,000 cars a day**"; "For the density of all species combined the disturbance distance was **120 and 560 m**" (`FT` `R13`). Context: "about 10% of the area has a traffic noise load of more than 50 dB(A) and about 30% of more than 40 dB(A)" in the north and west of the Netherlands (`FT` `R13`).

**Documented — the mechanism, and a perverse result.** Noise alone reduces nesting species richness and changes community composition, but "noise indirectly facilitates reproductive success of individuals nesting in noisy areas as a result of the disruption of predator–prey interactions" (`ABS` `R8`). Any assumption that noise monotonically harms breeding is therefore wrong in at least one well-cited system.

**Documented — the state of the evidence.** A systematic map update counted 1,794 articles from the 2020 map, "of which 466 were retained after re-screening the full texts", plus an update search yielding 13,698 records (`FT` `R14`).

**Not established in the sources searched.** No dB(A) threshold for *recreational* noise (people, dogs, music) in green space. The transfer from traffic noise (continuous, linear source, 24-h L<sub>eq</sub>) to intermittent event noise is not documented in anything retrieved, and should be flagged as an inference, not a finding.

### 10. Path creation / desire lines / informal trails

**Documented.** In Aconcagua Park (Andes), "Within the **237 ha** area surveyed in the Horcones Valley, over **19 km of trails** were found, nearly all of which (**94%**) were informal"; the network "resulted in the direct loss of **11.5 ha of vegetation** and extensive fragmentation of alpine meadows (21 fragments) and steppe vegetation (68 fragments)"; "**81% of 102 randomly located plots** showed evidence of disturbance, with the severity of disturbance greatest close to trails"; and "vegetation in **90% of the Valley** has been damaged by visitor use" (`ABS` `R5`).

**Documented — edge effects, which are the mechanism by which a small patch loses interior habitat.** "nearly 20% of the world's remaining forest now found within 100 m of an edge, 50% within 500 m and 70% within 1 km"; "11%, 30%, 41% and 57% of bird, reptile, amphibian and mammal species, respectively, showed strong declines towards forest edges" (`FT` `R19`).

**Contested / caution.** `R5` is an alpine, high-altitude, pack-animal system with no formal trail density comparable to a Dutch park; the transferable finding is the *shape* of the relationship (small numbers of informal lines do most of the areal damage; severity decays with distance from the line), not the magnitudes.

**Not established in the sources searched.** No retrieved study quantifies informal-trail density (km/ha) or trail widening for a Dutch or Belgian urban park, and none relates trail density to interior-habitat loss in patches of park size (<50 ha).

### 11. Carrying capacity / visitor-density thresholds

**Documented — the frameworks exist and are explicitly normative.** The Limits of Acceptable Change system is "A wilderness management-by-objectives planning system … Through identification of standards, acceptable wilderness conditions are defined and appropriate management actions formulated" (`ABS` `R20`) — i.e. LAC defines *standards chosen by people*, not ecological limits discovered by measurement.

**Documented — the critique, in the literature's own words.** "It is in fact very difficult to establish a mechanical relationship between the level of frequentation and the degree of impacts"; and "The actors who most cling to the CC concept are managers and policy-makers who interpret it in normative terms. But even this normative use is a fallacy" (`FT` `R21`). The same critique notes that "decision making processes often define CC by considering site-specific objectives and related activities, which is indeed tautological and permits the legitimization of one sided interests" (`FT` `R21`). This is consistent with `R2`'s empirical finding that trampling intensity explains less than community composition.

**Not established in the sources searched — the expected null, confirmed.** **No retrieved source gives a visitor-density carrying capacity with units (visitors ha⁻¹ yr⁻¹, or simultaneous visitors per hectare) for any temperate urban green space.** What exists instead are three surrogates, each with a different unit and none a capacity: dB(A) thresholds and derived metre distances for breeding birds (`R13`); dogs ha⁻¹ day⁻¹ with a derived kg N ha⁻¹ yr⁻¹ (`R9`); and pass-counts in trampling experiments (`R1`, `R12`). The honest statement for the risk matrix is that **there is no ecological number to import; a site limit must be constructed, and the literature says so explicitly rather than supplying one.**

### 12. Small urban habitat patches

**Documented — the counter-intuitive finding.** A global synthesis "based on 31 systematic conservation planning studies across four continents" concluded "that small, isolated patches are inordinately important for biodiversity conservation" and argued against "simplistic application of island biogeography theory" (`FT` `R18`). This directly contradicts the premise that a small patch is simply worth less.

**Documented — but interior habitat is genuinely scarce in small patches.** Forest-core species reach peak abundance only beyond 200–400 m from a sharp edge (`FT` `R19`), which implies that a patch narrower than ~400–800 m has no true core — a geometric consequence, not a visitor effect. Edge-to-area ratio therefore predicts *which species a patch can hold at all*, before any visitor arrives.

**Not established in the sources searched.** **No retrieved study tests whether a small patch degrades faster under the same visitor load** — that is, whether the per-visitor effect is patch-size-dependent. The interaction between edge effects and recreational pressure in patches of Dutch park size is, on this search, unstudied. The risk matrix should treat "small patches lose value faster per visit" as a plausible mechanism with **no direct evidence either way**, and should not cite edge-effect literature as if it were evidence for it.

---

## Thresholds table

Every value below is a *documented* number. "Confidence" states what kind of number it is, not how much I trust the authors.

| Threshold / value | Value + unit | What it applies to | Id | Design | Geography | Confidence |
|---|---|---|---|---|---|---|
| Cover loss at low intensity | 25 passes → relative cover 33% | *Dryopteris campyloptera* ground layer | `R1` | field experiment, 4 replicates, 0–500 passes | North Carolina, USA | measured |
| Cover loss threshold | substantial loss only at 500 passes | *Carex nigricans* ground layer | `R1` | field experiment | Washington, USA (subalpine) | measured |
| Resistance index range | 85% to 10% relative cover | 18 vegetation types, 0–500 passes | `R1` | field experiment | 5 US mountain regions | measured |
| Resilience index range | 98% to −45% | recovery in year 1 as % of loss | `R1` | field experiment | USA | measured |
| Tolerance index range | 99% to ≈38% | relative cover 1 yr after 0–500 passes | `R1` | field experiment | USA | measured |
| Intensity is not the main predictor | 9 RCTs, 188 effect sizes from 304 studies | trampling recovery, all vegetation | `R2` | systematic review + meta-analysis | global | measured (meta-analytic) |
| Compaction at high pass counts | significant at 1,000 passes; not quantified below | trail running / MTB transects | `R12` | field experiment, 1-yr recovery | Sierra de Guadarrama, Spain | measured |
| Bulk density — affects root growth | 1.63 g/cm³ (sandy loam/loam); 1.60 (silt loam); 1.49 (sandy clay); 1.39 (clay) | root growth | `R22` | general relationship table | USA (NRCS) | expert-guidance / rule-of-thumb |
| Bulk density — restricts root growth | >1.80 g/cm³ (loam); >1.75 (silt loam); >1.65 (silty clay loam); >1.47 (clay) | root growth | `R22` | general relationship table | USA (NRCS) | expert-guidance / rule-of-thumb |
| Dog nutrient load — N | 11 kg N ha⁻¹ yr⁻¹ (abstract); 11.5 mean, peak 31.3 | peri-urban forest / reserve | `R9` | 487 censuses/1.5 yr + literature parameterisation | Belgium (4 sites) | modelled from measured counts |
| Dog nutrient load — P | 5 kg P ha⁻¹ yr⁻¹ (abstract); peak ≈13 | as above; 3% via urine | `R9` | as above | Belgium | modelled from measured counts |
| Dog density | 1.3 off-leash + 2.9 on-leash dogs ha⁻¹ day⁻¹ | recreational dog use | `R9` | direct counts (1,629 dogs) | Belgium | measured |
| Critical N deposition load | 20 kg N ha⁻¹ yr⁻¹ (3 sites); 20–34 (4th site) | habitat quality threshold | `R9` | cited concept applied to sites | Belgium | expert-guidance |
| Background N deposition | 5–25 kg N ha⁻¹ yr⁻¹ (Europe); 7 (site, 2019) | comparison baseline | `R9` | EMEP data + Flemish agency | Belgium / Europe | measured (monitoring) |
| P export by hay removal | 2–20 kg P ha⁻¹ yr⁻¹ | comparison to dog P | `R9` | literature values | NW Europe | measured (literature) |
| Bird diversity / abundance loss with dogs | −35% diversity, −41% abundance | woodland bird assemblage | `R6` | manipulative field experiment, 90 sites | Sydney, Australia | measured |
| Disturbance threshold — all birds | 47 dB(A) (24-h L<sub>eq</sub>) | breeding bird density, grassland | `R13` | observational regression, threshold model | Netherlands | measured/modelled |
| Disturbance threshold — black-tailed godwit | 43 dB(A) (37–48) | breeding density | `R13` | as above | Netherlands | measured/modelled |
| Disturbance threshold — lapwing | 47 dB(A) (42–51) | breeding density | `R13` | as above | Netherlands | measured/modelled |
| Disturbance threshold — skylark | 48 dB(A) (46–56) | breeding density | `R13` | as above | Netherlands | measured/modelled |
| Disturbance distance — all species | 120 m (5,000 cars/day); 560 m (50,000 cars/day) | derived from dB(A) threshold | `R13` | model conversion | Netherlands | modelled |
| Disturbance distance — species range | 20–1,700 m (5,000 cars/day); 75–3,530 m (50,000 cars/day) | 12 grassland bird species | `R13` | model conversion | Netherlands | modelled |
| FID dataset scale | 4,420 observations, 68 species | avian fear response | `R23` | standardised field protocol + Bayesian phylogenetic mixed models | Prague, Czechia | measured |
| ALAN — firefly signalling inhibited | 50–1,000 lux (laboratory) | bioluminescent courtship | `R15` | lab experiments, review | multi | measured (lab) |
| ALAN — reference level | 0.05 lux ≈ quarter moon | ambient night-sky baseline | `R15` | review | multi | measured (reference) |
| Edge effect — core-species peak | >200–400 m from sharp high-contrast edge | forest-core vertebrates | `R19` | global synthesis, 1,673 species | 22 landscapes, 7 realms | modelled |
| Edge effect — species affected | 85% of 1,673 species (46% +, 39% −) | vertebrate abundance | `R19` | global synthesis | global | measured |
| Small-patch conservation value | 31 studies, 4 continents | patch size vs conservation value | `R18` | global synthesis | global | modelled |
| Informal trail network | 19 km trails, 94% informal, 11.5 ha vegetation lost, 81% of 102 plots disturbed, 90% of valley | alpine vegetation | `R5` | field survey + rapid visual assessment | Aconcagua, Argentina | measured |
| Festival vegetation loss | 18,500 m² = 35% of plant community | embryonic dune vegetation | `R11` | drone NDVI before/after | Portugal | measured |
| Dog-exclusion efficacy (parasite) | no difference between parks with/without exclusion | *Toxocara* egg contamination | `R10` | field survey | Utrecht, NL | measured (null) |
| LAC framework | no numerical standard; standards are chosen | wilderness/visitor management | `R20` | planning system | USA | expert-guidance |
| Carrying capacity as construct | no mechanical use–impact relationship | recreation management | `R21` | conceptual critique | international | expert-guidance |

---

## Counter-evidence and null results

1. **Intensity matters less than community composition.** The only retrieved meta-analysis found recovery "was not strongly dependent on the intensity of the trampling experienced" and that Raunkiaer life-form explained more variance (`FT` `R2`). Any linear "more visitors → proportionally more damage" model is contradicted.
2. **No nest-survival cost of human activity.** Four open-cup nesters, April–August 2023, Montreal: "no significant influence of human activity, vegetation concealment, and seasonality on nest survival" (`FT` `R7`). Displacement ≠ breeding failure, at least here.
3. **Noise can raise breeding success.** "noise indirectly facilitates reproductive success of individuals nesting in noisy areas as a result of the disruption of predator–prey interactions" (`ABS` `R8`).
4. **Dog exclusion did not reduce parasite contamination.** "no difference between parks with or without formal exclusion of dogs" (`ABS` `R10`) — direct counter-evidence to a dog-ban reflex, on one outcome (soil *Toxocara* eggs), in one city, in 1993.
5. **Small patches are disproportionately valuable, not disproportionately worthless.** ("small, isolated patches are inordinately important for biodiversity conservation", `FT` `R18`). The premise that a small patch is ecologically second-rate is contradicted.
6. **Trampling effects occur where dogs are banned and where they are allowed.** In `R6` the 35%/41% reduction held "both in areas where dog walking is common and where dogs are prohibited" — which cuts both ways: it weakens "dogs are the problem" and strengthens "human presence is the problem".
7. **Carrying capacity is a policy construct.** Stated by its own literature: the use–impact relationship is not mechanical and normative use is "a fallacy" (`FT` `R21`); LAC defines standards rather than discovering them (`ABS` `R20`).
8. **Effects can be smaller than design/management effects.** The nearest retrieved evidence: `R9` shows dog N input (11.5 kg N ha⁻¹ yr⁻¹) is of similar magnitude to mowing P export (2–20 kg P ha⁻¹ yr⁻¹) and to background deposition (5–25 kg N ha⁻¹ yr⁻¹), i.e. management and background fluxes are not trivially smaller than visitor-derived ones. No retrieved study directly compares visitor effect sizes against mowing/drainage effects on the same response variable — **that comparison is a gap, and any claim that "visitors matter less than mowing" is not established here.**

---

## Sources

**R1** — Cole, D.N. (1995). Experimental trampling of vegetation. II. Predictors of resistance and resilience. *Journal of Applied Ecology* 32(1): 215–224. PDF via USDA Forest Service Treesearch 23582: https://research.fs.usda.gov/download/treesearch/23582.pdf. **FT.** Retrieved 2026-11-26.
> "Eighteen experimental study sites were established in five different mountainous regions of the United States." · "Each type was trampled 0-500 times and vegetation response was assessed 2 weeks and 1 year after trampling." · "A pass was a one-way walk, at a natural gait, along the lane. The weight of tramplers was about 70kg and tramplers wore lug-soled boots with incised treads." · "Resistance indices varied from 85% in the Carex nigricans type to 10% in the Dryopteris campyloptera type." · "In the Dryopteris campyloptera type, just 25 passes reduced relative cover to 33%." · "Resilience indices varied from 98% (virtually complete recovery on all lanes) in Trifolium parryi to -45% in Pachistima myrsinites." · "Tolerance indices varied from 99% in Trifolium parryi to about 38% in the two Vaccinium scoparium types." · "Trampling treatments were administered in early summer, after vegetative cover approached its annual peak."

**R2** — Pescott, O.L. & Stewart, G.B. (2014). Assessing the impact of human trampling on vegetation: a systematic review and meta-analysis of experimental evidence. *PeerJ* 2: e360. https://doi.org/10.7717/peerj.360. **FT** (PMC4017817). Retrieved 2026-11-26.
> "The systematic search yielded 304 studies; of these, nine reported relevant randomized controlled experiments, providing 188 vegetation recovery effect sizes for analysis." · "This was related to resistance and recovery time, and the interactions of these variables with Raunkiaer life-form, but was not strongly dependent on the intensity of the trampling experienced." · "the dominant Raunkiaer life-form of a plant community accounts for more variation in the resilience of communities to trampling than the intensity of the trampling experienced"

**R3** — Roovers, P., Verheyen, K., Hermy, M. & Gulinck, H. (2004). Experimental trampling and vegetation recovery in some forest and heathland communities. *Applied Vegetation Science* 7(1). https://doi.org/10.1111/j.1654-109X.2004.tb00601.x. **ABS** (Europe PMC AGRIS record; abstract only). Retrieved 2026-11-26.
> "In this study, short-term effects – a 2-yr period – of human trampling on some common forest and heath communities in Central Belgium were studied experimentally." · "The analysis showed that site structure and vegetation were already affected by low intensities of trampling, while vegetation recovery during the first year after trampling was limited in most plant communities."

**R4** — Rusterholz, H.-P., Weisskopf-Kissling, M. & Baur, B. (2021). Single versus repeated human trampling events: Responses of ground vegetation in suburban beech forests. *Applied Vegetation Science* 24(3). https://doi.org/10.1111/avsc.12604. **ABS** (Europe PMC AGRIS abstract; Wiley full text not pursued — see access log). Retrieved 2026-11-26.
> "Experimental trampling of different intensity was conducted on a single day (single trampling) or on five days at intervals of four weeks (repeated trampling) in three suburban beech forests on different soil types." · "Most vegetation characteristics were more severely affected by repeated trampling than single trampling of equal intensity." · "Two years after experimental trampling, most vegetation characteristics still differed from those of undisturbed ground vegetation."

**R5** — Barros, A. & Pickering, C.M. (2017). How Networks of Informal Trails Cause Landscape Level Damage to Vegetation. *Environmental Management*. https://doi.org/10.1007/s00267-017-0865-9. **ABS.** Retrieved 2026-11-26.
> "Within the 237 ha area surveyed in the Horcones Valley, over 19 km of trails were found, nearly all of which (94%) were informal." · "This network of trails resulted in the direct loss of 11.5 ha of vegetation and extensive fragmentation of alpine meadows (21 fragments) and steppe vegetation (68 fragments)." · "81% of 102 randomly located plots showed evidence of disturbance, with the severity of disturbance greatest close to trails." · "vegetation in 90% of the Valley has been damaged by visitor use"

**R6** — Banks, P.B. & Bryant, J.V. (2007). Four-legged friend or foe? Dog walking displaces native birds from natural areas. *Biology Letters* 3(6): 611–613. https://doi.org/10.1098/rsbl.2007.0374. **FT** (PMC2391219). Retrieved 2026-11-26.
> "Here we show that dog walking in woodland leads to a 35% reduction in bird diversity and 41% reduction in abundance, both in areas where dog walking is common and where dogs are prohibited." · "In this study we experimentally manipulated dog walking at 90 sites in woodland on the urban fringe of Sydney, Australia" · "counted birds seen and heard along 250 m transects for 10 min after treatments were applied" · "Dog-walking activity at frequented sites was on average 10 dog walkers and 12 walkers per hour in the morning (07.30–09.30 hours) and 6 dog walkers and 7 walkers in the afternoon (14.30–16.30 hours)." · "Only two walkers in total were seen during all surveys of unfrequented sites and no dog walking was observed."

**R7** — Cull, C.A., Guest, M.J., Frei, B. & Ziter, C.D. (2025). Human recreational activity does not influence open cup avian nest survival in urban green spaces. *Urban Ecosystems* 28(2): 24. https://doi.org/10.1007/s11252-024-01669-0. **FT** (PMC11782460). Retrieved 2026-11-26.
> "We conducted a nest survival field study between April and August of 2023 in multiple green spaces in Montreal, Quebec, Canada" · "Our analyses surprisingly revealed no significant influence of human activity, vegetation concealment, and seasonality on nest survival for our target species."

**R8** — Francis, C.D., Ortega, C.P. & Cruz, A. (2009). Noise pollution changes avian communities and species interactions. *Current Biology* 19(16): 1415–1419. https://doi.org/10.1016/j.cub.2009.06.052. **ABS.** Retrieved 2026-11-26.
> "We show that noise alone reduces nesting species richness and leads to different avian communities." · "Contrary to expectations, noise indirectly facilitates reproductive success of individuals nesting in noisy areas as a result of the disruption of predator-prey interactions."

**R9** — De Frenne, P., Cougnon, M., Janssens, G.P.J. & Vangansbeke, P. (2022). Nutrient fertilization by dogs in peri-urban ecosystems. *Ecological Solutions and Evidence* 3(1): e12128. https://doi.org/10.1002/2688-8319.12128. **FT** — publisher copy deposited at Ghent University: https://biblio.ugent.be/publication/01GQHW43B4R5VFFDE5GC598A77/file/01GQHW4V8W1YQ9ASTEV1FN8S2T (Wiley landing page blocked, 403 Cloudflare, `cf-ray a60c3063ed4a44aa-AMS`). Retrieved 2026-11-26.
> "We used 487 direct-count censuses over 1.5 years to collect accurate dog abundance data per hectare per year in four sites in peri-urban forests and nature reserves in Belgium." · "We find that canine N and P fertilization rates on average amount to 11 kg N (more or less equally from urine and faeces) and 5 kg P (predominantly from faeces) per hectare per year, respectively." · "Across the four study sites and 487 count events, we counted 1629 dogs. We calculate a mean dog density of 1.3 dogs ha−1 day−1 off leash and a mean of 2.9 dogs ha−1 day−1 on leash" · "11.5 kg N ha−1 year−1 across all sites, with a peak of 31.3 kg N ha−1 year−1 in the study site with the highest dog densities" [extraction note: the two-column PDF interleaves a figure label into this sentence, so only the clean clause is quoted] · "Only 3% of the total P deposited by dogs is via their urine." · "this critical deposition load is 20 kg N ha−1 year−1, whereas it ranges for study site 4 between 20 and 34 kg N ha−1 year−1" · "5–25 kg N ha−1 year−1 across most of Europe; based on EMEP data in Staude et al., 2020" · "7 kg N ha−1 year−1 in 2019 in the study area (Flemish Environmental Agency, 2020)" · "removal rates are 2–20 kg P ha−1 year−1 under mowing with hay removal (Schelfhout et al."

**R10** — Jansen, J., van Knapen, F., Schreurs, M. & van Wijngaarden, T. (1993). [Toxocara ova in parks and sand-boxes in the city of Utrecht]. *Tijdschrift voor Diergeneeskunde* 118(19): 611–614. PMID 8211920. **ABS.** Retrieved 2026-11-26.
> "The pollution of parks with the eggs of the dog's ascarid Toxocara canis is comparable with reports from other European cities." · "Interestingly there was no difference between parks with or without formal exclusion of dogs."

**R11** — Andriolo, U. & Gonçalves, G. (2023). Impacts of a massive beach music festival on a coastal ecosystem — A showcase in Portugal. *Science of the Total Environment* 858: 160733. https://doi.org/10.1016/j.scitotenv.2022.160733. **ABS.** Retrieved 2026-11-26.
> "the comparison of Normalized Difference Vegetation Index (NDVI) maps revealed that 18,500 m2 of embryonic dune vegetation, which represented 35 % of the existing plant community, was removed by works on the beach and by trampling of festival attendees." · "a massive beach music festival held on a Portuguese beach-dune system over three days in July 2022" · "Digital Surface Model (DSM) analysis showed that beach configuration was approximately restored to the pre-festival configuration after the event."

**R12** — Gómez-Prieto, F., Tejedo, P., Faucha, M., Escudero, A., Leung, Y.F., Valladares, F. & Benayas, J. (2026). Impacts of trail running and mountain biking: Resilience of a Mediterranean mountain ecosystem. *iScience* 29(10): 117721. https://doi.org/10.1016/j.isci.2026.117721. **FT** (PMC13661210). Retrieved 2026-11-26.
> "Results show that soil compaction and vegetation cover are the most affected among the variables analyzed, with significant alterations when applying a high number of passes on foot or by bicycle, but without significant differences between the two sports." · "One year after the disturbance, in February 2025, penetration resistance decreased in all impacted transects." · "Soil penetration resistance, a commonly used indicator of compaction, was measured only in the 1,000 pass treatments in the flat area and on the sloped areas" · "Mediterranean seasonality strongly modulates impacts."

**R13** — Reijnen, M.J.S.M. (1995). *Disturbance by car traffic as a threat to breeding birds in the Netherlands.* PhD thesis, Rijksuniversiteit Leiden / IBN-DLO. https://edepot.wur.nl/390629. **FT.** Retrieved 2026-11-26.
> "The noise load in the transects from road traffic, varied from 59 + 6 dB(A) in the strips adjacent to the road to 38 + 5 dB(A) in the most remote strips." · "Since the threshold value for the density of all species combined is 47 dB(A) and for the black-tailed godwit, the most characteristic species, 42 dB(A)(Table 1), significant population reductions can be expected." · "With respect to species the estimated disturbance distance varied from 20 to 1700 m at 5000 cars a day and from 75 to 3530 m at 50 000 cars a day (Table 2). For the density of all species combined the disturbance distance was 120 and 560 m, respectively (Table 2)." · "about 10% of the area has a traffic noise load of more than 50dB(A) and about 30% of more than 40dB(A)(Anon. 1988)." · Table 1 (T(CFL) column, dB(A), 90% CI in parentheses): "Lapwing … 47(42-51)"; "Black-tailed godwit … 43(37-48)"; "Skylark … 48(46-56)"; "Mute swan … 36"; "Mallard … 53(27-61)"; "Shoveler … 51(42-59)"; "Coot … 60(41-63)"; "Tufted duck … 61"; "Redshank … 52"; "Oystercatcher … 27(?-43)" (leading character OCR-ambiguous in the retrieved PDF). *Note: 42 dB(A) in the prose vs 43 dB(A) in Table 1 for black-tailed godwit — the two are reported as they appear, not reconciled.*

**R14** — Terray, L., Petiteau, B., Dutilleux, G., Vanpeene, S., Amiard, P., Sordello, R. & Reyjol, Y. (2025). What is the evidence for the impacts of airborne anthropogenic noise on wildlife? A systematic map update. *Environmental Evidence* 14: 14. https://doi.org/10.1186/s13750-025-00368-3. **FT** (PMC12297495). Retrieved 2026-11-26.
> "Sordello et al. (2020) provided 1,794 articles, of which 466 were retained after re-screening the full texts. The search update yielded 13,698 ci[rded records]" (sentence truncated in the retrieved text).

**R15** — Owens, A.C.S. & Lewis, S.M. (2018). The impact of artificial light at night on nocturnal insects: A review and synthesis. *Ecology and Evolution* 8(22): 11337–11358. https://doi.org/10.1002/ece3.4557. **FT** (PMC6262936). Retrieved 2026-11-26.
> "Early light exposure experiments conducted in the laboratory demonstrated that sufficiently bright light (from 50 to 1,000 lux) completely inhibits bioluminescent signaling in several firefly species" · "Although lux is widely used by engineers and policymakers, and is easiest to measure, it poorly approximates brightness as it is perceived by non-human animals" · "0.05 lux, similar to that produced by a quarter moon" · "They established four pairs of 20-m-diameter plots, placing a downward-facing LED floodlight (301 lux at plot center) at the center of each plot."

**R16** — Russo, D. & Ancillotto, L. (2015). Sensitivity of bats to urbanization: a review. *Mammalian Biology* 80(3): 205–212. https://doi.org/10.1016/j.mambio.2014.10.003. **FT** (PMC7094881). Retrieved 2026-11-26.
> "The response of bats to this process is highly species-specific: some species tolerate urban habitat or are even favoured by its roosting or foraging opportunities, others are affected by the loss or fragmentation of key natural habitat, or by the physical and chemical pollution associated with urbanization."

**R17** — Ministerie van BZK / IPLO (2020). *Uitvoering motie lichthinder* (leidraad, december 2020). https://iplo.nl/publish/pages/166287/leidraad_uitvoering_motie_lichthinder_december_2020.pdf. **FT** (complete, 17,457 characters). Retrieved 2026-11-26.
> "Overheden maken, afhankelijk van de locatie en gewenste activiteiten, een belangenafweging bij het toestaan van kunstlicht." [Gloss: authorities weigh interests when permitting artificial light, depending on location and intended activity.] · Negative finding, stated as a check: the string "lux" occurs **0 times** in the retrieved document.

**R18** — Wintle, B.A., Kujala, H., Whitehead, A., Cameron, A., Veloz, S., Kukkala, A., Moilanen, A., Gordon, A., Lentini, P.E., Cadenhead, N.C.R. & Bekessy, S.A. (2019). Global synthesis of conservation studies reveals the importance of small habitat patches for biodiversity. *PNAS* 116(3): 909–914. https://doi.org/10.1073/pnas.1813051115. **FT** (PMC6338828). Retrieved 2026-11-26.
> "We undertook a global synthesis of the relationship between the conservation value of habitat patches and their size and isolation, based on 31 systematic conservation planning studies across four continents." · "We found that small, isolated patches are inordinately important for biodiversity conservation." · "Our results provide a powerful argument for redressing the neglect of small, isolated habitat patches … and for avoiding simplistic application of island biogeography theory in conservation decisions."

**R19** — Pfeifer, M., Lefebvre, V., Peres, C.A., et al. (2017). Creation of forest edges has a global impact on forest vertebrates. *Nature* 551: 187–191. https://doi.org/10.1038/nature24457. **FT** (PMC5681864, author manuscript). Retrieved 2026-11-26.
> "We assembled an unmatched global dataset on species responses to fragmentation and developed a new statistical approach … to quantify edge-determined changes in abundance of 1673 vertebrate species." · "We show that 85% of species' abundances are affected, either positively or negatively, by forest edges." · "Forest core species, which were more likely to be listed as threatened by the IUCN, only reached peak abundances at sites farther than 200-400 m from sharp high-contrast forest edges." · "nearly 20% of the world's remaining forest now found within 100 m of an edge, 50% within 500 m and 70% within 1 km" · "The abundances of 11%, 30%, 41% and 57% of bird, reptile, amphibian and mammal species, respectively, showed strong declines towards forest edges."

**R20** — Stankey, G.H., Cole, D.N., Lucas, R.C., Petersen, M.E. & Frissell, S.S. (1985). *The Limits of Acceptable Change (LAC) system for wilderness planning.* Gen. Tech. Rep. INT-GTR-176. USDA Forest Service. https://research.fs.usda.gov/treesearch/66741. **ABS** (landing page + abstract; the 8.99 MB PDF was not downloaded). Retrieved 2026-11-26.
> "A wilderness management-by-objectives planning system is outlined. Through identification of standards, acceptable wilderness conditions are defined and appropriate management actions formulated. A case example is provided."

**R21** — Hausser, Y., Travis, T. & Finger-Stich, A. (2006). Beyond Carrying Capacity in Recreation Management: In Search of Alternatives. In Siegrist, D., Clivaz, C., Hunziker, M. & Iten, S. (eds), *Exploring the Nature of Management*, Proc. 3rd Int. Conf. on Monitoring and Management of Visitor Flows in Recreational and Protected Areas, Rapperswil, pp. 189–192. https://mmv.boku.ac.at/refbase/files/hausser_yves_travi-2006-beyond_carrying_capa.pdf. **FT.** Retrieved 2026-11-26.
> "It is in fact very difficult to establish a mechanical relationship between the level of frequentation and the degree of impacts." · "The actors who most cling to the CC concept are managers and policy-makers who interpret it in normative terms. But even this normative use is a fallacy" · "decision making processes often define CC by considering site-specific objectives and related activities, which is indeed tautological and permits the legitimization of one sided interests"

**R22** — USDA Natural Resources Conservation Service. *Soil Health — Bulk Density* (Soil Health Guide sheet). https://www.nrcs.usda.gov/sites/default/files/2022-11/Bulk%20Density%20-%20Soil%20Health%20Guide_0.pdf. **FT** (complete, 4,190 characters). Retrieved 2026-11-26.
> Table "General Relationship of Soil Bulk Density to Root Growth Based on Soil Texture": "Sand, Loamy Sand <1.60 | 1.63 | >1.80"; "Sandy Loam, Loam <1.40 | 1.63 | >1.80"; "Silt, Silt Loam <1.40 | 1.60 | >1.75"; "Silt Loam, Slity Clay Loam <1.40 | 1.55 | >1.65"; "Sandy Clay, Silty Clay, Clay Loam <1.10 | 1.49 | >1.58"; "Clay (<45 percent clay) <1.10 | 1.39 | >1.47" (columns: ideal for plant growth / affects root growth / restricts root growth, g/cm³). Footnote: "Does not apply to red clayey soils and volcanic ash".

**R23** — Mikula, P., Grünwald, J. & Reif, J. (2025). Species' urbanization time but not present urban tolerance predicts avian fear responses towards human. *BMC Biology* 23. https://doi.org/10.1186/s12915-025-02427-0. **FT** (PMC12492597). Retrieved 2026-11-26.
> "Here, we examined whether avian flight initiation distance (a proxy of fear)—the distance at which a bird flees from an approaching human—is associated with a species' timing of urban colonization" · "Using standardized data from 4420 flight initiation distance observations across 68 species, we applied Bayesian phylogenetic mixed models" · "we collected both in the same city (Prague, Czechia)".

**R24** — Ticktin, T. (2004). The ecological implications of harvesting non-timber forest products. *Journal of Applied Ecology* 41(1): 11–21. https://doi.org/10.1111/j.1365-2664.2004.00859.x. **Metadata only** — identified via Europe PMC AGRIS record and marked "Free" through Unpaywall, but not retrieved (Wiley domain, see access log). Retrieved 2026-11-26. **No claim or number in this file rests on R24.**

**R25** — Schmidt, I.B. & Ticktin, T. (2012). When lessons from population models and local ecological knowledge coincide — Effects of flower stalk harvesting in the Brazilian savanna. *Biological Conservation* 152: 187–195. https://doi.org/10.1016/j.biocon.2012.03.018. **ABS** (Europe PMC AGRIS abstract). Retrieved 2026-11-26.
> "We combined ethnoecological interviews, seed phenology surveys over a large geographical area and harvest experiments in nine sites over 3 years to assess local ecological knowledge and management of golden-grass and its long-term effects on population dynamics." · "Matrix population models illustrate that harvest according to traditional management practices had no impact on golden-grass population dynamics. Earlier harvest of golden-grass, as practiced by new artisans, leads to population decline due to plant uprooting."

**R26** — Gaoue, O.G. & Ticktin, T. (2010). Effects of harvest of nontimber forest products and ecological differences between sites on the demography of African mahogany. *Conservation Biology* 24(2): 605–614. https://doi.org/10.1111/j.1523-1739.2009.01345.x. **ABS** (Europe PMC AGRIS abstract). Retrieved 2026-11-26.
> "In particular, we examined the effect of bark and foliage harvest on the demography of populations of African mahogany (Khaya senegalensis) in two contrasting ecological regions of Benin, West Africa." · "K. senegalensis bark and foliage harvest significantly reduced its stochastic population growth rates, but ecological differences between regions had a greater effect on population growth rates than did harvest."

---

## What would change the answer

- A visitors-per-hectare figure for a Dutch or Belgian urban park, with a measured ecological response variable. Nothing retrieved supplies one; if one exists it is most likely in Dutch grey literature (the WUR `library.wur.nl` 403 above is the likeliest home) or in a municipal/Provincial monitoring report.
- A lux-based Dutch ecological guidance value for bats or insects. The national leidraad is procedural only (`R17`); a provincial or Rijkswaterstaat guidance document with lux contours would change §8 from "no threshold" to "documented guidance".
- A NW-European replication of the dog-walking bird experiment (`R6`). The 35%/41% figures are single-witness and Australasian; if they do not replicate in a Dutch park, item 5's disturbance claim weakens sharply.
- Any study connecting recreational pass-counts to bulk density in a temperate soil. That single study would convert §2 from "mechanism only" to a usable threshold chain.
- A visitor-load × patch-size interaction study. That is the one experiment that would settle item 12.

## Dead ends and search-quality notes

- Europe PMC author search for Reijnen is contaminated by a same-named medical-imaging author; title search for the 1997 *Biodiversity & Conservation* paper returned 0 hits (not indexed). The thesis (`R13`) was the accessible route to the same numbers, and it is the primary source.
- A search snippet attributed a Dutch recreation-capacity/"sociale capaciteit" statement to `library.wur.nl/WebQuery/wurpubs/fulltext/211959` ("De totale lengte aan (wandel)paden in een gebied is een cruciaal kenmerk van het fysieke aanbod als het gaat om de sociale capac…"). The record was **403** and the quoted sentence could not be verified. **Do not use that sentence; it is a snippet, not a source.**
- Europe PMC searches for "music festival" + soil/vegetation return mostly irrelevant records (wildfire, strawberry cultivars); the one usable hit is `R11`.
- FID literature is large (213 hits) but is dominated by behavioural-ecology questions (urban tolerance, predator recognition) rather than buffer-distance guidance. No disturbance-distance table for pedestrians in NW European parks was found.

## Adjacent questions noticed, not researched

1. Whether *mowing regime* or *drainage* effects on the same vegetation outweigh visitor effects — the "management vs visitors" comparison (`R9` hints at it; no study retrieved tests it).
2. Whether urban green space design (path layout, surfacing, screening) measurably reduces trampling/compaction at equal visitor numbers. Effort-based design literature exists (e.g. `R5`'s recommendation) but no quantified comparison was retrieved.
3. Winter waterbird roost disturbance in Dutch wetlands — a well-developed Dutch disturbance literature that this line did not enter, and which may hold the seasonal-window numbers §4 lacks.
4. Whether food-forest harvesting has any documented ecological effect anywhere in temperate Europe — the search returned nothing, but only English- and Dutch-language queries were run.
