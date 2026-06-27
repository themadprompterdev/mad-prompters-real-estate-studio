# How to Use — Mad Prompters Real Estate Studio

A plain-language guide to running the `mad-prompters-real-estate-studio` skill. Keep this next to the skill in your library.

---

## What it does

Takes a folder of ordinary listing photos and produces a **15-second cinematic property video** — running entirely inside a Claude chat on the Higgsfield MCP. The whole point is that the video **actually looks like the real house** (no warping/"morphing" into invented rooms), in the **visual style of your choice**, with optional music, voiceover, and on-screen text.

You pick a **style** at the start, and that style can be either:

- a **smooth continuous walkthrough** (a true one-take glide through the home), or
- a **punchy viral cut-style edit** (fast hard cuts, punch-ins, FX — built for the feed).

It works for **any tier** — a luxury estate, a family home, or an updated starter/character home — and adapts the look and the copy to match.

---

## The 10 styles (pick one first)

Every style keeps the same morph-free lock to your real photos. Only the camera, cutting, energy, grade, and audio change.

**Walkthrough styles (continuous one-take):**

| Style | The vibe | Best for |
|---|---|---|
| **Smooth Glide** *(default)* | Calm, golden-hour glide | Any property — the safe workhorse |
| **Luxe Cinematic** | Slow crane/dolly, rich contrast, orchestral | Luxury / modern / architectural |
| **FPV Rush** | Fast drone-style flythrough | Social, younger buyers, fast flow |
| **Bright & Airy** | Clean midday daylight, soft + welcoming | Family / starter / mid-market |
| **Twilight Glam** | Warm evening exterior, glowing interiors | Evening hero / curb appeal |
| **Social Pop** | Vertical-native, beat-synced | Reels / TikTok / Shorts lead-gen |
| **Story (Narrated)** | Emotional, documentary cadence, voiceover-led | Agent-brand storytelling |

**Viral cut styles (one clip, internal hard cuts):**

| Style | The vibe | Best for |
|---|---|---|
| **Viral Cut** | Fast hard cuts on the beat, punch-in/out zooms, speed ramps | Scroll-stopping listing edit |
| **FX Showcase** | Snappy cuts + stylized FX (zoom-blur whips, light streaks, flares) | Eye-candy social that still reads every room |
| **Hype Reel** | Fastest cuts, punch/shake, beat-drop sync, bold hooks | Maximum-energy hook for the feed |

> **The cut styles still don't morph.** They hard-cut *between* locked real frames and only ever apply FX *on* those frames — so even a fast edit stays faithful to the house. Seedance renders the whole thing as **one 15-second clip** (no stitching, no separate editing app).

---

## Creator Mode (make a walkthrough hit harder)

**Creator Mode** is a toggle that layers viral pacing — punch-in zooms, speed ramps, beat-sync, and a few well-placed hard cuts — **on top of any walkthrough style** (except Story, where it would fight the narration). So you can run **Twilight Glam + Creator Mode** and get the glam evening look, but cut to land on the feed. It keeps the base style's grade and mood; it just adds energy.

---

## When it runs

**Automatically**, when you start a property-video task. You don't flip a switch — just describe what you want. Openers that trigger it:

- "Make a 15-second walkthrough video for this new listing" *(+ attach photos)*
- "Turn these home photos into a reel"
- "I want a viral cut-style edit of this listing for TikTok"
- Even just dropping a batch of interior/exterior shots and asking for footage

**Or force it by name:** start a message with `/mad-prompters-real-estate-studio`.

---

## Before you start

1. **Enable the Higgsfield connector** in the conversation. Every generation (storyboard image, voiceover, video) runs through it.
2. **Have the photos ready.** Up to 30 per home. Listing/MLS photos are perfect.
3. **Optional:** a property description (address, beds/baths, standout features). Helps the copy.

---

## The flow, step by step

**1. Kick it off.** Use one of the openers above, or `/mad-prompters-real-estate-studio`.

**2. Pick a style.** Because there are 10 presets, you choose in two quick taps:
   - First tap: **Walkthrough**, **Viral Cut / FX**, or **Recommend one** (Claude picks from your property).
   - Second tap: up to 4 curated presets from that family.
   - If you picked a walkthrough, Claude offers **Creator Mode** ("add viral pacing?").

**3. Drop the photos + description.** Attach the photos **in the chat** (so Claude can see and judge them) and paste any description. Chat attachments have no count limit — attach all of them here first.

**4. Approve the hero shots.** Claude looks at every photo, sorts them into beats (exterior → living → kitchen → feature room → outside → exterior close), and proposes **4–6 hero shots by filename** with a one-line reason each. It tells you what it excluded (floorplans, raw/unfinished spaces, clutter, redundant angles). Swap anything, then approve.

**5. Upload the winners.** Claude opens the Higgsfield uploader for **only the approved shots** (max 20 per batch) and maps each filename to its Higgsfield ID.

**6. Answer what's left** (tappable). The style already set the grade, energy, transitions, beat count, genre, and audio feel — so Claude only asks the leftovers:
   - **Engine** — Seedance 2.0 (default) or Marketing Studio.
   - **Aspect** — only if the style didn't already set one (cut styles default to 9:16).
   - **Audio** — confirm or flip the style's default (music on/off, VO on/off).
   - **CTA line** (free text), or skip.
   - **On-screen text** — *if you chose a cut style or Creator Mode*, Claude asks whether you want text hooks (see next section).

