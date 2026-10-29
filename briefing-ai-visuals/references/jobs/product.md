# Job: product imagery (studio, lifestyle, banner, ads, carousel)

The product must stay the product: shape, color, label and proportions exactly right. That is why the real product photo is the most important input, and why fidelity is checked before style.

## Ready check

- [ ] At least one clean photo of the real product (several angles if it must turn or be shown from the side). Without one, a written spec: category, shape, material, colors, packaging, label text
- [ ] Where the images will live: shop page, website hero, Pinterest, paid social, marketplace listing; that sets aspect ratio and rules
- [ ] How many, and whether they must work as a coordinated set (carousel, ad pack)
- [ ] The angle or hook per image, decided before generating
- [ ] Brand colors and any existing campaign imagery
- [ ] People: none, hands only, a generated model (not presented as a real customer), or Soul ID from consented photos
- [ ] Text that must appear, quoted exactly; or none, with copy set in layout afterwards
- [ ] Marketplace rules if any (white background, no badges on the main image)

## Think

1. **Fidelity first.** Start from the real photo or product page, not a prompt alone; the shape, color and packaging are already correct there.
2. **Pick the mode by intent:** clean studio, lifestyle scene, close-up with hands, Pinterest pin, wide hero banner, carousel, ad pack, try-on, conceptual (levitating, splash, sculptural), restyle of an existing shot.
3. **Give each reference one job** and say it in the prompt: product reference for the product only, location reference for the place, character reference for identity and not for lighting.
4. **For a set, vary on purpose:** format, hook, setting and mood; a slight variation of the same shot is not a second ad. Keep one palette and one light logic across the set.
5. **Honesty:** a lifestyle scene must not imply a real shop, customer or review.

## Make

1. Two or three candidates at the cheap setting from the product photo; check the product against the photo before judging style.
2. Re-roll only the layer that failed (product drifted: stronger product reference; light wrong: one lighting line; scene wrong: the setting).
3. Keepers at full quality. For a website, regenerate the chosen image at about twice display width with a calm area for text if it is a banner.
4. Animate only keepers (`video.md`): short image-to-video from the approved still.

Higgsfield routes: Product Photoshoot (ten modes, among them `product_shot`, `lifestyle_scene`, `hero_banner`, `social_carousel`, `ad_creative_pack`, `conceptual_product`, `restyle`; its backend writes the prompt, so give it the photo and a short intent, not a hand-written prompt; `--count` for coordinated variants). Marketplace Cards for listing images. Ads Studio turns a website link into a batch of static ads. Marketing Studio for UGC-style or TV-spot video ads from a product URL. Check `../higgsfield-notes.md`.

## Keeper checks (examples)

- Shape, color, label and proportions match the real product photo
- The product is the first thing the eye lands on
- Text that must appear is spelled exactly; nothing else is written in the image

## Typical spend

Stills are cheap (a 2K image about 8 credits in Higgsfield's August 2026 example); one multi-variant call for a set is cheaper than many single runs. Video ads: a 15 s 720p piece was 89 credits in Marketing Studio in the same example. Test hooks on stills before paying for video.
