# Job: hero image or key visual for a website

The hero decides the look of the whole site and every asset after it, so it is the first lock. The deliverable is a plate the page ships (no text in it) plus the decision of how text and action sit over or beside it.

## Ready check

- [ ] The page's mode (usually Persuade) and the one action the visitor should take
- [ ] The real headline (about five words) and the one supporting line, written before generating
- [ ] Brand tokens if they exist: palette hex, typefaces, logo, existing imagery. Read them from the site's CSS or design files when you can
- [ ] What the subject is, in the project's own things (product, place, people, material, community)
- [ ] Composition decision: does the picture lead the screen, sit beside the text, or is the hero type-led with a small accent
- [ ] Where text sits: the calm area of the plate, or outside it
- [ ] Sizes: desktop 16:9 or 21:9, and how it crops on a phone (a portrait version or center-safe composition)
- [ ] People: none, generated (not presented as the user's team), or Soul ID from consented photos

## Think

1. Subject sentence first (`taste.md` §1). A hero that shows atmosphere but nothing of the subject fails.
2. Choose the hero's scale: picture-led (media covers most of the first screen), balanced, or type-led (a statement with a small visual or none). Decide; don't split the difference.
3. Choose the composition from what leads the content: text docked bottom-left over the image, centered low, image as the whole canvas with a calm area, split, off-grid. Do not reach for left-text/right-image by reflex.
4. Hold the hero to four text elements at most (headline, one line, action, and optionally one small label) and two lines of headline on desktop. These are set in HTML.
5. If the brand has no strong imagery, consider type and color alone; it is a legitimate hero.

## Make

1. **Comps first (optional in Light mode):** three full-screen comps of the hero with the real headline and navigation, differing in what leads. Pick one with the user. These are references only.
2. **Plate:** a photographer's brief, not a mood: subject, camera angle and lens feel, light direction and hardness, background, the calm area for text ("negative space in the left third"), aspect ratio, palette hex, and "no text, no logos, no watermark". Generate two candidates at the cheap setting, then the keeper at full quality and at about twice display width.
3. **Match the rest to it:** every later plate (section images, OG image, the scroll film's storyboard) uses the hero as the reference for light and palette.
4. **Interaction pair (optional):** if the page reveals the hero (dark to lit, desaturated to color), generate the base first, then a re-grade of the same composition with the base as reference, so they align.

Higgsfield routes: GPT Image 2.5 or Nano Banana for art-directed plates; Product Photoshoot `hero_banner` when the hero is a product (give it the product photo and intent; its backend writes the prompt); Soul or Seedream for people; Layers to split a finished plate into editable layers for parallax; Relight or Color Palette to grade a plate to brand hex. Check current names in `../higgsfield-notes.md`.

## Keeper checks (examples, write your own three)

- The subject is identifiable at phone size
- The calm area holds the headline at 4.5:1 contrast without a scrim covering the picture
- Light and palette match the brand tokens; no tell from the dated list

## Typical spend

Comps and plate candidates are stills: cheap. A 2K hero image cost about 8 credits in Higgsfield's August 2026 example. Budget three to six stills before the keeper; stop and change the brief, not the wording, if two rounds miss.
