# THUMBNAIL SPEC v2 — Google Maps Lead Agent
Rebuilt against Kallaway's thumbnail playbook. Supersedes the thumbnail section of
`PACKAGING_zero-touch-pipeline.md`.

Channel state: 47 views/video · CTR 1.11% · **Dhruvesh is an unknown face on YouTube.**
That single fact changes most of the design decisions below.

---

## WHAT v1 GOT WRONG

| v1 said | Kallaway says | Correction |
|---|---|---|
| Big face, front and center | *"If nobody knows you this could backfire… often it's better not to use a face than to use one that's pretty unknown."* | Face becomes a **testable variable**, not a default. Ship a no-face variant. |
| Dark navy background | Contrast **against the category**, not just within the frame. He went light because competitors went dark. | Every AI/automation thumbnail is a dark terminal. **Go light.** This is the single biggest available edge. |
| Text = `ZERO-TOUCH` | Text should name the **silent feeling**, not describe the mechanism ("basically cheating," "alone"). | Mechanism descriptors are weaker than felt states. Revised options below. |
| "No drop shadows" | *"If you're struggling to create separation between your face and the background, use shadows."* | Ban decorative glow. **Keep shading for subject separation.** |
| One thumbnail | *"You should be testing with at least three."* Bartlett tests 100. | Ship **3 variants**, one hypothesis each. |
| Amber accent | Green = good, red = bad. Other colors carry no baked-in comprehension. | Use **green/red to encode the before→after**, amber only as neutral contrast. |

---

## THE PSYCHOLOGY FLOW — gut-check all three

1. **Visual stun gun** — does it stop the scroll? (light background in a dark category)
2. **Title value hunting** — does the title trigger the desire loop? (more customers, less chasing)
3. **Visual validation** — do the thumbnail elements *support the title promise* without repeating it?

Failure modes: easy to read but doesn't pop → dies at 1. Pops but weak title → dies at 2.
Strong title but elements don't back it → dies at 3 (confusion).

**Current video dies at step 1.** Dark thumbnail in a dark category, no visual pop.

---

## DESIRE LOOP (define before designing)

- **Core desire (owner):** more customers, less chasing.
- **Pain point:** "I'm paying for lead lists / doing prospecting manually / my pipeline is empty."
- **Solution:** a system that finds and contacts them without me.
- **Curiosity loop:** *"If I click this, will I stop having to chase customers?"*

---

## TEXT ON THE THUMBNAIL — must not repeat the title

Title already carries: the number, Google Maps, and "without opening it."
Thumbnail text must add a **felt state**, a **pain trigger**, or **proof**.

| Option | Type | Notes |
|---|---|---|
| `WHILE I SLEPT` | felt state | Adds a time dimension the title doesn't have. **Only if true.** |
| `STOPPED BUYING LEADS` | pain trigger | Strongest owner language. |
| `$0` | proof / big number | Stun-gun category 4. Very high pop. |
| `ZERO-TOUCH` | mechanism | Keep as the term brand in the video, weaker on the image. |
| ~~`NEVER OPENED IT`~~ | ❌ | Redundant with the title. Cut. |

⚠️ **Conflict flagged:** the account's One Degree Rule says never name money directly. Kallaway's
stun-gun list explicitly recommends big dollar figures. On YouTube for an owner avatar, `$0` is
justified — but it breaks the standing rule. Decide deliberately.

---

## THE THREE VARIANTS TO TEST

Three elements maximum in every one. Bottom-right 130 × 45 px stays empty (duration stamp).
1280 × 720, PNG, under 2 MB.

### Variant A — light · no face · before/after  ← highest CTR bet
**Hypothesis:** an unknown face is costing more than it earns; category contrast wins the stun gun.

- **Background:** warm off-white `#F5F1E8`. Pops against every dark AI thumbnail in the feed.
- **Composition:** A/B split (transformation), arrow between the halves.
- **Left panel:** a lead-tool invoice or a hand-built spreadsheet, desaturated, **red** `#E24B4A`
  cross or tint. This is the anti-transformation — reminds them of the pain.
- **Right panel:** real dashboard rows, **green** `#1D9E75` SENT column. The end state.
- **Text:** `$0` — enormous, bottom-left or center. Or `STOPPED BUYING LEADS` if you'd rather
  hold the One Degree Rule.
- **Elements: 3** (pain graphic, result graphic, big text).

### Variant B — light · face · asymmetric  ← trust/booking bet
**Hypothesis:** for a consulting funnel, the face is worth the CTR cost.

- **Background:** same off-white `#F5F1E8`.
- **Composition:** rule of thirds — you on the **right third**, dashboard filling the left two-thirds.
- **Your expression: relief / quiet satisfaction.** Not shock. The emotion must match what the
  viewer will feel if the promise is delivered, and an owner wants *relief*, not amazement.
  Shock faces read as tutorial content and re-sort you back to the builder audience.
- **Separation:** soft drop shadow behind you against the light background. Required here.
- **Text:** `WHILE I SLEPT`, upper-left over the dashboard.
- **Elements: 3** (face, dashboard graphic, text).

### Variant C — dark · face · term brand  ← control
The v1 design, kept only as the baseline to measure A and B against. Expect it to lose the
stun-gun step. If it wins, the category-contrast theory was wrong for your niche and you should
know that.

---

## HARD RULES (all variants)

- **No terminal, code editor, or VS Code chrome anywhere in frame.** One glimpse re-sorts the audience.
- Three elements maximum. No arrows *and* circles *and* badges — pick.
- Green means good, red means bad. Don't use them decoratively.
- Every graphic must be a **real screenshot**. Mockups trigger the bait-and-switch spook.
- Nothing important in the bottom-right corner.
- Upscale grainy assets (magnific.ai) rather than shipping soft imagery.
- Text large enough to read at **1/16 of an iPhone screen**. If in doubt, make it bigger and
  delete something else.