**7. Approve the storyboard.** Claude generates a locked storyboard image from your real rooms — **9 panels** for most walkthroughs, **12 panels** for high-energy and cut styles (where it's a *shot list* of hard-cut frames). Eyeball it for fidelity — especially that the kitchen and feature room didn't blend — then lock it. *This is the most important checkpoint.*

**8. (If voiceover is on) Approve the script + pick a voice.** Claude writes a timed ~40-word script — **hook (0–3s) / body (3–12s) / CTA (12–15s)** — aligned to the beats. Approve it, pick a voice, and it generates the VO.

**9. It renders the video.** Claude runs the engine (Seedance does the full 15s — including any internal cuts — in one clip) and the result appears in the chat. It flags any drift to check.

**10. Finish in post.** One quick step happens outside the chat (by design):
   - Drop a **licensed music track** if you used the native bed (it's a scratch track).
   - *(On-screen text already renders in the clip — it's baked into the storyboard. Only touch it in post if a line came out soft or you want a different font.)*

---

## On-screen text (for cut styles & Creator Mode)

When a cut style or Creator Mode is active, Claude asks if you want on-screen text — and if yes, offers a menu:

- **Hook + payoff** — e.g. "WAIT FOR THE KITCHEN" → the reveal.
- **Stat cards** — "3 BED • 3 BATH • UPDATED," price, or address.
- **CTA punches** — "BOOK A SHOWING," "DM TO TOUR."
- **Custom** — you type the exact copy.

Claude confirms the literal lines and where they land, then **bakes them right into the storyboard panels** — `gpt_image_2` renders clean type and Seedance carries it into the video, so the words pop up on screen in the final clip with no editing app required. Keep them short and punchy (caps read best). Post is only a fallback if a line comes out soft or you want a font you can't get in-image.

---

## Choosing the engine

| Pick **Seedance 2.0** (default) when… | Pick **Marketing Studio** when… |
|---|---|
| You want a true continuous one-take **or** an internal-cut viral edit | You want a product-template/brand-spot look |
| You want the full 15s (cuts included) in a single render | You already have an MS product flow going |
| You want native audio + voiceover timing in-engine | You'll handle all audio in post anyway |

> **Note:** "Hyper Motion" is **not** a Marketing Studio mode. For continuous-flythrough or hard-cut looks, use Seedance — that's its specialty, and it does the cut styles' internal hard cuts in one clip.

---

## Audio options, explained

- **Music ON** → Seedance lays a **native audio bed** (a scratch track — swap a licensed cue for delivery).
- **Voiceover ON** → Claude writes the timed script, generates the VO with Higgsfield text-to-speech, and the video is built around it.
- **Both ON** → VO is baked in-engine; add the licensed music under it in post.
- **Both OFF** → silent clip.

> Standalone **music generation** isn't available through this pipeline, so a polished, *licensed* track is always a post step — regardless of engine.

---

## Tips for the best result

- **Match the style to the home.** Bright & Airy for a starter home, Luxe for an estate, Viral Cut/Hype Reel when you need the scroll-stop. Let Claude recommend if you're unsure.
- **Give it range.** A strong front exterior, your best kitchen, the standout room, and an outdoor shot. Coverage diversity beats ten shots of the same room.
- **Skip the dead weight.** Floorplans, unfinished basements, and tight clutter shots hurt the story — Claude excludes them.
- **Trust the gates.** The hero-shot and storyboard checkpoints are where you steer the whole video — a 10-second look there saves a re-render.
- **Want both energies?** Run a walkthrough style *and* a cut style off the same photos to A/B which performs.

---

## Known limits & gotchas

- **On-screen text renders in the clip.** When you ask for text, it's baked into the storyboard and comes through in the video — no post step. (Keep it short; very long lines or a specific font are the only reasons to add it in post instead.)
- **Native music is a scratch bed.** Replace with a licensed track for delivery.
- **Marketing Studio renders silent.** All audio is post for that engine.
- **One continuous take has honest seams.** Going front → backyard → front isn't a real oner, so the closing exterior is a clean "beauty-card" cut.
- **Cut styles are still one clip.** The hard cuts happen *inside* a single Seedance render — there's no separate editing step to assemble them.
- **Preset auto-match.** Higgsfield sometimes thinks your prompt matches a named preset (like "IN THE DARK") and pauses — the skill declines it and generates your exact prompt. (Evening styles trip this every time; it's handled.)

---

## Quick reference

```
Style    →  pick a preset (Walkthrough / Viral-Cut / Recommend) — tappable
            (walkthrough? optional Creator Mode for viral pacing)
Photos   →  attach in chat (≤30) for triage
Triage   →  approve 4–6 hero shots by filename
Upload   →  winners only, via the Higgsfield widget (≤20/batch)
Options  →  only what the style didn't set (engine · aspect · audio · CTA · text)
Story    →  9- or 12-panel board, locked to real rooms  → APPROVE
Script   →  (if VO) hook/body/CTA ~40 words             → APPROVE
Render   →  Seedance 2.0 — one 15s clip (cuts included)
Post     →  licensed music (text already renders in-clip)
```
