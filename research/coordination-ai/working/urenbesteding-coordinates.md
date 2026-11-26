# Trefpunt Groen *Jaarverslag 2025* — the "Urenbesteding 2025" donut: how the pairing was settled

**Status: settled.** The seven label→percentage pairs are now established by rendering the page, not inferred from text. The pairing is:

| Label | Share |
|---|---|
| Managementtaken en administratie | **5%** |
| Communicatie | **20%** |
| Netwerk intensiveren | **5%** |
| Overige projecten | **10%** |
| Omgevingsplannen adviseren | **25%** |
| Kapaanvragen adviseren | **20%** |
| Afstemming achterban | **15%** |

Sum 100. Source: Stichting Trefpunt Groen Eindhoven, *Jaarverslag 2025*, p. 22, `https://www.trefpuntgroeneindhoven.nl/uploads/Nieuws/jaarverslagen/TGE%20Jaarverslag%202025.pdf` (sha256 begins `7ee352566e828c25`, identical to the `source_read` retrieval recorded in `../sources.md` `[S20]`).

## Why the text layer could not settle it, and what did

The chart is a **donut with external labels and leader lines** — a vector graphic. Its text stream lists labels and percentages in an order that does not correspond to the segments, so any pairing read off `pdftotext` (with or without `-layout`) is an artefact of extraction order. Two different readers of the same plain text can and did reach opposite pairings, and both sum to 100, so arithmetic cannot discriminate.

**Decisive method — render the page and look at the leader lines** (2026-11-26):

```
pdftoppm -f 22 -l 22 -r 150 -png -x 1000 -y 420 -W 1120 -H 850 \
  "TGE Jaarverslag 2025.pdf" donut
```

Crop committed as [`donut-22.png`](donut-22.png) (1120×850, 254 kB) so a reviewer can check the pairing without a toolchain. It shows, clockwise from the pale top segment: *Managementtaken en administratie* 5% → *Afstemming achterban* 15% → *Kapaanvragen adviseren* 20% → *Omgevingsplannen adviseren* 25% → *Overige projecten* 10% → *Netwerk intensiveren* 5% → *Communicatie* 20%.

**Corroborating method — word coordinates** (`pdftotext -bbox -f 22 -l 22`). Pairing each percentage to its nearest label box, and independently to the label with the smallest angular difference from the chart centre (740, 405), both agree with the rendered reading on all seven, at a consistent 47–54 pt distance — the signature of a correct one-to-one assignment rather than a coincidence.

## The correction this settled

The first draft of [`../note.md`](../note.md) reported only four categories and presented "**45% on advice**" as a figure the report prints. Both were wrong: the document publishes **seven** categories, and 45% is *the note's own aggregation* of kapaanvragen adviseren (20%) plus omgevingsplannen adviseren (25%). The note now gives all seven values, labels the aggregation as such, and says administrative work is **tied for smallest** — management/administratie and netwerk intensiveren both at 5% — rather than uniquely smallest.

## History, briefly

The PI's first verification read the two mid-list values the other way (netwerk 10% / overige 5%) from a `pdftotext -layout` line order. I recorded the disagreement rather than absorbing it, on the ground that a pairing my two geometric methods contradicted should not be adopted on authority. The PI then rendered the page, found the same pairing recorded above, and withdrew the objection. Two independent methods now agree with the rendered page, and the ambiguity is closed rather than carried.
