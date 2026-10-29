# Taste: how to think before generating

Distilled from Impeccable (Paul Bakaus), Taste Skill and imagegen-skills (Leonxlnx), Emil Kowalski's skills and Higgsfield's own skills. Rewritten here as working rules; see `sources.md` for what came from where. Use it at Stop 3 for every job, and for reviewing results.

## Contents
1. Subject before style
2. The surface's mode
3. Comp, plate or code
4. One dominant move
5. The default check (dated tells)
6. Real content, honest proof
7. Pictures on web pages
8. Text over pictures
9. Where the sources disagree, and our call
10. Review questions

## 1. Subject before style

A look picked from a mood list is a default with a new name. Start from the subject:

- List what only this project has: the product's own objects and materials, the place, the people, the data, the history, the words the community uses. Five to ten items.
- Write one sentence tying that material to a direction ("the pixel crayfish and the Discord wall of builds, set as a Swedish print workshop: flat ink fields, one red"). That sentence is the idea; every prompt carries it.
- Removing every AI tell and putting nothing in its place gives an empty page with good manners, which is a tell too. Fill the gap with the subject first, then check.
- The brief wins. Pinned colors, fonts, eras and brand tokens are honored even when they appear on a tells list. A brand's own palette is not a default.

## 2. The surface's mode

Name what the visitor's success looks like, from the surface, not the company:

| Mode | Surfaces | What the visuals may do |
|---|---|---|
| Persuade | landing pages, campaigns, pricing, launch posts | Full commitment: one memorable visual move, real imagery, a visible action |
| Experience | portfolios, showcases, galleries | The work leads from the first screen; the interface recedes |
| Read | docs, articles, guides, changelogs | Structure first; imagery explains, never decorates |
| Operate | app screens, dashboards, tools, settings | Restraint: familiar patterns, scannable, brand only in details; no hero art inside the tool |

A tool's landing page is still Persuade. A docs index is still Read. When the user asks for "hero art" on an Operate surface, say so and offer it for the landing page instead.

## 3. Comp, plate or code

Decide per region what the pixels are before prompting. This is the step that most often decides whether an AI-made site looks expensive or blurry.

- **Comp:** a generated picture of the whole screen or section, with real headline and content, used only to choose a direction. Generate three that differ in structure (what leads, density, focal point), not three tidier copies of one. A comp is a reference, never a shipped asset.
- **Plate:** the raster the page actually ships: a photograph, a product, a material or texture, an illustration with shading or perspective. Regenerate it from the approved comp's crop at 1.5 to 2 times its display size, with no text and no UI chrome. Isolated objects on the page ground become transparent cutouts (check the alpha on light and dark grounds); full-frame imagery stays opaque.
- **Code:** all text, buttons, navigation, cards, diagrams with countable parts, flat shape systems, and anything that must move, scale or respond. Icons come from one library or one generated set, never mixed in one area.

A cropped comp shipped as an asset is how a beautiful comp becomes a blurry site. Text baked into a hero image cannot be translated, read by search, or fixed without a re-roll.

## 4. One dominant move

- At most three signature decisions, one of them bold. A look with ten loud features has none.
- Commitment is depth, not spread: one move carries the screen, the rest holds still in the same material. A second element competing at the same scale is the design shouting; keep the strongest, quiet the rest.
- One treatment for a whole set of pictures (untouched, greyscale, one grade). Mixed treatments read as a stock dump.
- One palette across every comp and plate: a ground, a text color, one accent used sparingly. Name it with hex values in every prompt.

## 5. The default check (dated tells)

A tell is a device that makes work read as generated. Most started as good ideas; they became tells by appearing everywhere without a reason. This list is dated because it moves: today's remedy is next quarter's tell. Checked 2026-10-29.

For each decision, ask: would I land here for any similar brief? If yes, it is a default. Use it only if the brief or brand asks.

**Palettes:** violet or indigo glow; near-black with one neon cyan, blue or green accent; graphite with orange or ember; cream or beige with terracotta, clay, brass or oxblood (the "make it warm and editorial" fix, now the most recognizable generated look); glossy teal and orange. Also: reusing the palette family of the previous job in the same session.

