# Working notes — #14

## Delegation: attempted, refused, not performed

Two bounded subagent briefs were written and submitted, and **both were refused by the session's child-agent limit** ("subagent limit reached (active child limit: 16)"), which was already saturated by sibling researchers in the same session. No delegation took place. Both lines were then worked by the researcher alone, to a lower standard than intended.

The two briefs, recorded so a later pass can pick them up:

1. **Dated founding genealogy** — for each named initiative (De Vergeten Tuin/Vereniging Veldwerk, Wasven, Phood Farm, Trefpunt Groen Eindhoven, Struikroven, Stadsakkers, TransitieStad Eindhoven, De Wielewaal, Voedselbos Eindhoven, the Henri Dunantpark food forest, De Buurtwerf, De Block Acker, Bij Albrecht, Victoriapark): founding date, founders, land and tenure, money, legal form, current status — with the Wayback snapshot date recorded for every archived page and a one-witness/two-witness judgement for every claim. **Not performed.** `note.md` carries the date coverage it could reach from the sibling notes plus the new retrievals; the pre-2014 and 2019–2025 chains are thin.
2. **Municipal and provincial policy-and-land timeline 2000–2026** — Duurzaamheidspact; the green-policy chain (Kadernota/Structuurvisie/Groenbeleidsplan/Omgevingsvisie); **the successive editions of the Beleidsregel groen en water**, which would settle whether an earlier edition had a community-management route for "middel of hoog" green; the groensubsidie's introduction and any earlier non-owner version; the Lichtbos council decision; the February 2022 Wielewaal purchase; Strijp-S and Strijp-R development; **a comprehensive gemeenteblad search on "Elburglaan" across all years**; provincial nature/agriculture subsidy lines and the Regiodeal. **Not performed.**

Both would materially strengthen `note.md` §7 (path dependencies) and §3 (timeline). Neither would change the §4 reconstruction, which rests on documents already retrieved.

## Retrieval technique that worked

The platform's site was a **client-side Wix application**: every archived HTML capture returns only "Loading" or the page title. The way in was the **RSS feed** (`/feed.xml`), archived at seven timestamps between 2015 and 2018. Parsing all `<item>` elements for `pubDate` / `dc:creator` / `title` produced the platform's own dated chronology — 45 items in the 2016-05-19 capture, 50 in the 2018-06-30 capture. That is the backbone of `note.md` §3 and §4.

The second technique that worked: **notubiz blocks, the mirror host does not.** `eindhoven.notubiz.nl/document/1771480/1` returned 403 with a Cloudflare challenge and a `cf-ray`; the same document id on `raadsinformatie.eindhoven.nl` returned 200 with full text. The two hosts serve the same corpus.

The technique that failed: recovering the platform's own inventory of the city's initiatives (`/stadslandbouw-in-040-lijst`, `/stadslandbouw-in-040-kaart`) — archived, 200, and unreadable without a JavaScript renderer.

## What a next pass should do first

1. Ask the municipality in writing for the **Visie Stadslandbouw** (July 2016). Its own authors describe it as available "op aanvraag" — a free, legitimate request, and the document that decides whether three years of process produced an instrument or a PDF.
2. Retrieve the **December 2014 motion** text from the council's file (`raadsinformatie`/`notubiz`, motion of the week of 16 December 2014).
3. Run the gemeenteblad search on **"Elburglaan"** across all years, and look for any disposal or lease of Elburglaan 8.
4. Check **KVK** directly for Proeftuin040 (nothing found by search; a register query would settle whether it ever had a legal form).
5. Recover the **"Rapport Stadslandbouw Nederland 2018–2020"** (DuurzaamDoor/RVO) from another host — the archived PDF is corrupt and the live one has been withdrawn.
