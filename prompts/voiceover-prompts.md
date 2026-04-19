# 🎙️ Fish AI — Voiceover Tags & Format Guide

All VaultCam narration is generated via [Fish AI](https://fish.audio) using the **single-narrator format**. This guide covers tag usage, pacing conventions, and formatting standards.

---

## Voice Profile

| Setting | Value |
|---------|-------|
| Voice | [Your selected Fish AI voice ID] |
| Format | Single narrator |
| Style | Calm, authoritative, documentary tone |
| Tempo | Moderate — not rushed, not dramatic |

---

## Tag Reference

### Pause Tags
| Tag | Effect |
|-----|--------|
| `[pause:short]` | ~0.3s pause — between clauses |
| `[pause:medium]` | ~0.7s pause — between sentences for weight |
| `[pause:long]` | ~1.2s pause — after dramatic reveals |

### Tone / Emotion Tags
| Tag | Effect |
|-----|--------|
| `[tone:calm]` | Neutral, documentary delivery |
| `[tone:tense]` | Slightly elevated urgency |
| `[tone:serious]` | Grave, weighted delivery |
| `[tone:urgent]` | Faster pace, heightened energy |

### Emphasis
| Tag | Effect |
|-----|--------|
| `[emphasis]word[/emphasis]` | Stress a specific word |

---

## Script Formatting Standard

```
[tone:calm] It was a routine traffic stop. [pause:medium]
The kind officers handle hundreds of times a year. [pause:short]
But this one [pause:short] was different. [pause:long]

[tone:tense] At 11:42 PM, [emphasis]Deputy Harris[/emphasis] pulled over a black F-150 on Route 9. [pause:medium]
What he didn't know [pause:short] was what was waiting inside. [pause:long]
```

---

## Pacing Guidelines

- **Opening hook:** Start with `[tone:calm]`, short punchy sentences, `[pause:medium]` between each.
- **Rising tension:** Shift to `[tone:tense]` as the incident escalates. Shorten sentences.
- **Peak moment:** Use `[pause:long]` before and after the key dramatic beat.
- **Resolution:** Return to `[tone:calm]` or `[tone:serious]` for the outcome.
- **Outro:** End with a reflective line + `[pause:medium]` before final CTA.

---

## Full Script Template

```
[tone:calm] [HOOK — 1-2 punchy lines setting the scene] [pause:long]

[tone:calm] [CONTEXT — Who, where, when. 2-3 sentences.] [pause:medium]

[tone:tense] [ESCALATION — What went wrong / unexpected. 3-4 sentences.] [pause:medium]

[tone:urgent] [PEAK — The critical moment. Short, sharp sentences.] [pause:long]

[tone:serious] [OUTCOME — What happened next. 2-3 sentences.] [pause:medium]

[tone:calm] [REFLECTION — 1 closing line.] [pause:medium]
If you want to see more incidents like this, [emphasis]subscribe[/emphasis]. [pause:short] VaultCam.
```

---

## Notes

- Do **not** use multiple emotion tags back-to-back without a pause between them.
- Keep individual sentences under 20 words for clean TTS output.
- Avoid em-dashes (—) — replace with `[pause:short]` for better rhythm.
- Always end with the VaultCam sign-off line.
