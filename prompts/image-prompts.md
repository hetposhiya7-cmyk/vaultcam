# 🖼️ Google Flow — Image Prompt Templates

All image generation is done via [Google Flow](https://flow.google). Since Flow lacks cross-generation context, every prompt must include a **Scene Lock header** to maintain visual consistency across scenes.

---

## Scene Lock Header (Paste at top of every prompt)

The Scene Lock header defines fixed visual parameters for a video. Copy and prepend to every image prompt in that video.

```
[SCENE LOCK]
Setting: [location — e.g. suburban highway, night, rain]
Lighting: [e.g. flashing blue-red police lights, headlights]
Camera style: [e.g. bodycam POV, fisheye lens, handheld shaky]
Color grade: [e.g. desaturated, cool tones, high contrast]
Time of day: [e.g. late night / golden hour / overcast day]
Officer appearance: [e.g. male, dark uniform, visible badge, short hair]
Vehicle: [e.g. black Ford F-150, rear-ended, hazard lights on]
[/SCENE LOCK]
```

---

## Base Prompt Structure

```
[SCENE LOCK BLOCK]

Scene: [what is happening in this specific frame]
Foreground: [main subject and action]
Background: [environment details]
Mood: [tense / urgent / calm / chaotic]
Text overlay: NONE
Style: photorealistic, documentary, cinematic
Negative: cartoon, illustration, text, watermark, blurry
```

---

## Example Prompts by Scene Type

### Bodycam POV — Officer Approach
```
[SCENE LOCK]
Setting: suburban road, night
Lighting: police cruiser lights flashing red and blue
Camera style: bodycam POV, slight fisheye, shaky
Color grade: desaturated, high contrast
[/SCENE LOCK]

Scene: Officer approaching a stopped vehicle from behind
Foreground: back of officer's hand reaching toward car door handle
Background: lit-up vehicle interior, driver silhouette visible
Mood: tense
Style: photorealistic, bodycam footage
Negative: cartoon, text, watermark
```

### CCTV Overview — Parking Lot Incident
```
[SCENE LOCK]
Setting: parking lot, evening
Lighting: harsh overhead fluorescent lights, deep shadows
Camera style: fixed CCTV wide angle, elevated POV, timestamp overlay
Color grade: washed out, slightly grainy
[/SCENE LOCK]

Scene: Two figures in confrontation near a parked car
Foreground: man pointing aggressively, second person backing away
Background: empty parking lot, lone streetlight
Mood: chaotic
Style: surveillance footage, photorealistic
Negative: cartoon, illustration, watermark
```

### Rescue Scene — Water
```
[SCENE LOCK]
Setting: river bank, daytime, overcast
Lighting: flat natural light, grey sky
Camera style: handheld news-style, slightly shaky
Color grade: muted greens and blues
[/SCENE LOCK]

Scene: Officer wading into river toward struggling swimmer
Foreground: officer waist-deep in water, arm extended
Background: fast-moving river, far bank with trees
Mood: urgent
Style: photorealistic, documentary
Negative: cartoon, text, watermark
```

---

## Tips

- **Always repeat the Scene Lock block** for every prompt in the same video — Flow has no memory between generations.
- Keep `Text overlay: NONE` unless you specifically want on-screen text.
- For consistent officer appearance, describe physical traits in the Scene Lock block, not just individual prompts.
- If a scene looks off, add `ultra-detailed, sharp focus` to quality boosters.
