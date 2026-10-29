# Job: video with shots (teaser, ad film, recurring character or product)

Video is where credits disappear. Every shot inherits from a locked still and a locked layer, so the plan is mostly about what to decide before the first clip.

## Ready check

- [ ] The one thing the viewer should do or feel, and the channel with its format and length (9:16 short-form, 16:9 site, 1:1 feed)
- [ ] The approved hero frame or keyframes (stills first)
- [ ] Recurring people: Soul ID from the user's own or consented photos, or Elements from a generated image for invented characters; one Soul ID is one person
- [ ] Recurring products and places: Elements or a fixed reference with one job
- [ ] A shot list: one action and one camera move per shot, with duration
- [ ] Audio: native audio from the model, music made separately, voiceover, or silent with captions
- [ ] Captions or on-screen text: planned in the edit, not generated in the footage
- [ ] The cheap test setting for each model in use

## Think

1. **Layers:** identity (face, body, outfit), world (place, props, time of day), camera (move, lens, tempo, start and end framing), story (beat, cutoff). Change one layer at a time; mixed layers cannot be debugged.
2. **One shot, one action, one camera move.** Conflicting moves destabilize a shot. Name the move with the words in `../motion.md` §3.
3. **Start and end frames** carry direction better than words; if the prompt describes motion that cannot plausibly reach the end frame, the result drifts. Simplify the prompt and let the frames lead.
4. **Same words for the same things** in every prompt, no synonyms.
5. **Short-form structure:** hook early, short shots, one idea per shot.

## Make

1. Keyframes as stills until each passes its keeper checks.
2. Test each shot at the cheap setting from its locked frame.
3. Full quality only on keepers; extend or edit the keeper instead of regenerating the whole clip where the tool allows.
4. Edit, crop, grade and caption outside the generator before any re-roll.
5. Keep the failure log: symptom, layer, fix.

Higgsfield routes: Cinema Studio 4.0 (up to 30 s, up to 50 references, Director's Panel for camera, lens, color and light, forward and backward extend, edit one object or face); Seedance 2.5 as the default video model with a draft mode; Kling 4.0; Veo 3.1 and Gemini Omni for start and end frames; Genjutsu to swap a product or object in existing footage; Marketing Studio for ad formats; FLUX 3 Video Upscaler. Check `../higgsfield-notes.md`.

## Keeper checks (examples)

- The face (or product) holds across the shot
- Light matches the hero frame
- No morphing hands, objects or text

## Typical spend

Estimate shots x attempts x cost per attempt from the platform, with stills and test clips in separate lines. Max three attempts per shot; a shot that fails twice gets a different layer changed, not a third prompt tweak.
