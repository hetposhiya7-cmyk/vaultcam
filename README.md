# VaultCam 🎥

> AI-generated faceless YouTube Shorts production pipeline — bodycam, CCTV, and dashcam-style content.

---

## 📌 What is VaultCam?

VaultCam is a fully AI-generated, faceless YouTube Shorts channel focused on real-incident recreations using bodycam and CCTV-style footage aesthetics. All content is labeled **"AI Generated"** in titles, captions, and on-screen text.

The pipeline combines:
- **Google Flow** — AI image/scene generation with Scene Lock headers for visual consistency
- **Fish AI** — Voiceover generation with emotion/pause tags (single-narrator format)
- **CapCut** — Video editing and assembly
- **Notion** — Script writing and batch management

---

## 📁 Repository Structure

```
vaultcam/
├── README.md                        # Project overview (this file)
├── scripts/
│   └── README.md                    # Index of all video scripts by batch
├── prompts/
│   ├── image-prompts.md             # Google Flow image prompt templates
│   └── voiceover-prompts.md         # Fish AI voice tags and format guide
├── workflow/
│   └── production-checklist.md      # Step-by-step video production SOP
└── assets/
    └── README.md                    # Reference links and asset notes
```

---

## 🎬 Batch Log

| Batch | Videos | Status |
|-------|--------|--------|
| Batch 1 | Videos 1–5 | ✅ Complete |
| Batch 2 | Videos 6–8 | ✅ Scripts done |
| Batch 3 | Videos 9–10 | 🔄 In production |

---

## ⚙️ Tech Stack

| Tool | Purpose |
|------|---------|
| Google Flow (flow.google) | AI scene/image generation |
| Fish AI | Voiceover with emotion tags |
| CapCut | Video editing & assembly |
| Notion | Script writing & batch tracking |
| Airtable | Content channel tracker |

---

## ⚠️ Compliance

All VaultCam content must include:
- `[AI Generated]` in the video title
- "AI Generated" caption on first frame or throughout
- On-screen disclaimer text where applicable

---

## 🚀 Getting Started

1. Read `/workflow/production-checklist.md` for the full production SOP
2. Use `/prompts/image-prompts.md` for Google Flow scene generation
3. Use `/prompts/voiceover-prompts.md` for Fish AI narration formatting
4. Store completed scripts in `/scripts/` with batch prefix (e.g. `b2-v6-hurst-traffic-stop.md`)
