# The Adoption Deck — Art Assets

**Style decision:** the deck's identity is warm paper-and-sage — the consulting
site's daylight world, deliberately distinct from the Judgement Deck's
brass-lamp noir. All generated art uses the locked **sage daylight** identity.
Every prompt starts with this canonical prefix:

```
warm editorial photograph, cream paper and sage-green palette, soft diffused
daylight from a window, clean minimal composition, generous calm negative
space, shallow depth of field, natural wood and linen textures, quiet
professional atmosphere
```

Every prompt ends with:

```
no text, no letters, no words
```

Card faces stay typographic; art lives on the box, the back, the banner and
the art-edition banner zone.

## Regenerating

```sh
limn generate -s 768x1024 -o assets/art/cover.png "<prefix>, <subject>, no text, no letters, no words"
```

Provider: the default SwarmUI (`juggernautXL_v9`). Each `.png.json` sidecar
records the exact prompt and parameters.

## Files

| File | Use | Subject |
|---|---|---|
| `cover.png` | Box front, landing hero art | Boardroom table by a window, index cards on a sage folder, tea |
| `back.png` | Deck back when printed double-sided | Sage green with cream linework; central emblem is an oak leaf medallion |
| `banner.png` | Social preview, landing banner | Top-down boardroom table, five rows of cards being sorted |

## ill/ — the concept-keyed vignette library

Five landscape vignettes, one per section, keyed by concept. The art edition
tints each in its section colour at render time (CSS hue-rotate from a sepia
base): sage Can we, rust Should we, slate How, ochre Ready, plum Value.

| File | Section | Subject |
|---|---|---|
| `can.png` | Can we do AI? | Archive boxes on a shelf, one pulled forward |
| `should.png` | Should we do AI? | Brass balance scale, weights on one pan, folded card on the other |
| `how.png` | How would we do it? | Index cards in sequence, one held above the next empty position |
| `ready.png` | Are we ready? | Wooden garden gate slightly open onto a gravel path |
| `value.png` | What's the value? | Leather ledger open beside a fountain pen, light across the columns |
