SYSTEM CONTEXT: UNGE VIL BRAND IDENTITY

Version: 2.0 BETA
Role: Master Source of Truth for Design & Development
Usage: Provide this file to AI agents to ensure strict adherence to the brand guidelines.

1. ORGANIZATIONAL DNA

Mission & Vision

Core Purpose: Forebygge utenforskap og styrke sosial/mental helse gjennom inkludering, mestring og lokal bærekraft.

Operating Model: "Ungdomsdrevet innhold – voksenforankret styring."

Key Values: Samarbeid, Ressursdeling, Inkludering, Medvirkning, Mestring.

Tone of Voice (Copywriting Guide)

Generelt (Unge Vil): Inkluderende, varm, tydelig, men aldri "ovenfra-og-ned". Vi bruker et språk som treffer ungdom, men som oppleves trygt for voksne/kommuner.

ATLAS (System): Profesjonell, metodisk, presis. Bruk begreper som "økosystem", "ressursdeling", "verktøy". Unngå "buzzwords" uten substans.

Create A Spark (Energy): Korte setninger. Imperativ form ("Gjør det", "Start nå"). Energisk, uredd, "hype". Bruk gjerne CAPS for effekt.

2. BRAND ARCHITECTURE & HIERARCHY

We operate with a "House of Brands" structure tied together by a common visual DNA.

A. Unge Vil (The Mother Brand)

Role: The organization, the safe harbor, the sender.

Visual Key: Soft, round, welcoming. Purple & Coral.

B. ATLAS-modellen (The Methodology)

Role: The tool for municipalities and partners. Structure, documentation, system.

Visual Key: Technical, grid-based, modular. Slate & Teal.

C. Create A Spark (The Youth Brand)

Role: Innovation lab, workshops, creative explosion. Also known locally as "Kollektivet".

Visual Key: High contrast, chaotic energy, stickers. Black & Gold.

3. DESIGN TOKENS (VISUAL LANGUAGE)

Color Palette (Tailwind CSS Map)

Scope

Token Name

HEX

Tailwind

Usage

Main

brand-purple

#9333EA

purple-600

Primary action, brand background.

Main

brand-dark

#7E22CE

purple-700

Hover states.

Main

brand-coral

#FB7185

rose-400

Creative accents, warmth.

Main

bg-tint

#FBF7FF

N/A

Light section backgrounds.

Atlas

atlas-dark

#0F172A

slate-900

Professional backgrounds/text.

Atlas

atlas-base

#334155

slate-700

Borders, secondary text.

Atlas

atlas-teal

#0D9488

teal-600

Success, growth, balance accents.

Spark

spark-gold

#FBBF24

amber-400

Energy, highlights, stickers.

Spark

spark-black

#000000

black

Backgrounds for maximum contrast.

Gradient Token:

spark-gradient: linear-gradient(135deg, #FBBF24 0%, #F59E0B 100%)

Typography System

Font Family: Inter (Google Fonts).
Fallback: Arial, sans-serif.

Usage

Weight

Style

Tracking

Case

Logo/Hero

900 (Black)

Normal

-0.05em

Mixed or Uppercase

Headlines

900 (Black)

Normal

-0.02em

Sentence

Spark Hero

900 (Black)

Italic

-0.02em

UPPERCASE

Subheads

700 (Bold)

Normal

0

Sentence

UI Labels

600 (SemiBold)

Normal

0.05em

UPPERCASE

Body

400 (Regular)

Normal

0

Sentence

Iconography (Lucide Icons)

Stroke: 2px constant width.

Cap/Join: Round.

Style: Minimalist outline. Never filled (unless active state).

4. UI & WEB IMPLEMENTATION GUIDE

Border Radius (Corner Rounding)

Unge Vil (Default): rounded-[2rem] (32px) for large containers. Very friendly.

Buttons: rounded-full (Pill). Always.

Atlas: rounded-xl (12px). More precise/technical.

Spark: rounded-lg (8px) or mixed with rounded-none.

Shadows & Depth

Light Mode: Soft, colored shadows. box-shadow: 0 10px 40px -10px rgba(147, 51, 234, 0.15);

Atlas Mode: Glassmorphism. bg-white/5 backdrop-blur-md border border-white/10.

Spark Mode: Hard drop shadows or glows. box-shadow: 0 0 20px rgba(251, 191, 36, 0.3);

Logo Construction on Web

Always use the text-based wordmark in HTML when possible for accessibility/SEO, or the SVG asset.

<!-- Main Logo Concept -->
<div class="font-black tracking-tighter text-4xl">
  <span class="text-gray-900 dark:text-white">UNGE</span><span class="text-[#9333EA]">VIL</span>
</div>


5. SUB-BRAND SPECIFICS

ATLAS-modellen

Keywords: System, Structure, Blueprint, Navigation.

Modules (Content):

Blanke Ark (Need analysis)

Gi det videre (Peer-learning)

IdéLab (Workshop)

Forståelse (Context)

Visual Assets: Use generic "Blueprint Grids" as backgrounds. Use dashed lines to show connections.

Create A Spark

Keywords: Energy, Speed, Raw, Workshop.

Alias: "Kollektivet [Stedsnavn]" (e.g. Kollektivet Haugalandet).

Key Asset: IdéLab Deck. A physical deck of square cards used in workshops. Icon: Glowing lightbulb.

Visual Assets: "Hazard Tape" patterns, Noise textures, Stickers (rotated -5 to 5 degrees).

6. PROMPTING GUIDE FOR AI GENERATION

Use these prompts when asking an AI to generate assets for Unge Vil.

For Unge Vil Images:

"Minimalist 3D render or flat illustration, soft rounded shapes, purple and coral gradient lighting, friendly and inclusive atmosphere, white background, high key."

For Spark Images:

"Gritty urban aesthetic, high contrast black and yellow, stickers, tape textures, motion blur, bold typography, energetic, spark particles, dark mode."

For Atlas Images:

"Isometric grid, blueprint style, clean lines, teal and navy blue, data visualization, connected nodes, structured, professional, white or dark slate background."
