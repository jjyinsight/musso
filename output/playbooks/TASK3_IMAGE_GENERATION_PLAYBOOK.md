# Task 3: Image Generation Execution Playbook
**무쏘맨 AI 어워즈 - 5 Scene Image Generation**

**Status**: READY FOR EXECUTION (awaiting Task 1 completion)  
**Tool**: Leonardo.ai  
**Duration**: 2-3 hours  
**Output**: 5 high-quality scene images (1024x1024+)

---

## 📋 Executive Summary

Generate 5 cinematic scene images for the Mussoman transformation video:
1. Desert intro (silhouette in sandstorm)
2. Mussoman sprint (side view action)
3. Close-up power (determined expression)
4. Transformation setup (pre-transformation pose)
5. Musso finale (pickup truck + KGM logo)

**Quality Standard**: Epic/cinematic movie trailer aesthetic, consistent visual style, 1536x1536 resolution preferred.

---

## ✅ Prerequisites Checklist

- [ ] Task 1 complete (Leonardo.ai account created)
- [ ] Leonardo.ai logged in with credits available
- [ ] Reference images reviewed (`src/무쏘, 무쏘맨_자료 모음/무쏘맨_누끼/`)
- [ ] Transformation strategy reviewed (`output/strategy/transformation_strategy.md`)
- [ ] Output directory exists (`output/images/`)

---

## 🎬 Scene 1: Desert Intro - Silhouette in Sandstorm

### Visual Description
Vast desert landscape at golden hour, massive sandstorm approaching from the horizon. In the foreground, a powerful silhouette of Mussoman (anthropomorphic rhino character) stands heroically, backlit by dramatic sunset. Sand particles swirl around, creating atmospheric depth. Wide cinematic composition emphasizing scale and isolation.

### Leonardo.ai Prompt

**Positive Prompt**:
```
Epic cinematic wide shot of vast desert landscape at golden hour, 
massive sandstorm approaching in background, 
powerful silhouette of anthropomorphic rhino character standing heroically in foreground,
backlit by dramatic orange sunset, 
sand particles swirling in wind creating atmospheric depth,
cinematic composition, movie trailer aesthetic,
8k quality, photorealistic, dramatic lighting,
rule of thirds composition, epic scale
```

**Negative Prompt**:
```
cartoon, anime, low quality, blurry, distorted, multiple characters, 
text, watermark, signature, oversaturated, unrealistic proportions
```

**Settings**:
- Model: Leonardo Phoenix or Leonardo Kino XL
- Aspect Ratio: 1:1 (1536x1536)
- Guidance Scale: 7-9
- Number of Images: 3 (select best)

### Quality Acceptance Criteria
- [ ] Silhouette clearly recognizable as humanoid rhino
- [ ] Sandstorm creates dramatic atmosphere
- [ ] Golden hour lighting evident
- [ ] Composition follows rule of thirds
- [ ] Resolution 1024x1024 minimum
- [ ] No text/watermarks visible

### File Naming
- `scene_01_v1.png`, `scene_01_v2.png`, `scene_01_v3.png`
- Final selection: `scene_01.png`

---

## 🏃 Scene 2: Mussoman Sprint - Side View Action

### Visual Description
Dynamic side-view shot of Mussoman running powerfully across desert terrain. Anthropomorphic rhino character with muscular humanoid body wearing tactical/adventure clothing, rhino face with prominent horn clearly visible. Dust trail behind him, motion blur suggesting speed. Mid-action pose captured at peak movement. Desert background with sand dunes, dramatic sky.

### Character Reference
- **Face**: Rhino features (horn, thick skin texture, powerful jaw)
- **Body**: Muscular humanoid build, athletic pose
- **Clothing**: Adventure/tactical style (refer to `무쏘맨_전시장.png`)
- **Colors**: Earth tones, desert palette

### Leonardo.ai Prompt

