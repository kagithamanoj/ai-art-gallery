# Stable Diffusion & DALL-E Prompt Engineering Guide

## Prompt Anatomy

A great AI art prompt has 5 components:

```
[Subject] + [Style] + [Medium] + [Lighting] + [Quality Modifiers]
```

### Example
```
A cyberpunk samurai standing on a neon-lit rooftop in Tokyo, 
digital art, concept art style, 
dramatic cinematic lighting with purple and cyan neons,
highly detailed, 8K, artstation trending
```

## Prompt Formulas

### 1. Portrait Formula
```
[Adjective] portrait of [subject], [art style], [lighting], 
[camera details], [quality modifiers]
```
**Example**: `Ethereal portrait of a young scientist, oil painting style, Rembrandt lighting, shallow depth of field, masterpiece, ultra-detailed`

### 2. Landscape Formula
```
[Environment type] [time of day], [art style], [mood], 
[atmospheric effects], [quality]
```
**Example**: `Vast alien desert at golden hour, Studio Ghibli style, serene and mysterious, volumetric fog, cinematic composition, 8K wallpaper`

### 3. Character Design Formula
```
[Character archetype] [action/pose], [clothing/armor details], 
[art style], [background], [quality]
```
**Example**: `Futuristic bounty hunter reloading weapon, matte black tactical suit with glowing blue accents, cyberpunk art, dark industrial backdrop, concept art, trending on artstation`

### 4. Architecture Formula
```
[Building type] [architectural style] [setting], 
[time/weather], [rendering style], [quality]
```
**Example**: `Ancient temple built into a cliff face, Mayan-Japanese fusion architecture, jungle setting at sunrise, ray-traced rendering, hyper-realistic, 4K`

## Style Keywords

### Art Styles
| Keyword | Effect |
|---------|--------|
| `oil painting` | Rich textures, classical feel |
| `watercolor` | Soft, flowing, translucent |
| `digital art` | Clean, modern, vibrant |
| `concept art` | Professional, game/film quality |
| `anime` | Japanese animation style |
| `photorealistic` | Looks like a photograph |
| `pixel art` | Retro, 8-bit aesthetic |
| `vector art` | Clean lines, flat colors |
| `vaporwave` | 80s aesthetics, neon, nostalgia |
| `art nouveau` | Organic forms, ornate decoration |

### Lighting Keywords
| Keyword | Effect |
|---------|--------|
| `dramatic lighting` | High contrast, cinematic shadows |
| `volumetric lighting` | God rays, atmospheric depth |
| `Rembrandt lighting` | Classic portrait lighting |
| `golden hour` | Warm, magical sunset light |
| `neon lighting` | Cyberpunk, colorful glow |
| `studio lighting` | Clean, professional, even |
| `rim lighting` | Edge-lit subject, dramatic separation |
| `bioluminescent` | Organic glowing light |

### Quality Modifiers
```
highly detailed, 8K, ultra HD, masterpiece, best quality,
sharp focus, intricate details, professional, award-winning,
trending on artstation, cinematic, photorealistic
```

### Negative Prompts (what to exclude)
```
blurry, low quality, deformed, ugly, bad anatomy, 
bad proportions, duplicate, watermark, text, 
extra fingers, mutated hands, poorly drawn face
```

## Model-Specific Tips

### DALL-E 3
- Understands natural language well — be descriptive
- Specify aspect ratio: "wide format", "square", "portrait"
- Works great with: artistic styles, character design, logos

### Stable Diffusion (SDXL)
- Responds better to comma-separated keyword lists
- Negative prompts are critical
- Use CFG scale 7-12 for best results
- Samplers: DPM++ 2M Karras (fast), Euler a (creative)

### Midjourney
- Add `--ar 16:9` for aspect ratio
- Add `--v 6.1` for latest version
- Separate with `::` for weight control: `cat::2 hat::1`
