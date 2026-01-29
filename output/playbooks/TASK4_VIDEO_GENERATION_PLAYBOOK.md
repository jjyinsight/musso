# Task 4: Video Generation Execution Playbook
**무쏘맨 AI 어워즈 - 5 Scene Video Generation**

**Status**: READY FOR EXECUTION (awaiting Task 3 completion)  
**Tool**: Kling AI / Pika Labs / Runway ML  
**Duration**: 4-6 hours  
**Output**: 5 video clips (3-5 seconds each)

---

## 📋 Executive Summary

Generate 5 cinematic video clips from Task 3 images:
1. Desert intro - Zoom into silhouette
2. Mussoman sprint - Side tracking shot
3. Close-up power - Slow zoom with intensity
4. **Transformation** - Character to vehicle (CRITICAL)
5. Musso finale - Truck driving with dust trail

**Quality Standard**: Cinematic motion, smooth camera work, 3-5 seconds per clip, transformation scene must be convincing.

---

## ✅ Prerequisites Checklist

- [ ] Task 1 complete (AI tool accounts created)
- [ ] Task 3 complete (5 scene images generated)
- [ ] Transformation strategy reviewed (`output/strategy/transformation_strategy.md`)
- [ ] Tool selected (Kling AI, Pika Labs, or Runway ML)
- [ ] Output directory exists (`output/videos/`)

---

## 🎬 Tool Selection Decision

### Recommended Priority Order

**1st Choice: Pika Labs 2.5** ⭐
- **Why**: Pikaffects transformation effects (Melt, Dissolve, Transform)
- **Best For**: Scene 4 (transformation)
- **Pros**: Specialized transformation tools, good motion quality
- **Cons**: 5-10 second clip limit

**2nd Choice: Kling AI 2.5**
- **Why**: Good character animation, vehicle examples exist
- **Best For**: Scenes 2, 5 (character/vehicle motion)
- **Pros**: Longer clips possible, good physics
- **Cons**: Less transformation-specific features

**3rd Choice: Runway Gen-4**
- **Why**: Highest quality output, best motion control
- **Best For**: All scenes if budget allows
- **Pros**: Cinema-quality, precise motion prompting
- **Cons**: More expensive, steeper learning curve

### Decision Matrix

| Scene | Pika Labs | Kling AI | Runway Gen-4 |
|-------|-----------|----------|--------------|
| 1. Desert intro | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| 2. Sprint | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| 3. Close-up | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| 4. **Transformation** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| 5. Finale | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ |

**Recommended Approach**: Use Pika Labs for Scene 4 (transformation), Kling AI for others.

---

## 🎥 Scene 1: Desert Intro - Zoom Into Silhouette

### Input
- Image: `output/images/scene_01.png`
- Duration: 3-5 seconds

### Motion Description
Camera slowly zooms in on the silhouette figure in the sandstorm. Sand particles swirl and move naturally. Atmospheric depth with parallax effect (foreground sand moves faster than background). Subtle camera shake for realism.

### Kling AI Prompt
```
Camera slowly zooms in on silhouette figure,
sand particles swirling and floating in wind,
atmospheric depth with parallax effect,
cinematic camera movement,
smooth zoom, subtle camera shake,
epic desert atmosphere,
golden hour lighting intensifying
```

### Pika Labs Approach
- Upload `scene_01.png`
- Motion: "Zoom In" (built-in)
- Prompt: "Sand particles swirling, atmospheric movement"
- Motion Strength: 3-4/10

### Runway Gen-4 Prompt
```
The camera slowly pushes in toward the silhouette.
Sand particles drift and swirl in the wind, creating atmospheric depth.
Foreground elements move faster than background (parallax).
Subtle handheld camera shake adds realism.
Golden sunlight intensifies as we move closer.
```

### Quality Acceptance Criteria
- [ ] Smooth zoom motion (no jitter)
- [ ] Sand particles move naturally
- [ ] Parallax effect visible
- [ ] Duration 3-5 seconds
- [ ] No artifacts or glitches
- [ ] Maintains image quality

### Troubleshooting
- **Issue**: Zoom too fast/abrupt
  - **Fix**: Reduce motion strength, add "slow, gradual zoom"
- **Issue**: Sand particles static
  - **Fix**: Emphasize "swirling particles, wind movement"

---

## 🏃 Scene 2: Mussoman Sprint - Side Tracking Shot

### Input
- Image: `output/images/scene_02.png`
- Duration: 4-5 seconds

### Motion Description
Side tracking shot following Mussoman as he runs. Camera pans left-to-right matching his movement. Dust kicks up behind him. Motion blur on background suggests speed. Character remains in frame center.

