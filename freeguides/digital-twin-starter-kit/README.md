# AI Digital Twin Starter Kit

Build a persistent AI version of yourself for content generation. No model training, no GPU, no code.

## What's inside

```
ugc-creator/
  SKILL.md              ← The full UGC Creator skill (install this)
  references/           ← Camera profiles, realism anchors, anti-patterns, background kits
  actors/
    _template.json      ← Blank actor template — fill in your details
    real-estate-agent.json   ← Marcus — ready-to-use real estate profile
    financial-advisor.json   ← Priya — ready-to-use finance profile
    fitness-coach.json       ← Jess — ready-to-use fitness profile
```

## Setup (3 steps, ~5 minutes)

### 1. Install Claude Code

Open your terminal and run:

```bash
npm install -g @anthropic-ai/claude-code
```

Then launch it:

```bash
claude
```

### 2. Install the skill

Copy the `ugc-creator` folder to your Claude Code skills directory:

```bash
cp -r ugc-creator ~/.claude/skills/ugc-creator
```

Verify it works — open Claude Code and type:

```
show roster
```

You should see the three starter actors listed.

### 3. Create your digital twin

Tell Claude Code:

```
create actor
```

It will interview you about your appearance — skin tone, eye shape, hair, signature accessories, distinguishing marks. Be specific. The more detail you give, the more consistent your generations will be.

Or duplicate `_template.json`, fill it in manually, and save it as `your-name.json` in the actors folder.

## Your first generation

Once your actor exists, try:

```
Marcus reviewing a property listing at a modern kitchen island, golden hour light
```

```
Priya explaining compound interest on a video call, home office background
```

```
Jess demonstrating a resistance band exercise in a bright gym
```

The skill builds a 6-layer prompt: character lock → scenario → environment → camera profile → realism injection → anti-patterns. Copy the output into Higgsfield (or any image/video AI tool).

## Multi-shot consistency

Generate 5 different scenarios with the same actor. The identity card keeps face, outfit, lighting, and accessories locked across all of them. No drift.

## Customize a starter profile

1. Open any `.json` file in the `actors/` folder
2. Change the fields to match your look
3. Rewrite the `prompt_seed` paragraph — this is what gets injected into every prompt
4. Save and generate

The `prompt_seed` is the most important field. It's one dense paragraph with every visual identifier: age, ethnicity, hair, skin hex code, eyes, nose, lips, distinguishing marks, signature accessories, build.

## Questions?

Reply to the email that brought you here — I read every one.

Built by Jerel — [jerelai.netlify.app](https://jerelai.netlify.app)
