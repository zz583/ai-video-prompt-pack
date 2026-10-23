# AI Short-Video Prompt Pack Vol.1
## Segmented Generation + Character Consistency + Style Replication — a production-verified method with 36 templates

> Nothing here is scraped from prompt lists. Every rule comes from shipped work: a 14s original-character PV, two 25.2s character PVs, a 35s photorealistic slice-of-life film, a Y2K DV day-in-the-life, and film-look replication tests. Each template notes the tool, aspect ratio, duration and segmentation it was verified with. Replace the [brackets] with your content and generate.

---

## Part 1 — Core Methodology (read this first)

### Method 1: Segmented generation (the only stable way to go long)
- Models stay stable for ~5–10s per generation. For a 15–35s film, **cut on narrative beats**, generate each segment independently, and stitch in your editor.
- Golden cuts: 15s = 2 segments; 25s = 3 segments (8.4s × 3); 35s = 5 segments (merge 1–2 shots per segment).
- Segments connect through "the same character lock block + the same lighting description" — never through tail-frame chaining (see Method 4).

### Method 2: The Character Lock Block (the root of consistency)
Write your character ONCE as a fixed block and paste it **verbatim, word for word**, into every segment prompt:
```
[Lock block example] The same girl: long mint-green hair in loop-shaped side buns with thin braids, amber-gold eyes with star-shaped highlights, white-and-navy off-shoulder sailor top, blue-cyan chest bow with a golden star, star-pattern pleated skirt, a large blue bow on her back, one long dark-blue tail tipped with a blue heart.
```
Cover everything: hair color/style · eyes · top · bottom · signature accessories · special traits. Miss one item, that item drifts.

### Method 3: Style replication — image-to-video beats text (learned the hard way)
- Writing "in the style of X" only ever gets you an approximation.
- The working method: take 1–2 real stills of the target look as reference images, use **image-to-video**, and let the prompt describe only action and camera movement.
- The smaller the motion (micro-movement, slow push-in), the better the look survives.

### Method 4: Independent generation + reference anchor > tail-frame chaining
- Chaining from the previous segment's last frame looks seamless but drifts the worst in practice (faces and outfits quietly mutate).
- Instead: generate every segment independently from the **same character sheet** as reference, unified by the lock block.

### Method 5: Negative-constraint list (attach to every segment)
```
no subtitles, no text, no watermark, no logos, no close-ups of brand trademarks, normal hands (five fingers), no distorted face, no face change
```
With real branded props, add: `do not emphasize brand marks, no trademark close-up shots`.

### Method 6: Pre-delivery frame check
Same face? / Hair and accessories complete? / Outfit colors unswapped? / Prop states continuous (a bottle cap may only be open AFTER the segment where it opens)? / No stray generated text? If a segment fails, re-run that segment alone — never the whole film.

---


---

## Get the full pack
Part 2 (36 templates) + Part 3 (parameter cheat sheet) are in the full edition:
👉 https://zzstudio.itch.io/ai-video-prompt-pack-vol1 — $4.99, one-time, free Vol.1 updates.