**Type and surface:** gradient headline text; glass panels everywhere; a soft grey shadow under every card; a serif display face as the shortcut to "premium"; one italic or colored word in a sans headline; monospace as a costume for "technical"; tiny tracked uppercase labels above headings; numbered section markers (01 / 02 / 03); hairline rules and outlined boxes as the whole structure.

**Layout:** centered headline, subtitle, two buttons, screenshot below; left text, right image as the reflex hero; three identical cards with an icon in a rounded square; a bento grid as the feature section; a headline of three or four lines; every section in the same layout family; everything centered.

**Pictures:** abstract blobs, orbs and swooshes; people smiling at laptops; a fake dashboard of grey bars and donut charts; isometric clip art; a poster where a page should be; one small picture floating with equal margins on all sides.

**Motion:** the same fade-and-rise on every block; staggered entrances on everything in the hero; hover lift on every card; bounce easing; loops that mean nothing.

**Copy:** unlock, supercharge, seamless, elevate, effortless, next-gen, revolutionize; "not just X, it's Y"; three-part slogans; invented logos, star rows and "10,000+ teams"; "Get started" and "Learn more" as the only labels.

## 6. Real content, honest proof

- Prompt comps with the real product name, the planned headline, real numbers with units and the next action by name. Placeholder copy gives placeholder layouts.
- Never invent claims, prices, testimonials or benchmarks the material does not carry. Generated imagery is a material, not evidence: a generated "customer", "team" or "office" must not be presented as real.
- A found or generated picture may show the world around the subject (its city, its materials, its kind of thing); it must not stand in for the user's own product, room, team or customers unless it is labeled.

## 7. Pictures on web pages

Measured on award sites (Taste Skill's study of Awwwards Sites of the Day, 2026), treat as starting values, not law:

- A picture leads its screen (60% or more of it) or stays small (under 10%). Screen after screen of half-size pictures reads as filler.
- Strong pages show more than they tell: on most top sites one piece of media covers at least half the first screen.
- Two aspect ratios for most pictures (for example 4:5 portraits, 16:9 or 3:2 landscapes); a third only on purpose.
- Square corners by default; if rounded, one radius everywhere.
- Serve at about twice the display width, capped near 2,400 px.
- Type and color alone is a legitimate design, not a gap: make the type the image, or use color at scale. Do not fill the gap with icons in squares or gradient blobs.

## 8. Text over pictures

- Put only display text on a picture: a headline, one short line and one action. Body text goes beside or below.
- Plan a calm area in the plate prompt (sky, a dark wall, the shadow side, negative space on one side) and dock text there.
- Contrast at the text's own position: 4.5:1 for body, 3:1 for large text. If it fails, move the text, add a solid card in the ground color, or a neutral scrim over the text area only.
- A fixed navigation over pictures needs a solid band.

## 9. Where the sources disagree, and our call

| Question | Positions | Our call |
|---|---|---|
| Duotone, color washes, gradients behind photos | imagegen-skills encourages palette-matched grades and duotone; Taste Skill v2 bans washes and duotone | A treatment is one of your three signature decisions. Choose one for the whole set, or none |
| Serif display faces | Higgsfield's website skill bans serif as a default; Taste Skill has no rule | Default check applies. A brand that already uses a serif keeps it |
| Hero composition | Higgsfield prefers split or asymmetric over centered; imagegen-skills calls left-text/right-image the most overused | Neither is the answer. Choose from what leads the content; avoid the reflex either way |
| Cost estimates | Higgsfield's own skills: don't pre-estimate unless asked, prefer quality | This skill exists to protect the budget: always set a ceiling and estimate when the tool can |
| Icons | Higgsfield generates a custom set; Impeccable and Taste prefer a real library | Library for dense UI; one generated set for a few large brand icons; never mixed |
| Interviewing | Higgsfield asks up to four labeled questions; Impeccable runs one or two rounds | At most three per round, each with options and a default |

## 10. Review questions

Run these on every comp and plate before accepting it:

- Point at the subject. A render that shows the atmosphere and nothing of the subject fails, however pretty.
- Name the mode from the image alone. If you cannot tell it is a landing page (or an app screen), it is art direction without a surface.
- Could it hang as a poster? Then it is not a comp. Could it pass as a stock photo? Then it is not a plate for this brand.
- Squint: is there one clear first thing to look at?
- Run the default check once more on the result, not only on the plan.
- Does it pass the three keeper checks written before generating?
