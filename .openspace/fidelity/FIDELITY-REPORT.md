# Visual fidelity

Overall match: **71/100** — fonts, type sizes, spacing and each section measured in a browser on both sites (75%), and how alike the pages look as pictures (25%). How it's scored: docs/qa/import-fidelity.md.

Scored two ways, side by side: **71/100 corrected**, 71/100 by the strict v3 scorer. The corrected score reads three things the strict one gets wrong (navigation in a header themed "brand", off-screen slides counted as columns, a picture-only band on a phone); the pages below list where it did.

Auto-tuning raised it from 68/100:

- h1: 149.1px, 91.6px on phones, tracking -0.03em
- section padding 88px
- text on light sections #000000, as on the original (2 of 2 sections)
- heading on light sections #0f3a48, as on the original (1 of 2 sections)
- /research: section 1 "Published Research" recreated as a custom component
- h2: 19.5px, 86.2px on phones, tracking -0.03em

Without custom components: 70/100; with the sections recreated as components: 70/100.

## / at 1440px — 69/100 (strict v3: 65/100)

Corrected scoring on this page:

- The new site's navigation sits in a header themed "brand" (os-theme-brand): read as navigation, not as a logo.

Checks 69/100 · looks alike 69/100 (screenshots compared).

Original: https://www.omniharmonic.com/home/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Instrument Serif | Instrument Serif | same |
| Heading 1 size | 137px | 17px | **differs** |
| Heading 2: present | Instrument Serif 19.5px | not found | **differs** |
| Body font | Public Sans | Public Sans | same |
| Body text size | 16px | 16px | same |
| Label font | Public Sans | Public Sans | same |
| Buttons size | 16px | 16px | same |
| Buttons letter spacing and case | -0.03em, none | -0.03em, none | same |
| Navigation size | 16px | 16px | same |
| Navigation letter spacing and case | -0.02em, none | -0.02em, none | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Section padding | 55px | 44px | same |
| Button corners | 300px | 0px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | I seem to be a verb·I seem to be a verb·I seem to be a verb I seem to be a verb · | 29 | Background: #ffffff → #131313; Columns: 5 → 2; Height: 5913px → 685px |

What would close the gap:

- choices.typography.scale.h1.size = 137
- choices.shape = "round"
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## / at 390px — 61/100

Checks 56/100 · looks alike 76/100 (screenshots compared).

Original: https://www.omniharmonic.com/home/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Instrument Serif | Instrument Serif | same |
| Heading 1 size | 91.6px | 16px | **differs** |
| Heading 2: present | Instrument Serif 18.2px | not found | **differs** |
| Body font | Public Sans | Public Sans | same |
| Body text size | 16px | 16px | same |
| Buttons: present | Public Sans 16px | not found | **differs** |
| Label font | Public Sans | Public Sans | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Section padding | 102px | 28px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | I seem to be a verb·I seem to be a verb I seem to be a verb · | 14 | Background: #ffffff → #131313; Columns: 2 → 1; Image crop: 0.71:1 → 0.31:1; Height: 7276px → 1241px |

What would close the gap:

- choices.typography.scale.h1.sizeMobile = 92
- choices.layout.sectionPaddingMobile = 102
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Use the original's image proportions (the block's aspect ratio).

## /about at 1440px — 88/100

Checks 88/100 · looks alike 91/100 (screenshots compared).