### Kling AI Prompt (Recommended for this scene)
```
Side tracking shot following running character,
camera pans smoothly left to right,
dust and sand particles kicked up behind,
motion blur on background suggesting speed,
character stays centered in frame,
dynamic action shot,
cinematic camera work,
heroic running motion
```

### Pika Labs Approach
- Upload `scene_02.png`
- Motion: "Pan Right" + "Character Animation"
- Prompt: "Running motion, dust trail, speed lines"
- Motion Strength: 5-6/10

### Runway Gen-4 Prompt
```
The camera tracks alongside the running character from the side,
panning smoothly to keep him centered in frame.
His legs pump powerfully, arms swing with momentum.
Dust and sand particles explode from his footfalls.
Background blurs slightly to convey speed.
Heroic, dynamic running motion.
```

### Quality Acceptance Criteria
- [ ] Smooth camera pan (no stuttering)
- [ ] Character motion looks natural
- [ ] Dust trail visible and dynamic
- [ ] Background motion blur present
- [ ] Character stays in frame
- [ ] Duration 4-5 seconds

### Troubleshooting
- **Issue**: Character looks static
  - **Fix**: Add "dynamic running motion, legs pumping, arms swinging"
- **Issue**: Camera pan too fast
  - **Fix**: Specify "smooth, steady pan matching character speed"

---

## 💪 Scene 3: Close-up Power - Slow Zoom with Intensity

### Input
- Image: `output/images/scene_03.png`
- Duration: 3-4 seconds

### Motion Description
Slow zoom in on Mussoman's face. Eyes intensify, slight head tilt upward. Rim lighting flickers slightly (energy building). Background defocus increases. Dramatic, tense moment before transformation.

### Kling AI Prompt
```
Slow zoom in on character's face,
eyes intensifying with determination,
slight upward head tilt,
rim lighting flickering with energy,
background defocus increasing,
dramatic tension building,
cinematic portrait shot,
heroic intensity
```

### Pika Labs Approach
- Upload `scene_03.png`
- Motion: "Zoom In" (slow)
- Prompt: "Intense expression, energy building, dramatic lighting"
- Motion Strength: 2-3/10 (subtle)

### Runway Gen-4 Prompt
```
The camera slowly pushes in on the character's face.
His eyes narrow with intense focus and determination.
A slight upward tilt of the head emphasizes heroism.
Rim lighting flickers subtly as energy builds around him.
The background gradually defocuses, isolating the subject.
Tension and power radiate from his expression.
```

### Quality Acceptance Criteria
- [ ] Smooth, slow zoom
- [ ] Facial expression intensifies
- [ ] Lighting effects subtle but visible
- [ ] Background defocus increases
- [ ] Duration 3-4 seconds
- [ ] Maintains facial detail

### Troubleshooting
- **Issue**: Zoom too fast
  - **Fix**: Specify "very slow, gradual zoom"
- **Issue**: Face distorts
  - **Fix**: Lower motion strength, add "maintain facial proportions"

---

## ⚡ Scene 4: TRANSFORMATION - Character to Vehicle (CRITICAL)

### Input
- Image: `output/images/scene_04.png`
- Duration: 3-5 seconds (longer if possible)

### Motion Description
**THIS IS THE MOST IMPORTANT SCENE.** Mussoman's body transforms into the Musso pickup truck. Energy effects, particle dissolution, mechanical reconfiguration. Must be visually convincing.

### Strategy (from Task 2)

**Approach 1: Pika Labs Pikaffects** ⭐ RECOMMENDED
```
Stage 1: Apply "Dissolve" or "Melt" effect
- Upload scene_04.png
- Effect: Dissolve
- Prompt: "Character dissolving into glowing energy particles"
- Duration: 2-3 seconds

Stage 2: Apply "Rebuild" or "Transform" effect
- Input: Stage 1 output
- Effect: Rebuild
- Prompt: "Energy particles reforming as pickup truck"
- Duration: 2-3 seconds

Combine both stages in CapCut for full transformation
```

**Approach 2: Kling AI Direct Transformation**
```
Anthropomorphic rhino character transforming into pickup truck,
body parts shifting and reconfiguring mechanically,
glowing energy particles swirling around,
transformer-style mechanical transformation,
panels folding and rotating,
smooth morphing transition,
cinematic transformation effect,
epic power surge
```

