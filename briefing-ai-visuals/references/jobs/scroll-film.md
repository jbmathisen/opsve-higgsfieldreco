# Job: a hero that moves (scroll film, ambient loop, animated hero)

The most expensive web job, and the one most often started too early. It inherits everything from an approved still, so it comes after `web-hero.md`, never instead of it. Read `../motion.md` first.

## Ready check

- [ ] An approved hero still or storyboard (the film inherits its quality; a weak still gives a weak film)
- [ ] The motion gate passed: what the motion is for, and that the surface is not Operate or Read
- [ ] Which type: scroll-driven film (scroll plays the footage), ambient loop (plays by itself, scroll does nothing) or a single animated element
- [ ] The journey: 3 to 6 chapters of copy mapped to moments of one film, each with one headline and one sentence
- [ ] Journey shape: single-shot (default) or multi-leg (only when the story truly travels between different worlds)
- [ ] Mobile: center-safe framing or a separate portrait source; lighter encodes
- [ ] Byte budget for all clips (start near 32 MB desktop, 16 MB mobile)
- [ ] Reduced-motion fallback: the same chapters over still posters
- [ ] Who builds the page (Higgsfield's website skill, the user's own stack, or a developer), since the footage rules depend on how it is played

## Think

1. **Single-shot first.** One continuous take of about 15 seconds, scrubbed end to end, has no seams to fail. "It would look cooler with more scenes" is not a reason for multi-leg; each leg costs a generation, a sequential wait and a seam check.
2. **Direct it like a product film:** one hero subject, one continuous move (slow orbit, push-in, rise, fly-through, assembly), dark low-detail background, locked exposure, start state different from end state. All rules are in `../motion.md` §4.
3. **Chapters are HTML over the film,** in the calm space the film leaves. Never put text in the footage.

## Make

1. **Storyboard:** one 16:9 image showing six keyframes of one continuous move in a grid, with "one continuous move, not six different scenes" and no text. It pins palette, lens and camera progression for the price of a still. Show it to the user; budget two re-rolls.
2. **Test clip:** the move at the cheap setting (draft or lowest resolution, shortest length that shows the move). Check the keeper tests on the test, not on the final.
3. **Final film:** the longest single take the model supports, highest resolution needed, audio off. Pass the storyboard as a style reference, not as the start frame.
4. **Multi-leg only:** each leg starts from the previous leg's actual last rendered frame (extract it, upload it as the start frame); never from an imagined destination still. Check each leg's last frame before paying for the next. Use one model and one grade for the whole chain.
5. **Encode for scrubbing:** H.264, short keyframe interval (about 8 frames desktop, 4 mobile), audio removed, fast start; a poster from the first frame of each final clip. Higgsfield's website skill ships a ready helper for this (`higgsfield-websites/references/scroll-scrub*.md`).

Higgsfield routes: Seedance 2.5 is Higgsfield's default video model (4 to 30 s, up to 1080p, a draft mode for cheap previews); Kling 3.0, Veo 3.1 and Gemini Omni support start and end frames (check Kling 4.0 in its schema); Cinema Studio 4.0 for directed shots up to 30 s. Higgsfield's website skill builds an animated scroll site by default and asks animated or not first. Check `../higgsfield-notes.md`.

## Keeper checks (examples)

- No cut, shake, exposure pumping or flicker anywhere in the take
- Every paused frame works as a still behind the chapter copy
- The subject stays center-safe in a 9:16 crop

## Typical spend

From Higgsfield's pricing post (2026-10-20), an 8 s Seedance 2.5 clip cost 24 credits at 480p, 56 at 720p and 128 at 1080p; a 30 s clip about 195 credits (August example). Draft at 480p until the move is right, then render the keeper once. Stop after two failed tests and change the move, not the wording.
