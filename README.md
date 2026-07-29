# Bāla Saṁskāra & Janma Doṣa Guide

*An Astrogaami tool for early-childhood spiritual planning*

A single-file, offline HTML tool that reads a newborn's chart data, identifies
sensitive natal points (Gandanta and intensity nakshatras), and generates a
clean, printable **Saṁskāra timeline** — the traditional developmental and
spiritual milestones of the first years of life.

No install, no server, no data leaving the device. Open the `.html` file in any
browser and it works.

---

## Why this tool exists

In classical Jyotisha, the early life of a child is not left to chance. The
*saṁskāras* — Nāmakaraṇa (naming), Niṣkramaṇa (first outing), Annaprāśana
(first grain), Karṇavedha (ear piercing), Cūḍākaraṇa (tonsure), and
Upanayana / Vedārambha (initiation into learning) — are timed rites that mark
both spiritual and developmental transitions.

Two problems make this hard for a practitioner in practice:

1. **Chart data is scattered.** The Janma Nakshatra, pāda, tithi, weekday, and
   the sensitive points a chart carries all have to be read off separately and
   assembled by hand for every child.
2. **The saṁskāra schedule is easy to garble.** Timings shift by gender and by
   tradition, and parents need it explained in plain language, not jargon.

This tool collapses both into a single paste-and-generate workflow, so the
practitioner can spend attention on judgement rather than clerical assembly, and
hand the family a dignified, readable report.

---

## What it does

- **Parses JHora output directly.** Paste the *Body Longitude* table and the
  *Date / Tithi / Yoga* panchanga block from JHora into two boxes — no
  reformatting needed. The parser handles both old and new JHora spellings,
  3- and 4-character nakshatra codes, retrograde and karaka annotations, and
  the DMS longitude format.
- **Identifies the Janma Nakshatra and pāda** from the Moon, and lays out every
  body's nakshatra placement in a status table.
- **Flags sensitive natal points:**
  - **Gandanta** — the water–fire junctions at Ashwini 1 / Revati 4,
    Magha 1 / Ashlesha 4, Mula 1 / Jyeshtha 4. Marked as high-priority for
    muhurtha-based remedies.
  - **Sensitive nakshatras** — Mula, Ashlesha, Jyeshtha — marked as
    higher-intensity energy calling for steady mantra and prayer.
  - Everything else is marked **Supportive** (naturally stable).
- **Generates a gender-aware Saṁskāra timeline.** Annaprāśana is set to the
  6th month for boys and the 5th month for girls, per tradition; the rest of the
  milestones carry short developmental checkpoints (neck-holding, social smile,
  hand–eye coordination, and so on) so the report doubles as a practical
  parenting guide.
- **Produces a print-ready report** with an editable title, subtitle, and
  astrologer's signature line — double-click any heading in the report to edit
  it before printing or saving to PDF.

---

## How to use it

1. Open `Janma_Dosha_v3b.html` in any modern browser.
2. In **Planet Longitudes (A)**, paste the Body Longitude table from JHora.
3. In **Panchanga Data (B)**, paste the Date / Tithi / Yoga block from JHora.
4. Enter the child's name and select gender.
5. Click **Analyze** to see the nakshatra status table.
6. Click **Generate Report** for the full printable Saṁskāra guide.
7. (Optional) Set your report title and digital signature in the settings, then
   print or "Save as PDF" from the browser dialog.

**Tip:** if parsing returns too few bodies, the tool will tell you — recheck
that the full longitude table was copied, not just a fragment.

---

## Design notes

- **Single file, fully offline.** All logic lives in one HTML file. Nothing is
  uploaded anywhere; birth data never leaves the user's machine. This is
  deliberate — natal data of a child deserves privacy by default.
- **Astrologer in the loop.** The tool surfaces and organises data; it does not
  pretend to replace the practitioner's judgement. The saṁskāra timings and
  remedy pointers are starting frames, meant to be refined against the full
  chart and muhurtha analysis.
- **JHora-native.** Input is designed around JHora's copy-paste output so it
  fits existing workflows rather than demanding re-entry.

---

## Scope and limitations

- Sensitivity flagging currently covers **Gandanta** and the three
  intensity nakshatras (Mula, Ashlesha, Jyeshtha). It is a triage layer, not a
  full doṣa audit — Bhakoota, Mangala, and other analyses are out of scope here.
- Saṁskāra timings follow a common traditional schedule; regional and family
  traditions vary, and the practitioner should adjust accordingly.
- The tool assists planning and education. It is **not** medical advice; the
  developmental checkpoints are general guidance, not a substitute for a
  paediatrician.

---

## License

Released under the **MIT License**.

```
MIT License

Copyright (c) 2026 Astrogaami

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

*Offered as a gift to the Jyotisha community. — Astrogaami*