Original: https://www.omniharmonic.com/about/  
Imported: /about (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Instrument Serif | Instrument Serif | same |
| Heading 1 size | 149.1px | 149.1px | same |
| Body font | Public Sans | Public Sans | same |
| Body text size | 16px | 16px | same |
| Label font | Public Sans | Public Sans | same |
| Buttons size | 16px | 16px | same |
| Buttons letter spacing and case | -0.03em, none | -0.03em, none | same |
| Navigation size | 16px | 16px | same |
| Navigation letter spacing and case | -0.02em, none | -0.02em, none | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Button corners | 0px | 0px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | I did it all for love | 67 | Columns: 2 → 1; Image placement: center, 100% wide → none; Height: 12290px → 1082px |

What would close the gap:

- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.

## /about at 390px — 79/100

Checks 78/100 · looks alike 83/100 (screenshots compared).

Original: https://www.omniharmonic.com/about/  
Imported: /about (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Instrument Serif | Instrument Serif | same |
| Heading 1 size | 63.9px | 39px | **differs** |
| Body font | Public Sans | Public Sans | same |
| Body text size | 16px | 16px | same |
| Label font | Public Sans | Public Sans | same |
| Buttons size | 16px | 16px | same |
| Buttons letter spacing and case | -0.03em, none | -0.03em, none | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Section padding | 375px | 66px | **differs** |
| Button corners | 0px | 0px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | I did it all for love | 69 | Heading: Instrument Serif 63.9px → Instrument Serif 39px; Image crop: 0.38:1 → 2.32:1; Height: 17992px → 837px |

What would close the gap:

- choices.typography.scale.h1.sizeMobile = 64
- choices.layout.sectionPaddingMobile = 375
- Use the original's image proportions (the block's aspect ratio).

## /art at 1440px — 61/100

Checks 61/100 · looks alike 61/100 (screenshots compared).

Original: https://www.omniharmonic.com/art/  
Imported: /art (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 2: present | Instrument Serif 128.3px | not found | **differs** |
| Label font | Public Sans | Public Sans | same |
| Navigation size | 16px | 16px | same |
| Navigation letter spacing and case | -0.02em, none | -0.02em, none | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Section padding | 229px | 43.5px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Art | 44 | Background: #ffffff → #131313; Heading: Instrument Serif 128.3px → Instrument Serif 19.5px; Height: 1188px → 594px |

What would close the gap:

- choices.layout.sectionPadding = 229
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).

## /art at 390px — 64/100

Checks 63/100 · looks alike 70/100 (screenshots compared).

Original: https://www.omniharmonic.com/art/  
Imported: /art (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading 2: present | Instrument Serif 86.2px | not found | **differs** |
| Label font | Public Sans | Public Sans | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Section padding | 257px | 20.5px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Art | 56 | Background: #ffffff → #131313; Image crop: 0.66:1 → 0.87:1; Height: 1188px → 450px |

What would close the gap:

- choices.layout.sectionPaddingMobile = 257
- Give the section its own background color (style.background = { type: "color", color: "#ffffff" }).
- Use the original's image proportions (the block's aspect ratio).

## /research at 1440px — 93/100

Checks 97/100 · looks alike 83/100 (screenshots compared).

Original: https://www.omniharmonic.com/research/  
Imported: /research (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Instrument Serif | Instrument Serif | same |
| Heading 2 size | 128.3px | 128.3px | same |
| Body font | Public Sans | Public Sans | same |
| Body text size | 16px | 16px | same |
| Label font | Public Sans | Public Sans | same |
| Navigation size | 16px | 16px | same |
| Navigation letter spacing and case | -0.02em, none | -0.02em, none | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Content width | 1360px | 1360px | same |
| Section padding | 103px | 100px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Published Research | 92 | Image crop: 1.14:1 → 0.8:1 |

What would close the gap:

- Use the original's image proportions (the block's aspect ratio).

## /research at 390px — 53/100

Checks 50/100 · looks alike 61/100 (screenshots compared).

Original: https://www.omniharmonic.com/research/  
Imported: /research (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | Instrument Serif | Instrument Serif | same |
| Heading 2 size | 86.2px | 103px | **differs** |
| Body font | Public Sans | Public Sans | same |
| Body text size | 16px | 14px | **differs** |
| Label font | Public Sans | Public Sans | same |
| Site title size | 16px | 16px | same |
| Site title letter spacing and case | -0.02em, none | -0.02em, none | same |
| Section padding | 124px | 84px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | Published Research | 25 | Heading: Instrument Serif 86.2px → Instrument Serif 103px; Text: Public Sans 16px → Public Sans 14px; Columns: 2 → 1; Image placement: right, 49% wide → center, 87% wide; Image crop: 0.95:1 → 0.8:1; Height: 1217px → 3143px |

What would close the gap:

- choices.typography.scale.h2.sizeMobile = 86
- choices.typography.scale.body.sizeMobile = 16
- choices.layout.sectionPaddingMobile = 124
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.
- Use the original's image proportions (the block's aspect ratio).

