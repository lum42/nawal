# Los veinte días · The twenty days

A nawal calculator and a cross-tradition reference for the twenty Maya day-signs
(*tzolk'in* / *cholq'ij*), built from published sources only.

**Live:** https://lum42.github.io/nawal/ — one file, works offline, Spanish and English.

## What it does

- **Calculator.** Pick a date → the day's coefficient (drawn as a Maya bar-and-dot numeral), its
  name, and the names the same slot carries in thirteen language traditions. GMT correlation
  584283 (21 Dec 2012 = 4 Ajaw); the birth nawal is read on the Guatemalan civil day.
- **Wheel.** The twenty days as a ring, with the everyday readings: force, glyph, animal
  companion, office, the Komon Tohil etymology, and the divinatory character.
- **Names.** All twenty days across thirteen columns: K'iche', Yucatec, Kaqchikel, Mam, Ixil,
  Poqomchi', Chuj, Q'anjob'al, Jakalteko, Tzeltal, Chicomuceltec, Proto-Ch'olan and Nahuatl.
- **Bridges.** The five places where the traditions genuinely disagree — the K'at/K'an false
  friend, Lamat/Q'anil/Tochtli, Kab'an/No'j, Kawak's etymological thunder, and the three
  year-bearer sets.
- **Sources.** Every claim tiered A (peer-reviewed or primary), B (institutional or organised
  tradition), C (popular, orientation only), with a coverage matrix that says which traditions
  are complete and which are still open.

## Files

| file | what |
|---|---|
| `index.html` | the whole app, self-contained, no dependencies |
| `days.json` | the dataset, also inlined into `index.html` |
| `RESEARCH.md` | the write-up: evidence layers, the elements question, the divergences, the gaps |
| `LICENSE` | CC BY-SA 4.0 for text and data, MIT for the code |

## Dataset schema (`days.json`)

| field | meaning |
|---|---|
| `seq` | position 1–20 in the count |
| `kiche` | K'iche' name (standard orthography) |
| `yuc` | 16th-c. Yucatec name (Landa's orthography) |
| `kaq` | 1685 Kaqchikel spelling |
| `chuj`, `qan` | Ministerio de Cultura, *Armonización Maya*, Cuadro 1 |
| `nah` | Aztec/Nahuatl counterpart, same slot |
| `names` | the same slot in all thirteen traditions |
| `glyph` | Classic glyph reading (Kettunen & Helmke; Miller & Taube) |
| `classic` | reconstructed Classic-period word, `—` where unknown |
| `force` | the day's natural force, from the etymologies |
| `animal`, `office` | animal companion; social role (**editorial synthesis**) |
| `kt` | Komon Tohil (Zunil) etymology and role |
| `div` | divinatory character (Weeks, Sachse & Prager 2009) |
| `note` | divergences and traps |
| `es` | Spanish text for the fields above |

## Rebuilding

`index.html` is generated: `days.json` is inlined at the `__DAYS__` placeholder in
`app2.template.html` (kept in the author's working copy, not in this repository).

## Cautions

- The twenty *positions* are shared; the *names* are not translations of each other, though most
  are cognates within the Mayan family.
- None of the sources consulted documents a pre-Hispanic four-element scheme for the days.
  Individual days do carry a natural force, and Kawak's is etymological (proto-Mayan *kahoq).
- Dreamspell "seals" are a separate 20th-century system and are excluded.
- A local *ajq'ij*'s count can run a day off the GMT correlation; inside a community, that count
  governs.
- This is cultural and divulgative material. It is not medical, psychological or religious advice.

## Licence

Text and data: CC BY-SA 4.0. Code: MIT. Quotations and figures from the cited works remain with
their authors; the bibliography is in `RESEARCH.md`.
