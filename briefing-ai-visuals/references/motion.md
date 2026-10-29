# Motion: when things move

For every job where something moves: an animated hero, a scroll film, UI motion around generated assets, or video shots. Built on Emil Kowalski's animation rules (restraint first), Higgsfield's scroll-scrub footage rules and Impeccable's "one authored moment".

## Contents
1. The motion gate
2. Budgets
3. Words that get the right motion (camera and UI)
4. Footage that survives scrolling
5. Reduced motion and weight

## 1. The motion gate

Every moving thing passes four questions, in order. Most candidates should fail; a short list of motion with conviction beats motion everywhere.

1. **How often is it seen?** Many times a day (navigation, shortcuts, tools): no motion. Tens of times: barely any. Occasionally (a landing page visit, a modal): standard motion. Once (first visit, launch, celebration): this is where the spectacle budget lives.
2. **What is it for?** Name one: explanation (shows how the product works), spatial continuity (where something came from or went), state (a change becomes legible), feedback (the interface heard you), or delight on a rare moment. "It looks cool" is not on the list.
3. **Can it stay in budget?** Time and bytes, see below.
4. **Does it help the task?** Content people read or act on must not move for style. A moving hero on a docs page or inside a dashboard fails.

On a Persuade page: one authored moment per page (the hero film, or one reveal), not the same entrance on every section.

## 2. Budgets

- UI responses: 100 to 300 ms, ease-out for things entering, never ease-in. Marketing and explanatory motion may run longer.
- Scroll film: about 15 seconds of footage for a whole page journey in one take; plan an aggregate byte budget (start near 32 MB desktop, 16 MB mobile for all clips) and shorten or re-encode before relaxing it.
- Ambient loop: 5 to 15 seconds, muted, with a poster frame, paused out of view; hero source around 1920x1080 under 10 MB.
- Video shots for short-form ads and teasers: short shots and the hook in the first seconds. Working rule from opensverige's own film pipeline, not measured: 1.2 to 3.5 seconds per shot, hook inside 2.5 seconds.

## 3. Words that get the right motion

Vague words give the model room to improvise. Name the move.

**Camera (video prompts, one per shot):** static / locked-off; slow push-in (toward the subject); pull-back (reveal); orbit (around the subject); crane or rise; lateral track or dolly; pan (turn left or right in place); tilt (up or down in place); rack focus (soft to sharp); handheld (only when the brief wants it). Add speed ("slow, constant speed") and what holds still ("locked exposure, no cuts, no shake").

**Subject motion:** turn toward camera; assemble (parts come together); exploded view; emerge from darkness; light sweep across the surface; transformation from state A to state B.

**UI motion (for the page around the assets):** fade, slide, scale-in (never from zero), reveal by clip or mask, stagger (30 to 80 ms between items), crossfade, shared element transition, layout animation, scroll-driven animation, parallax, view transition, press feedback, spring (subtle bounce 0.1 to 0.3, only for drag and playful moments). Say which one you mean, and its duration and easing.

## 4. Footage that survives scrolling

When a page scrubs a film with the scroll, every frame is shown as a still, forwards and backwards. That sets the footage rules:

- One continuous move, no cuts. A cut becomes a jump mid-scroll.
- One hero subject, kept center-safe (the video is cropped on phones), with clean negative space where the copy sits.
- A background the copy can survive: dark, seamless, low-detail. A bright busy environment behind text is the most common reason a beautiful film is unusable.
- Slow, steady speed; ease only at the very start and end. The scroll supplies the pacing.
- Locked exposure and white balance, no flicker, minimal motion blur.
- Start state differs from end state, or the scrub has no payoff.
- No text, logos or watermarks in the footage; all type is HTML over it.
- Pass the storyboard as a style reference, not as the start frame, or the page opens on a static board for a second.

Subjects that scrub well: a product slowly orbiting on black; an exploded-view assembly; a macro detail travelling along a surface; a transformation; an object emerging from darkness.

Frame-sequence scroll animations (hundreds of stills) can feel slightly laggy; direct MP4 scrubbing with short keyframe intervals is the alternative (see `jobs/scroll-film.md`).

## 5. Reduced motion and weight

- Every moving element has a still fallback: under reduced-motion settings, show the poster or final frame and fetch no video.
- Mobile gets lighter encodes and the same story.
- If motion cannot be finished properly in scope, ship a clean still page instead of half-wired motion.