**Approach 3: Runway Gen-4 Detailed Transformation**
```
The rhino character's body begins to shift and reconfigure.
Mechanical panels fold outward from his torso and limbs.
Glowing energy particles swirl around the transformation.
His form gradually morphs into the shape of a pickup truck.
Metal surfaces emerge and lock into place with hydraulic movements.
The transformation is smooth yet mechanical, like a living machine.
Energy pulses through the changing form.
```

### Quality Acceptance Criteria (CRITICAL)
- [ ] Transformation visually recognizable (start = character, end = vehicle)
- [ ] Duration 2+ seconds minimum
- [ ] Visual continuity maintained
- [ ] Energy/particle effects present
- [ ] No major glitches or artifacts
- [ ] **If quality insufficient**: Proceed to Plan B (multi-clip approach)

### Plan B: Multi-Clip Transformation
If single-clip transformation fails quality check:

**Clip 4a** (2 seconds): Character powering up
- Energy building, glowing effects
- Character in transformation pose

**Clip 4b** (1-2 seconds): Transition effect (created in CapCut)
- Particle explosion
- Flash/glitch effects
- Energy burst

**Clip 4c** (2 seconds): Vehicle reveal
- Truck materializing/landing
- Dust settling
- Power dissipating

### Troubleshooting
- **Issue**: Transformation looks unnatural
  - **Fix**: Try Pika Pikaffects multi-stage approach
- **Issue**: Character features lost
  - **Fix**: Emphasize "maintaining rhino horn → truck antenna" or color continuity
- **Issue**: Too short duration
  - **Fix**: Use Pikaframes for extended duration, or Plan B multi-clip
- **Issue**: Quality unacceptable after 10+ attempts
  - **Fix**: Activate Plan B (multi-clip + CapCut effects)

---

## 🚗 Scene 5: Musso Finale - Truck Driving with Dust Trail

### Input
- Image: `output/images/scene_05.png`
- Duration: 4-5 seconds

### Motion Description
Pickup truck drives forward through desert. Camera follows from 3/4 angle. Massive dust cloud trails behind. Vehicle bounces slightly on terrain. Triumphant, powerful motion.

### Kling AI Prompt (Recommended for vehicle motion)
```
Pickup truck driving powerfully through desert,
camera following from 3/4 angle,
massive dust cloud trailing behind,
vehicle bouncing slightly on terrain,
chrome and paint gleaming in sunlight,
dynamic vehicle motion,
cinematic automotive shot,
triumphant and powerful
```

### Pika Labs Approach
- Upload `scene_05.png`
- Motion: "Move Forward" + "Camera Follow"
- Prompt: "Truck driving, dust trail, powerful motion"
- Motion Strength: 5-6/10

### Runway Gen-4 Prompt
```
The pickup truck drives forward powerfully through the desert.
The camera tracks it from a 3/4 angle, keeping it centered.
A massive dust cloud billows behind the vehicle.
The truck bounces slightly as it navigates the terrain.
Chrome details and paint gleam in the golden sunlight.
The motion conveys power and triumph.
```

### Quality Acceptance Criteria
- [ ] Truck motion looks realistic
- [ ] Dust trail dynamic and prominent
- [ ] Camera tracking smooth
- [ ] Vehicle stays in frame
- [ ] Duration 4-5 seconds
- [ ] Lighting consistent with Scene 1

### Troubleshooting
- **Issue**: Truck looks static
  - **Fix**: Emphasize "driving forward, wheels turning, suspension moving"
- **Issue**: Dust trail weak
  - **Fix**: Add "massive dust cloud, sand explosion, dramatic trail"

---

## 🎨 General Prompting Best Practices

### Motion Keywords
- **Camera**: "zoom in/out", "pan left/right", "track", "orbit", "push in", "pull back"
- **Speed**: "slow", "gradual", "smooth", "dynamic", "fast"
- **Effects**: "motion blur", "parallax", "depth", "atmospheric"

### Quality Modifiers
- "cinematic camera work"
- "smooth motion"
- "professional cinematography"
- "no jitter or stuttering"

### Negative Prompts (if supported)
```
static, frozen, jittery, glitchy, distorted,
low quality, blurry, artifacts, watermark
```

---

## 📊 Quality Control Process

### Per-Clip Verification
```bash
# Check file exists
ls -la output/videos/scene_01.mp4

# Check duration (should be 3-5 seconds)
ffprobe -v error -show_entries format=duration -of csv=p=0 output/videos/scene_01.mp4

# Check resolution
ffprobe -v error -select_streams v:0 -show_entries stream=width,height -of csv=p=0 output/videos/scene_01.mp4
```

### Visual Quality Checklist
- [ ] Smooth motion (no stuttering)
- [ ] No visible artifacts or glitches
- [ ] Maintains image quality from Task 3
- [ ] Motion matches intended description
- [ ] Duration within 3-5 second range
- [ ] File format compatible with CapCut (MP4/MOV)

