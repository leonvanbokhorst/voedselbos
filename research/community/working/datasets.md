# Working note — the two open-data sets, computed by hand

Not evidence in itself; the counts below are reproduced in `../note.md` §3.3 and the metadata is in `../sources.md`.
Retrieval: 26 November 2026, over HTTPS from the municipal open-data API (`data.eindhoven.nl`, OpenDataSoft v2.1). The
exports were downloaded whole and counted locally with `python3`; sha256 of the exact bytes is recorded below so a
reader can re-check the arithmetic.

## A. `vergroeningsprojecten` (Vergroeningsprojecten / Wensenkaart)

- Export URL: `https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroeningsprojecten/exports/json`
- 200, 81 786 bytes, sha256 `9ba8b9b25af0bfc21b7a99a152a9e574c0afb0ba5edf79701a0eb0d47e3fa5fb`
- Dataset metadata (`.../catalog/datasets/vergroeningsprojecten`), `modified` **2026-11-20T23:01:46+00:00**, `records_count` **124**.
- **124 records**, confirmed by count of the export.

Fields (verbatim from the catalogue, label / description as published):

| field | label | description |
|---|---|---|
| `binnengekomen_via` | BINNENGEKOMEN_VIA | "geco = gebiedscoordinator" |
| `betrokkenheid_bewoners` | BETROKKENHEID_BEWONERS | "laag, redelijk, of hoge betrokkenheid" |
| `type` | TYPE | "Wensenkaart vergroeningsprojecten (wens), of onderdeel van project actief ontharden" |
| `verwacht_aantal_m2_nieuw_groen` | — | "Aantal m2 die het betreft." |

Counted distributions:

- `status`: Kans of wens **56**, Lopend **21**, Uitgevoerd **20**, empty **16**, Afgevoerd **9**, On hold **2**.
- `binnengekomen_via`: `geco` **39**, `bewonersi` **31**, empty **21**, `collega` **11**, `anders` **11**, `buitenBet` **10**, `bouwteam` **1**.
- `betrokkenheid_bewoners`: empty **33**, matig **26**, redelijk **24**, laag **22**, hoog **19**.
- `uitvoeringsjaar_gepland`: empty **104**; 2025 **11**, 2023 **6**, 2024 **3** → **20** records with a planned year (the
  repository's participation note said 14; the export now shows 20, so the note's figure is superseded by the 20 Nov 2026 revision).
- `datum_ingediend`: 90 dated records, **2023-05-23** to **2026-09-15**.
- `type`: Wens 111, Actief ontharden 13.
- No record contains an `@`, i.e. no e-mail address anywhere in the free-text field; no name field exists at all.

Cross-tabulation `binnengekomen_via` × `betrokkenheid_bewoners` (this is the new finding):

| origin | laag | matig | redelijk | hoog | empty | total |
|---|---|---|---|---|---|---|
| `geco` (area coordinator) | 5 | 0 | 12 | **13** | 9 | 39 |
| `bewonersi` (resident initiative) | 1 | 20 | 6 | **4** | 1 | 31 |
| `collega` (municipal colleague) | 2 | 4 | 4 | 0 | 1 | 11 |
| `anders` | 10 | 0 | 1 | 0 | 0 | 11 |
| `buitenBet` (external party) | 4 | 2 | 1 | 0 | 3 | 10 |
| `bouwteam` | 0 | 0 | 0 | 1 | 0 | 1 |
| empty | 0 | 0 | 0 | 1 | 20 | 21 |

So of the 19 records rated "hoog", **13 came in through an area coordinator** and 4 from residents. Of the 31
resident-initiated records, 20 are rated only "matig".

`type` × `binnengekomen_via`: the 13 "Actief ontharden" records — which the dataset's own description says are
"aangedragen door bewoners" — split as empty 6, `geco` 5, `buitenBet` 1, `bewonersi` 1.

## B. `vergroenen-groenarme-buurten` (green-poor neighbourhoods)

- Export URL: `https://data.eindhoven.nl/api/explore/v2.1/catalog/datasets/vergroenen-groenarme-buurten/exports/json`
- 200, 32 523 bytes, sha256 `ea2cfc76e575dfac7ae325d68bcbbe84254a62dd27056f977c82b636577c37d2`
- Metadata `modified` **2026-11-22T22:00:28+00:00**, `records_count` **70**; **70 records** counted.
- Definition, verbatim from the dataset description: "Buurten met minder dan 75m² openbaar groen per woning zijn
  getypeerd als groenarme buurten." Nine selected neighbourhoods: Bloemenplein, Gildebuurt, Hemelrijken, Joriskwartier,
  Lakerlopen, Limbeek-Noord, Limbeek-Zuid, Rochusbuurt, Tivoli.
- `status`: Lopend 51, Nieuw 19. `buurt` counts: Hemelrijken 12, Tivoli 9, Gildebuurt 9, Limbeek-Zuid 7, Bloemenplein 6,
  Lakerlopen 6, Joriskwartier 5, Rochusbuurt 4, Limbeek-Noord 3, then singletons including two spellings of Limbeek-Noord
  ("Limbeek-Noord" and "Limbeek Noord") — a small coding inconsistency worth knowing before any count is made per buurt.
- The Limbeek-Zuid residents' initiative, verbatim: locatie "Aletta Jacobsplein – Roosje Vosstraat", status "Nieuw",
  `uitvoeringsjaar` empty, omschrijving: "**Initiatief vanuit de natuurwerkgroep (buurtbewoners) en beheer: voormalig
  hondenuitlaatterrein een extra groene invulling geven.**"
- Other documented residents' arrangements in the same set: Tivoli "Buurttuin "Verborgen Hof". Wordt door buurtbewoners
  gerund, grond van Woonbedrijf."; Bloemenplein "Een deel is in eigen beheer van de bewoners (beheerovereenkomst Gemeente
  en Stichting Bloemenbuurt Noord en bewoners). Zij onderhouden tuin (oa kruiden)."; Tivoli "Aanleg geveltuintjes
  Leeuwenstraat — Initiatief Woonbedrijf met bewoners."

## C. What the two sets cannot show

Neither set records a participant, an attendee, an age, a tenure status, an income, a language or a household. There is
no field in which a resident speaks in their own words; every description is a staff paraphrase. Neither set records
whether a wish was executed *with* the residents who asked for it, only a status and (sometimes) a planned year. So a
count from these sets is a count of *records about* participation, produced by the party that also decides what counts
as participation.
