# Build Your AI Digital Twin in 20 Minutes — No Code, No Studio, No Crew

Your face, your lighting, your brand — locked into AI. No model training, no GPU. Just a persistent identity system that makes every generation look like you.

---

## What is an AI Digital Twin?

Not a deepfake. Not a LoRA model. A digital twin is a persistent actor profile — your skin tone hex code, your exact eye shape, your signature accessories, the way light hits your face. Every prompt starts with YOUR visual DNA.

Think of it like this: instead of training a model on photos of you ($2/image, locked to one provider, takes hours), you create a text-based identity card that works everywhere. One file. Infinite generations. Portable across any AI platform.

### LoRA Training vs. Digital Twin

| | LoRA Training | Digital Twin |
|---|---|---|
| Cost | $2+ per image | Free |
| Setup time | Hours | 20 minutes |
| Technical skill | High (GPU, training) | None (plain English) |
| Portability | Locked to one model | Works with any AI tool |
| Control | Retrain for changes | Edit a text file |
| Consistency | Good for one angle | Good across scenarios |

---

## Step 1: Install Claude Code

Open your terminal and run one command:

```
npm install -g @anthropic-ai/claude-code
```

Then launch it:

```
claude
```

That's it. No accounts, no API keys needed for this part.

---

## Step 2: Install the Skill

Download the ZIP from the link at the bottom of this page. Extract it and copy the `ugc-creator` folder:

```
cp -r ugc-creator ~/.claude/skills/ugc-creator
```

Verify it's working — type this into Claude Code:

```
show roster
```

You should see three starter actors: Marcus (real estate), Priya (finance), and Jess (fitness).

---

## Step 3: Create Your Twin

Tell Claude Code:

```
create actor
```

It'll interview you about your appearance. The more specific you are, the more consistent your generations will be. Here's what it asks for:

**Face lock fields:**
- Skin tone hex code (use a color picker on a photo of yourself)
- Eye color, shape, and distinctive features
- Hair color, texture, length, and style
- Jawline shape
- Nose shape
- Lip shape and natural color
- Distinguishing marks (beauty marks, freckles, scars, dimples)
- Signature accessory (something you always wear)

**Body:**
- Build description
- Height impression

**Outfits:**
- Casual/home look
- Going out look
- Workout look
- Glam/professional look

**The prompt seed:** All of the above compressed into one dense paragraph. This is what gets injected into every single generation prompt. It's the most important field.

### Example: Real Estate Agent Profile

Here's what Marcus's prompt seed looks like:

> "34 year old African American man, polished professional energy. Black hair in tight coils with clean low fade and sharp lineup. Rich brown skin #8D5524, clean matte finish. Wide-set dark brown eyes, slightly hooded with direct confident gaze. Broad nose with rounded tip. Full natural lips. Small mole above right eyebrow, faint laugh lines at mouth corners, slight left dimple when smiling. Silver TAG Heuer watch on left wrist, thin silver wedding band (always). Athletic build, broad shoulders. Charcoal blazer over white crew-neck tee."

Every generation for Marcus starts with this paragraph, verbatim. That's why his face stays locked.

---

## Step 4: Your First Generation

Once your actor exists, give it a scenario:

```
Marcus reviewing a property listing at a modern kitchen island, golden hour light through floor-to-ceiling windows
```

The skill builds a 6-layer prompt automatically:

1. **Character Lock** — Your prompt seed (injected first, always)
2. **Scenario** — What you're doing, expressions, hand positions
3. **Environment** — Where you are, background objects, time of day
4. **Camera Profile** — Selfie front cam, rear cam, mirror selfie, or overhead
5. **Realism Injection** — 10 anchors that make AI output look like a real phone photo
6. **Anti-Patterns** — What to avoid (plastic skin, symmetrical face, studio lighting)

Copy the output into Higgsfield, Midjourney, or any image/video AI tool.

---

## Step 5: Multi-Shot Consistency

Same actor, 5 scenarios. Watch how the face, outfit, lighting, and accessories stay locked:

1. Kitchen island, reviewing listing documents
2. Standing in front of a sold sign, confident smile
3. Sitting in a luxury car, calling a client
4. Home office, recording a market update video
5. Coffee shop, casual meeting with a buyer

Same person across all five. That's the point.

---

## Step 6: Niche Prompts — Copy and Use

### Real Estate (5 prompts)

1. "Marcus standing in front of a modern home's entrance, holding a tablet showing a listing, warm afternoon light, slight smile, front cam selfie angle"
2. "Marcus at a polished conference table, reviewing contracts with a client sitting across, professional lighting, rear cam perspective"
3. "Marcus walking through an empty staged living room, gesturing toward features, natural window light, slight head turn"
4. "Marcus in his car after a showing, talking to camera about the market, dashboard visible, selfie front cam"
5. "Marcus at a neighborhood coffee shop, casual blazer, laptop open, chatting with a young couple about first-time buying"

### Financial Advisory (5 prompts)

1. "Priya at a clean white desk, explaining a chart on her laptop screen to camera, warm office light, front cam angle"
2. "Priya holding a notebook, walking the viewer through a budget breakdown, seated in a modern home office, natural light"
3. "Priya on a video call setup, ring light reflection in her eyes, professional but warm expression, discussing retirement planning"
4. "Priya at a cafe, casual outfit, laptop open, working on a client financial plan, candid lifestyle shot"
5. "Priya in her office, standing at a whiteboard with simple financial diagrams, teaching posture, rear cam perspective"

### Fitness Coaching (5 prompts)

1. "Jess demonstrating a resistance band shoulder exercise in a bright gym, coral sports bra, energetic expression, rear cam angle"
2. "Jess in her kitchen, making a protein smoothie, blender and ingredients on counter, morning light, front cam selfie"
3. "Jess sitting on a yoga mat, post-workout, talking to camera about recovery, slight sweat, natural glow, selfie angle"
4. "Jess in a park, showing a bodyweight squat form, athletic wear, golden hour, someone filming her from waist level"
5. "Jess in her car post-gym, hair in messy bun, talking about today's workout, dashboard and gym bag visible, front cam"

---

## What's Next

This is the foundation. Once your digital twin is locked:

- **Voice cloning** — Clone your speaking voice and pair it with your visual twin for talking head videos
- **Automated pipelines** — Generate a week of content in one batch, hands-free
- **Performance feedback loops** — Track what performs, automatically generate more of what works

I'm building all of this. Reply to the email that brought you here for 1-on-1 help getting set up.

---

## Download the Starter Kit

The ZIP includes:
- Full UGC Creator skill
- Camera profiles, realism anchors, anti-patterns
- Blank actor template
- 3 niche starter profiles (real estate, finance, fitness)
- README with setup instructions

**[Download ZIP]** ← (attach link here)

---

Built by Jerel | [jerelai.netlify.app](https://jerelai.netlify.app)