### Iteration Strategy
- Generate 2-3 versions per scene
- Select best based on:
  - Motion smoothness
  - Visual quality
  - Adherence to prompt
  - Duration appropriateness

---

## 📁 File Management

### Directory Structure
```
output/
├── videos/
│   ├── scene_01_v1.mp4
│   ├── scene_01_v2.mp4
│   ├── scene_01.mp4          ← Final selection
│   ├── scene_02_v1.mp4
│   ├── scene_02_v2.mp4
│   ├── scene_02.mp4          ← Final selection
│   ├── ... (scenes 3-5)
│   ├── transformation.mp4     ← Scene 4 final (or multi-clip)
│   └── metadata.txt          ← Prompts and settings used
```

### Metadata Tracking
Create `output/videos/metadata.txt`:
```
Scene 1: [tool used] | [prompt] | [settings] | Selected: v2
Scene 2: [tool used] | [prompt] | [settings] | Selected: v1
Scene 4: [approach used] | [notes on quality] | Plan B: Yes/No
...
```

---

## ⏱️ Execution Timeline

| Phase | Duration | Activity |
|-------|----------|----------|
| Setup | 10 min | Review images, select tool, prepare prompts |
| Scene 1 | 30 min | Generate 2-3 versions, select best |
| Scene 2 | 40 min | Generate 2-3 versions, select best |
| Scene 3 | 30 min | Generate 2-3 versions, select best |
| **Scene 4** | **90-120 min** | **Transformation (multiple attempts expected)** |
| Scene 5 | 40 min | Generate 2-3 versions, select best |
| QC | 20 min | Review all clips, verify quality |
| **Total** | **4-6 hours** | Including iteration and quality control |

**Note**: Scene 4 (transformation) allocated extra time due to complexity and importance.

---

## 🚨 Critical Success Factors

### Scene 4 (Transformation) is Make-or-Break
- **Budget 90-120 minutes** for this scene alone
- **Try multiple approaches** if first doesn't work
- **Don't settle for poor quality** - this is the video's climax
- **Activate Plan B** if quality unacceptable after 10+ attempts

### Free Tier Credit Management
- **Kling AI**: ~66 credits free (each video ~6-10 credits)
- **Pika Labs**: ~30 credits free (each video ~3-5 credits)
- **Runway Gen-4**: ~125 credits free (each video ~10-15 credits)

**Strategy**: Use free credits for Scenes 1-3, 5. Reserve paid option for Scene 4 if needed.

---

## 🔧 Troubleshooting Guide

### Common Issues Across All Scenes

**Issue**: Motion too subtle/barely visible
- **Solution**: Increase motion strength, add "dynamic, pronounced movement"

**Issue**: Motion too extreme/unrealistic
- **Solution**: Decrease motion strength, add "smooth, natural, realistic"

**Issue**: Video quality degraded from image
- **Solution**: Use highest quality settings, try different tool

**Issue**: Duration too short
- **Solution**: Request longer duration, use Pikaframes, or generate multiple clips to combine

**Issue**: Watermarks visible
- **Solution**: Ensure using paid/credited account, not free trial

### Scene-Specific Issues

**Scene 1**: Sand looks static
- Add "swirling particles, wind movement, atmospheric motion"

**Scene 2**: Character looks frozen
- Add "running legs, pumping arms, dynamic motion"

**Scene 4**: Transformation unconvincing
- Try Pika Pikaffects multi-stage
- Try Runway with detailed mechanical description
- Activate Plan B if quality insufficient

**Scene 5**: Truck looks static
- Add "wheels turning, suspension bouncing, forward motion"

---

## 🚀 Next Steps

After completing Task 4:
1. Verify all 5 video clips meet quality criteria
2. **Special attention**: Verify Scene 4 transformation is acceptable
3. Update notepad: `.sisyphus/notepads/mussoman-ai-video/learnings.md`
4. Proceed to Task 6: Video Editing (combine clips + BGM + subtitles)

---

## 📚 Reference Materials

- **Transformation Strategy**: `output/strategy/transformation_strategy.md` (detailed approaches)
- **Source Images**: `output/images/scene_*.png` (Task 3 outputs)
- **BGM**: `output/audio/bgm_selected.mp3` (for reference timing)
- **Brand Philosophy**: "Powered by Toughness"

---

**Document Version**: 1.0  
**Last Updated**: 2026-01-29  
**Status**: READY FOR EXECUTION (awaiting Task 3 completion)
