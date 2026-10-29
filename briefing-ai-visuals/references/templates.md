# Templates

## Contents
- 5-line brief (Light mode)
- Project dossier
- Full brief
- Art direction card
- Layers
- Prompt skeleton
- Shot entry
- Agent instruction
- First-hour plan
- Failure log

## 5-line brief (Light mode)

```
Goal / audience / single message: one line
Starting asset: path or description of what already exists
Deliverable: one file, one length, one channel
Must / must not appear:
Keeper test: three yes/no checks
```

## Project dossier

```
Project: what it is, in one sentence
For: who it is for
Assets: path - what it is (one per line)
Brand constraints:
Missing / unknown:
Assumptions made:
```

## Full brief

```
# Brief: [working title]
Line: goal / audience / single message
Objective: one outcome, measurable if possible
Audience: described by what they believe or want, not by age
Reasons to believe: 2-3 facts that trace to the material
Deliverable: format, aspect ratio, duration, count (one file, one length, one channel)
Tone: three words, each backed by an observable behavior
Mandatories: must appear / must not appear / legal / platform limits
Source material used:
Assumptions:
```

## Art direction card

```
Palette: 4-6 named hex values
Light: direction, hardness, time of day
Camera and lens feel:
Texture or medium:
Motion:
Type (if any): font style, text quoted exactly
The one bold decision:
Not this: 3-5 items
References: file - the one job it has
```

## Layers

Generate one layer at a time. Mixed layers cannot be debugged.

| Layer | Holds | Locked by |
|---|---|---|
| Identity | face, body, outfit | Soul ID or Element, character sheet |
| World | place, props, time of day | hero frame, location reference |
| Camera | move, lens, tempo, start/end framing | camera line in prompt, start and end frame |
| Story | beat, cutoff | shot list |

## Prompt skeleton

Image: subject, composition, action, location, style. Quote any text and name the font style. Add what must not happen.

Video: cinematography + subject + action + context + style and ambiance + audio. One camera movement per shot.

Compact form:
`[shot] subject + action. light: ... lens feel: ... color: ... ref: only X. keep Y unchanged. 4s, calm camera.`

## Shot entry

```
Shot N (duration):
Locked layers:
Open variables:
Prompt:
Not this:
Keeper test: yes/no x3
```

## Agent instruction

```
Check my Higgsfield credit balance first and tell me.
Budget for this task: N credits.
Max 3 attempts per shot. Ask me before every generation and say what it should cost if you can see it.
Stop and ask when 80% of the budget is spent or when a shot fails twice.
Upload reference files explicitly before generating and confirm each upload.
Use the lower test setting until I approve a shot.
```

## First-hour plan

```
Phase 1, stills only. Budget: __ credits. Done when: hero frame approved.
Phase 2, character or location locks. Budget: __. Done when: keeper test passes on a still.
Phase 3, short test clips from locked frames, lower setting. Budget: __. Done when: motion path is right.
Phase 4, full quality on keepers only. Budget: __.
Outside the generator: edit, crop and grade before any re-roll.
```

## Failure log

```
Symptom -> layer -> fix
```
Same error twice: change layer, not more prompt.
