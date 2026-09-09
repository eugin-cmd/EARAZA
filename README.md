# EARAZA Annual Conference 2026

One-page site for the **EARAZA Annual Conference 2026** — 25–30 October 2026,
hosted at Vantara, Jamnagar, Gujarat, India.

## Deploying

A single self-contained file. `index.html` sits at the repo root, so Vercel
needs no build step and no configuration: import the repo, framework
**Other**, root directory **`./`**.

The only external request is Google Fonts (Poppins). Every image — the EARAZA
badge, the Vantara and GZRRC logos, both stripe-pattern panels, the tiger
stripe texture and the seven species photographs — is embedded as a data URI,
so the page also runs from a local file or a subfolder.

## What's in the page

| Section | Notes |
|---|---|
| Banner | Logo row, justified `EARAZA / ANNUAL CONFERENCE / 2026` block, date box, flanking stripe panels |
| About + statistics | 95 member institutions, 24 countries, 20M+ visitors, 25+ programmes |
| Priority species | Seven cards, each linked to the matching Wikipedia article in the selected language |
| Mission, vision, science | Plus the six strategic priorities |
| Programme | All six days, 25–30 October |
| Attending | Eligibility, fee, and the ten inclusions |
| Getting there | JGA / HSR, connecting hubs, visa + insurance + NDA |
| Hosts | Vantara and GZRRC, with both leadership quotes |
| FAQ | 24 questions across four categories |

## Languages

Seven locales: **en · ru · es · fr · de · zh · pt**, via the globe switcher in
the header. Choice persists in `localStorage`; the browser language is used on
a first visit.

Official EARAZA copy (hero, about, mission, both quotes, the full schedule and
all registration text) comes from the association's own locale table. The
deck-derived sections and all 24 FAQ answers were translated for this build.

The justified title block measures itself at runtime, so the three lines stay
flush to one measure in every language rather than only in English.

## Design source

Follows the EARAZA event branding deck: orange `#E2662F` fields with the
tone-on-tone tiger stripe, dark navy `#14262C` headings on white, thin rules,
teal and lime accent cards, Poppins throughout.

## Open items

- **"Musk ox" card** — the deck's photograph appears to be a European bison
  (*Bison bonasus*), not a muskox. Either the label or the image needs
  swapping; the binomial is intentionally omitted until that is settled.
- **"Rare reptile species" card** — a generic label, so it carries no
  Wikipedia link. The photograph is a veiled chameleon.
- **Translations** — the non-official strings should get a native-speaker
  review before launch, since they carry visa and insurance detail.
- **Image licensing** — the species photographs and the medallion imagery in
  the stripe panels come from the brand deck and may be licensed stock.
  Confirm the licences cover public web use.