**Positive Prompt**:
```
Dynamic side view action shot of anthropomorphic rhino character running powerfully,
muscular humanoid body with rhino face and prominent horn,
wearing tactical adventure clothing,
mid-sprint pose with one leg forward, arms pumping,
dust trail and sand particles kicked up behind,
motion blur suggesting speed and power,
desert background with sand dunes,
dramatic sky with golden sunlight,
cinematic composition, movie action scene,
8k quality, photorealistic, epic lighting,
detailed character design, heroic pose
```

**Negative Prompt**:
```
cartoon, anime, static pose, multiple characters, 
blurry face, distorted anatomy, low quality,
text, watermark, unrealistic proportions
```

**Settings**:
- Model: Leonardo Phoenix (better for character consistency)
- Aspect Ratio: 1:1 (1536x1536)
- Guidance Scale: 8-10
- Number of Images: 3

### Quality Acceptance Criteria
- [ ] Rhino facial features clearly visible
- [ ] Humanoid body proportions correct
- [ ] Dynamic running pose convincing
- [ ] Dust trail adds motion sense
- [ ] Desert environment consistent with Scene 1
- [ ] Character matches reference images

### Troubleshooting
- **Issue**: Character looks too cartoonish
  - **Fix**: Add "photorealistic, detailed skin texture, realistic anatomy" to prompt
- **Issue**: Rhino features not prominent
  - **Fix**: Emphasize "prominent rhino horn, thick rhino skin, powerful rhino face"

---

## 💪 Scene 3: Close-up Power - Determined Expression

### Visual Description
Dramatic close-up of Mussoman's face and upper torso. Rhino face with intense, determined expression - eyes focused, jaw set, horn prominent. Slight upward camera angle to emphasize heroism. Background: defocused desert with dramatic sky. Lighting: rim light from behind creating heroic glow, face partially shadowed for drama.

### Leonardo.ai Prompt

**Positive Prompt**:
```
Dramatic close-up portrait of anthropomorphic rhino character,
intense determined expression with focused eyes,
prominent rhino horn catching light,
thick textured rhino skin with realistic details,
powerful jaw set with resolve,
slight upward camera angle emphasizing heroism,
rim lighting from behind creating heroic glow,
face partially shadowed for dramatic effect,
defocused desert background with dramatic sky,
cinematic portrait, movie hero shot,
8k quality, photorealistic, epic lighting,
detailed facial features, emotional intensity
```

**Negative Prompt**:
```
cartoon, anime, smiling, friendly expression, 
multiple characters, blurry, low quality,
text, watermark, flat lighting
```

**Settings**:
- Model: Leonardo Phoenix
- Aspect Ratio: 1:1 (1536x1536)
- Guidance Scale: 9-11 (higher for facial detail)
- Number of Images: 3

### Quality Acceptance Criteria
- [ ] Facial expression conveys determination
- [ ] Rhino features detailed and realistic
- [ ] Rim lighting creates heroic effect
- [ ] Background appropriately defocused
- [ ] Emotional intensity evident
- [ ] Matches character from Scene 2

### Reference
- Study `무쏘맨_기다림.png` and `무쏘맨_월척.png` for facial expressions

---

## ⚡ Scene 4: Transformation Setup - Pre-Transformation Pose

### Visual Description
Mussoman in powerful stance, arms spread wide, energy aura beginning to emanate from body. Dramatic lighting with glowing effects around character. Desert ground cracking beneath feet from power surge. Sky darkening with energy buildup. This is the moment before transformation - tension and power building.

### Leonardo.ai Prompt

**Positive Prompt**:
```
Anthropomorphic rhino character in powerful transformation stance,
arms spread wide with palms open,
glowing energy aura emanating from body,
electric blue and orange energy particles swirling around,
desert ground cracking beneath feet from power surge,
dramatic lighting with energy glow illuminating character,
sky darkening with storm clouds gathering,
tension and power building in the air,
cinematic transformation scene, epic moment,
8k quality, photorealistic with magical realism,
detailed energy effects, dramatic composition
```

