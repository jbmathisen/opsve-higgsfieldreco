# Templates

## Contents
- 5-line brief (Light mode)
- Project dossier
- Full brief
- Direction card
- Layers
- Prompt skeletons: comp, plate, section board, storyboard, video shot, compact
- Asset or shot entry
- Spend plan
- Agent instruction
- First-hour plan
- Failure log
- Debrief

## 5-line brief (Light mode)

```
Goal / audience / single message: one line
Starting asset: path or description of what already exists
Deliverable: format, size or length, channel, count
Must / must not appear:
Keeper test: three yes/no checks
```

## Project dossier

```
Project: what it is, in one sentence
For: who it is for, and the surface's mode
Only this project has: 5-10 items (objects, place, people, material, data, words)
Assets: path - what it is (one per line)
Brand tokens: palette hex, typefaces, logo (source)
Missing / unknown:
Assumptions made:
```

## Full brief

```
# Brief: [working title]
Line: goal / audience / single message
Surface and mode: e.g. landing page, Persuade
Objective: one outcome, measurable if possible
Audience: described by what they believe or want, not by age
Reasons to believe: 2-3 facts that trace to the material
Real content: headline, supporting line, the action, key numbers
Deliverable: format, aspect ratio, duration, count
Tone: three words, each backed by an observable behavior
Mandatories: must appear / must not appear / legal / platform limits
Source material used:
Assumptions:
```

## Direction card

```
Idea: one sentence tying the subject to the direction
Palette: ground, text, one accent, 1-3 supporting (hex)
Light: direction, hardness, time of day
Camera and lens feel:
Texture or medium:
Picture treatment: untouched / greyscale / one grade (one for the whole set)
Motion: the one authored moment, or none
Type (set in code): faces and roles
Pixels: which regions are plates, which are code
The one bold decision:
Signature decisions (max 3):
Not this: 3-5 items
References: file - the one job it has
```

## Layers

Generate one layer at a time. Mixed layers cannot be debugged.

| Layer | Holds | Locked by |
|---|---|---|
| Identity | face, body, outfit | Soul ID or Elements, character sheet |
| World | place, props, time of day | hero frame, location reference |
| Camera | move, lens, tempo, start/end framing | camera line in prompt, start and end frame |
| Story | beat, cutoff | shot list |

## Prompt skeletons

**Comp (a whole screen, to choose direction; 150-300 words):**
```
[Kind of screen] for [product name], rendered edge to edge with crisp readable text,
no browser window, device or desk around it.
The visitor [job in plain words]. Content: [real headline], [supporting line],
[real numbers with units], [the next action by name].
This comp leads with [what leads: the product / the offer / a statement / the work].
Parts in reading order: [phrase each].
Frame: [mark and name], [navigation], [utility controls].
Look: [the reference image carries palette, type and components; do not copy its content]
  OR [2-4 sentences of concrete visual law: ground and main colors with what each does,
  the type voices, the one signature].
```
Leave sizes, positions and component styling out unless the user pinned them.

**Plate (a raster the page ships; a photographer's brief):**
```
[Subject, named in the project's own words], [angle and lens feel], [light direction and hardness],
[background], calm area for text: [where], aspect [ratio], palette [hex],
[treatment]. No text, no logos, no watermark.
```
Generate the hero plate first; later plates name it as the reference for light and palette.

**Section board (website design reference, one per section):**
```
Website design reference, desktop, [section role], [theme + exact palette],
[type character] typography, composition anchor: [anchor], background: [mode],
motif: [narrative spine], real copy: "[headline]", clear hierarchy and spacing,
no watermark, no browser chrome.
```

**Storyboard (for a scroll film):**
```
One 16:9 image, a 6-panel grid showing six keyframes of ONE continuous camera move,
not six different scenes: [subject], [move], [background], [palette hex], [light].
No text anywhere in the image.
```

**Video shot:** cinematography + subject + action + context + style and ambiance + audio. One camera move per shot.
```
[shot size and move, speed] [subject] [one action]. Context: [place, time]. Light: [...].
Grade: [hex or named]. Locked exposure, no cuts, no shake. [duration], [aspect]. Audio: [...]
```

**Compact:**
`[shot] subject + action. light: ... lens feel: ... color: ... ref: only X. keep Y unchanged. 4s, calm camera.`

## Asset or shot entry

```
N. [name] (size or duration):
Kind: comp / plate / code / clip
Locked layers:
Open variables:
Prompt:
Not this:
Keeper test: yes/no x3
```

## Spend plan

```
Balance: __ credits (read on __)
Phase      Items x attempts x cost each   = credits
Stills     __ x __ x __                   = __
Tests      __ x __ x __ (cheap setting)   = __
Finals     __ x 1 x __                    = __
Total: __ (__% of balance). Stop at: __
Cost per attempt from: platform estimate / price page / blog example (date)
```

## Agent instruction

```
Check my Higgsfield credit balance first and tell me.
Budget for this task: N credits. Estimate the cost of each generation before running it
(on the CLI: higgsfield generate cost ...) and tell me.
Max 3 attempts per asset or shot. Ask me before every generation.
Stop and ask when 80% of the budget is spent or when an asset fails twice.
Use the cheap test setting (draft or lower resolution, shorter clip) until I approve.
Upload reference files explicitly before generating and confirm each upload.
Never put text, logos or watermarks in images unless I quote the text here.
If you use Higgsfield's own skills, follow this budget even though they default to quality.
```

## First-hour plan

```
Phase 1, stills or comps only. Budget: __. Done when: hero or direction approved.
Phase 2, locks (character, product, place). Budget: __. Done when: keeper test passes on a still.
Phase 3, short test clips from locked frames, cheap setting. Budget: __. Done when: the move is right.
Phase 4, full quality on keepers only. Budget: __.
Outside the generator: edit, crop and grade before any re-roll.
```

## Failure log

```
Symptom -> layer -> fix
```
Same error twice: change layer, not more prompt.

## Debrief (after a one-shot or a session)

```
Worked:
Drifted:
Change next time (which layer):
```
