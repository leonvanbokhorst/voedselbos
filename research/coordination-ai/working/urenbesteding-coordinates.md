# Trefpunt Groen Jaarverslag 2025 — 'Urenbesteding 2025' chart: coordinate extraction

Re-fetched the PDF directly (curl, 2026-11-26) and confirmed the bytes are identical to the
`source_read` retrieval: sha256 begins 7ee352566e828c25 (same as sources.md §1 [S20]).
Extracted with `pdftotext -bbox -f 22 -l 22`. The pie chart is a vector graphic, so the plain
text stream interleaves labels and percentages in an order that cannot be read as a list —
which is how a reader can pair '5%' with 'Netwerk intensiveren' or with 'Overige projecten'.

Two independent pairings — nearest label box, and smallest angular difference from the
chart centre (740,405) — agree on all seven categories:

label                            pct    centre       box-dist radial partner
--------------------------------------------------------------------------
Managementtaken en administratie 5%     (718,290)    47.2     same
Afstemming achterban             15%    (789,302)    53.7     same
Communicatie                     20%    (644,335)    54.1     same
Kapaanvragen adviseren           20%    (849,401)    52.5     same
Netwerk intensiveren             5%     (620,419)    54.0     same
Overige projecten                10%    (642,466)    51.8     same
Omgevingsplannen adviseren       25%    (754,514)    48.2     same

Sum 5+20+15+5+10+20+25 = 100.

The seven distances fall in a narrow 47-54 pt band, which is the signature of a correct
one-to-one assignment (each percentage sits just outside its own label's leader line).

The PI's verification read the two mid-list values the other way (Netwerk 10%, Overige 5%).
Both readings sum to 100, so arithmetic cannot settle it. **It does not affect the argument**:
under either reading there are two categories at 5%, so administrative work is tied for
smallest rather than uniquely smallest, and the 45% advisory share is an aggregation of
kapaanvragen (20) + omgevingsplannen (25) rather than a figure the report prints.