**Negative Prompt**:
```
cartoon, anime, static pose, weak energy effects,
multiple characters, blurry, low quality,
text, watermark, flat lighting
```

**Settings**:
- Model: Leonardo Kino XL (better for effects)
- Aspect Ratio: 1:1 (1536x1536)
- Guidance Scale: 7-9
- Number of Images: 3

### Quality Acceptance Criteria
- [ ] Transformation pose dynamic and powerful
- [ ] Energy effects visible and dramatic
- [ ] Ground cracking effect present
- [ ] Lighting emphasizes power buildup
- [ ] Character consistent with previous scenes
- [ ] Sets up transformation visually

### Integration Note
This image feeds directly into Task 4 (video generation) for the transformation sequence. Energy effects should be prominent enough to justify the transformation.

---

## 🚗 Scene 5: Musso Finale - Pickup Truck + KGM Logo

### Visual Description
KGM Musso pickup truck driving powerfully through desert, dust cloud trailing behind. Vehicle shot from dynamic 3/4 angle showing both front and side. Golden hour lighting making chrome and paint gleam. "Powered by Toughness" text integrated naturally (or KGM logo visible on vehicle). Triumphant, powerful mood - the transformation complete.

### Vehicle Reference
- Check `src/무쏘_누끼/` for accurate Musso design
- Color: Typically silver/grey or dark colors
- Style: Rugged, powerful, modern pickup

### Leonardo.ai Prompt

**Positive Prompt**:
```
KGM Musso pickup truck driving powerfully through desert landscape,
dynamic 3/4 angle showing front and side of vehicle,
massive dust cloud trailing behind,
chrome details and paint gleaming in golden hour sunlight,
rugged modern pickup truck design,
desert environment with sand dunes,
dramatic sky with warm sunset colors,
cinematic vehicle shot, automotive photography style,
8k quality, photorealistic, epic scale,
detailed vehicle design, powerful presence
```

**Negative Prompt**:
```
cartoon, toy car, low quality, blurry,
wrong vehicle type, multiple vehicles,
text, watermark, unrealistic proportions
```

**Settings**:
- Model: Leonardo Phoenix
- Aspect Ratio: 1:1 (1536x1536)
- Guidance Scale: 8-10
- Number of Images: 3

### Quality Acceptance Criteria
- [ ] Vehicle recognizable as pickup truck
- [ ] Dust cloud adds dynamic motion
- [ ] Lighting consistent with Scene 1 (golden hour)
- [ ] Vehicle design matches Musso reference
- [ ] Composition powerful and triumphant
- [ ] Desert environment consistent

### Brand Integration
- KGM logo can be added in Task 6 (editing) if not naturally generated
- "Powered by Toughness" text will be added as subtitle in final edit

---

## 🎨 Prompt Engineering Best Practices

### Leonardo.ai Syntax Tips
1. **Front-load important elements**: Put key subjects at beginning of prompt
2. **Use specific descriptors**: "anthropomorphic rhino" not just "character"
3. **Lighting keywords**: "golden hour", "rim lighting", "dramatic shadows"
4. **Quality modifiers**: "8k quality", "photorealistic", "cinematic"
5. **Composition terms**: "rule of thirds", "dynamic angle", "wide shot"

### Style Consistency
- Use same quality modifiers across all scenes: "8k quality, photorealistic, cinematic"
- Maintain lighting consistency: "golden hour" or "dramatic lighting"
- Keep color palette coherent: desert tones (golden, sandy, warm)

### Negative Prompts
Always include:
- `cartoon, anime` (avoid stylization)
- `low quality, blurry` (ensure sharpness)
- `text, watermark` (clean images)
- `multiple characters` (focus on single subject)

---

## 📊 Quality Control Process

### Resolution Check
```bash
file output/images/scene_*.png
# Should show: 1024 x 1024 or higher
```

