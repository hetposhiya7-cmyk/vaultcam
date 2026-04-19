# ✅ VaultCam Production Checklist

Step-by-step SOP for producing a single VaultCam YouTube Short from concept to upload.

---

## Phase 1 — Pre-Production

- [ ] **Select incident** — real, verifiable event with available bodycam/CCTV context
- [ ] **Research** — collect key facts: date, location, names, outcome
- [ ] **Write script** — use Fish AI voiceover format (see `/prompts/voiceover-prompts.md`)
- [ ] **Save to Notion** — paste script into VaultCam Notion workspace under correct batch
- [ ] **Save to repo** — add script file to `/scripts/` with naming convention `b[X]-v[Y]-[slug].md`
- [ ] **Write Scene Lock header** — define visual constants for this video (setting, lighting, camera style, color grade)

---

## Phase 2 — Image Generation (Google Flow)

- [ ] Open [flow.google](https://flow.google)
- [ ] For each scene:
  - [ ] Prepend Scene Lock header to prompt
  - [ ] Write scene-specific prompt (see `/prompts/image-prompts.md`)
  - [ ] Generate image
  - [ ] Review — check consistency with previous scenes
  - [ ] Regenerate if visual inconsistency detected
- [ ] Export all images at highest available resolution
- [ ] Number images sequentially: `scene-01.png`, `scene-02.png`, etc.

---

## Phase 3 — Voiceover Generation (Fish AI)

- [ ] Open [fish.audio](https://fish.audio)
- [ ] Select correct voice profile
- [ ] Paste formatted script with tags (see `/prompts/voiceover-prompts.md`)
- [ ] Generate audio
- [ ] Listen through — check for unnatural pauses, mispronunciations, or flat delivery
- [ ] Re-generate problem lines individually if needed
- [ ] Export as MP3 or WAV

---

## Phase 4 — Video Assembly (CapCut)

- [ ] Create new project — 9:16 vertical, 1080×1920, 60fps
- [ ] Import all scene images
- [ ] Import voiceover audio
- [ ] Sync images to voiceover timing:
  - [ ] Each image displayed for appropriate duration per narration beat
  - [ ] Add subtle Ken Burns (zoom/pan) effect to each image for motion
- [ ] Add on-screen text:
  - [ ] **"AI Generated"** label — persistent or intro card
  - [ ] Location/date lower third where relevant
- [ ] Add sound design:
  - [ ] Ambient background audio (police radio static, outdoor ambience, etc.)
  - [ ] Optional: subtle tension music bed at low volume
- [ ] Color grade — match desaturated/documentary feel if not already in images
- [ ] Add VaultCam outro (subscribe CTA)
- [ ] Export: 1080×1920, H.264, high bitrate

---

## Phase 5 — Upload & Publishing

- [ ] **Title format:** `[AI Generated] [Incident Description] #Shorts`
- [ ] **Description:** Brief factual summary + "All content AI Generated" disclaimer
- [ ] **Tags:** bodycam, police, AI generated, shorts, [location], [incident type]
- [ ] **Thumbnail:** Custom frame from video or separately generated image
- [ ] **Schedule or publish** via YouTube Studio
- [ ] **Update Airtable** — mark video as published, add YouTube URL
- [ ] **Update Notion batch tracker** — mark status as Published
- [ ] **Update `/scripts/README.md`** — update status to ✅ Published

---

## Phase 6 — Post-Upload Review (48 hours later)

- [ ] Check views, watch time, CTR in YouTube Studio
- [ ] Note any retention drop-off points
- [ ] Log observations in Notion for next batch improvements