---

## PROCESS FIXES

**Do the thumbnail first, not last.** The order is: idea → title → thumbnail concept → *then* film.
Currently this is being done in reverse, which is why the packaging is weaker than the content.

**One photo session, permanently.** Record 4K/60 video for 5–10 minutes cycling through:
happy · relieved · satisfied · surprised · shocked · pointing up-left · up-right · down-left ·
down-right · open palms · arms crossed · hands off keyboard. Pull stills forever after. This is
the highest-leverage 10 minutes available and removes the recurring bottleneck.

**Build a swipe file.** One folder. Screenshot any thumbnail that stops your scroll. Hand it to
a designer later.

**Testing stack:**
- `clickpilot.app` — preview in a simulated feed against real competitor channels
- YouTube native A/B/C test — run all three variants
- `thumbnailtest.com` — if you want title × thumbnail combinations

**Outsource when affordable.** Kallaway's position: hire a thumbnail designer as early as you
possibly can. Until then, Variant A is the one that needs the least design skill — it's two
screenshots and a number.

---

## ✅ LOCKED — VARIANT B (production spec)

Selected by Dhruvesh. Light background, face retained, asymmetric composition.
Rationale: keeps the category-contrast win (light frame in a dark niche) while retaining the
face, which is the trust asset that converts a viewer into a booked call. Accepts a small CTR
cost in exchange for funnel quality.

### Canvas
1280 × 720 px · PNG · under 2 MB · sRGB

### Grid (coordinates at 1280 × 720)

| Zone | Position | Contents |
|---|---|---|
| Background | full bleed | flat `#F5F1E8` — no gradient, no texture |
| Dashboard panel | x 40 → 830, y 90 → 640 | real screenshot, white card, 1px `#D3D1C7` border, 12px radius |
| Subject | x 830 → 1280 | Dhruvesh, chest-up, right third |
| Text block | x 70 → 500, y 60 → 210 | `WHILE I SLEPT`, two lines |
| Keep-clear | x 1150 → 1280, y 675 → 720 | YouTube duration stamp — nothing here |

### The dashboard screenshot
- Real capture. Never a mockup.
- 5–7 visible rows. Business names legible enough to read as *names*, not as texture.
- Right-hand status column showing green `SENT` — `#1D9E75`.
- Crop out all browser chrome, tabs, URL bar, and any localhost address.
- Boost saturation slightly so the green reads at small size.
- If the capture is soft, upscale with magnific.ai before placing.

### The subject
- **Crop:** chest-up, head occupying roughly the top 45% of the right third.
- **Body angle:** ~15° toward frame centre. Eyes to camera.
- **Pose:** arms crossed, or one open palm gesturing toward the dashboard. Relaxed shoulders.
- **Expression: relief / quiet satisfaction.** A small closed-mouth smile. **Not shock, not
  surprise, no open mouth.** The face must carry the emotion the viewer will feel if the promise
  lands — an owner wants relief, not amazement. Shock faces read as tutorial content and undo the
  owner positioning.
- **Wardrobe:** solid mid-to-dark shirt — navy, charcoal, forest. No logos, no patterns, nothing
  cream or white (disappears into the background).
- **Lighting:** soft key camera-left ~45°, warm. Quarter-power fill camera-right.
- **Separation:** cut out cleanly, then add a soft drop shadow — `0 4px 18px rgba(0,0,0,0.18)`.
  Required on a light background. This is separation, not decoration.

### The text
- **Copy:** `WHILE I SLEPT` — two lines, break after `WHILE`.
- **Case:** all caps.
- **Font:** Inter Black or Montserrat ExtraBold. Geometric sans only.
- **Cap height:** ≥ 95 px per line.
- **Tracking:** −2%. **Leading:** 0.92.
- **Colour:** `#2C2C2A` near-black. High contrast on cream, no colour competition with the green.
- **No stroke, no glow, no outline.** If contrast fails, lighten the area behind it instead.

⚠️ **Truth check:** only use this line if the sequence has genuinely run overnight.
Backup copy, in order of preference: `STOPPED BUYING LEADS` · `I NEVER LOOKED` · `$0 SPENT`.

### Palette
| Use | Hex |
|---|---|
| Background | `#F5F1E8` |
| Card | `#FFFFFF` |
| Card border / neutral rows | `#D3D1C7` |
| Success / SENT | `#1D9E75` |
| Text | `#2C2C2A` |

Green is reserved for "good." Do not use red anywhere in this variant — there is no
before/after here and red without a negative referent just adds noise.

### Element count: 3
Face · dashboard graphic · text. Nothing else. No arrows, no circles, no badges, no logos,
no Claude or Google Maps branding.

### Pre-export checklist
- [ ] Shrink to 168 × 94. Is the text readable? Is the expression legible? Is the green visible?
- [ ] Preview in `clickpilot.app` against real competitor channels in the niche.
- [ ] Bottom-right 130 × 45 confirmed empty.
- [ ] No terminal, code editor, or VS Code chrome anywhere in frame.
- [ ] Dashboard is a real screenshot, and the number on screen matches the number in the title.
- [ ] Under 2 MB.

### Still run the test
Ship **B as primary** and **A as the challenger** in YouTube's A/B/C tool. The test is free and
it answers the open question — whether an unknown face helps or hurts on this channel. That
answer is worth more than this one video.

---

## ON CLICKBAIT

Baiting the click is the job. It only becomes clickbait when the content doesn't match the
promise. Your content over-delivers on the promise, so lean in harder than you currently are —
"How to Scrape Unlimited Leads" is under-baited *and* vague, the worst combination.