### Visual Consistency Review
1. **Color Palette**: All scenes use desert/golden tones
2. **Lighting**: Consistent time of day (golden hour)
3. **Character**: Mussoman features recognizable across scenes
4. **Style**: All images have cinematic/epic aesthetic

### Iteration Strategy
- Generate 3 versions per scene
- Select best based on:
  - Technical quality (resolution, sharpness)
  - Composition (rule of thirds, balance)
  - Character accuracy (matches references)
  - Emotional impact (epic, heroic feel)

### Acceptance Checklist
- [ ] All 5 scenes generated
- [ ] Resolution 1024x1024 minimum (1536x1536 preferred)
- [ ] Visual style consistent across scenes
- [ ] Character recognizable in Scenes 2-4
- [ ] No watermarks or text
- [ ] Files properly named and organized

---

## 📁 File Management

### Directory Structure
```
output/
├── images/
│   ├── scene_01_v1.png
│   ├── scene_01_v2.png
│   ├── scene_01_v3.png
│   ├── scene_01.png          ← Final selection
│   ├── scene_02_v1.png
│   ├── scene_02_v2.png
│   ├── scene_02_v3.png
│   ├── scene_02.png          ← Final selection
│   ├── ... (scenes 3-5)
│   └── metadata.txt          ← Prompts used
```

### Metadata Tracking
Create `output/images/metadata.txt`:
```
Scene 1: [prompt used] | Settings: [model, guidance] | Selected: v2
Scene 2: [prompt used] | Settings: [model, guidance] | Selected: v1
...
```

---

## 🔧 Troubleshooting Guide

### Common Issues

**Issue**: Character doesn't look like a rhino
- **Solution**: Emphasize "prominent rhino horn, thick rhino skin, rhino facial features"
- **Alternative**: Use Image Reference feature in Leonardo.ai with `무쏘맨_전시장.png`

**Issue**: Images too cartoonish
- **Solution**: Add "photorealistic, detailed texture, realistic anatomy, professional photography"
- **Remove**: Any anime/cartoon style keywords

**Issue**: Inconsistent character across scenes
- **Solution**: Use same character description in all prompts
- **Alternative**: Generate Scene 2 first, use as reference for Scenes 3-4

**Issue**: Background too busy/distracting
- **Solution**: Add "simple desert background, defocused background" to prompt
- **Increase**: Guidance scale for better subject focus

**Issue**: Low resolution output
- **Solution**: Select 1536x1536 in settings
- **Check**: Leonardo.ai plan limits (free tier may cap resolution)

**Issue**: Watermarks visible
- **Solution**: Ensure using Leonardo.ai (not free trial with watermarks)
- **Alternative**: Crop watermark in post-processing

---

## ⏱️ Execution Timeline

| Phase | Duration | Activity |
|-------|----------|----------|
| Setup | 10 min | Review prompts, prepare references |
| Scene 1 | 20 min | Generate 3 versions, select best |
| Scene 2 | 25 min | Generate 3 versions, select best (character focus) |
| Scene 3 | 25 min | Generate 3 versions, select best (facial detail) |
| Scene 4 | 25 min | Generate 3 versions, select best (effects) |
| Scene 5 | 20 min | Generate 3 versions, select best |
| QC | 15 min | Review consistency, resolution, quality |
| **Total** | **2-3 hours** | Including iteration time |

---

## 🚀 Next Steps

After completing Task 3:
1. Verify all 5 images meet quality criteria
2. Update notepad: `.sisyphus/notepads/mussoman-ai-video/learnings.md`
3. Proceed to Task 4: Video Generation (uses these images as input)

---

## 📚 Reference Materials

- **Character Images**: `src/무쏘, 무쏘맨_자료 모음/무쏘맨_누끼/*.png`
- **Vehicle Images**: `src/무쏘_누끼/`
- **Transformation Strategy**: `output/strategy/transformation_strategy.md`
- **Brand Philosophy**: "Powered by Toughness"

---

**Document Version**: 1.0  
**Last Updated**: 2026-01-29  
**Status**: READY FOR EXECUTION
