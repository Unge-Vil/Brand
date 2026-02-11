# Brand System Specification: Unge Vil

**Version:** 1.7 ALPHA **Status:** Work in Progress **Last Updated:** Feb 2026

## 1. Core Identity

-   **Name:** Unge Vil
    
-   **Tone of Voice:** Ungdommelig, men profesjonell. Inkluderende, energisk og strukturert.
    
-   **Role:** Barne- og ungdomsorganisasjon. Fasilitator for unges ideer.
    
-   **Mission:** Skape åpne, gratis møteplasser og bygge lokal bærekraft gjennom ung medvirkning.
    

## 2. Color Palette & Harmony

Our palette uses a split-complementary harmony. **Purple** (Creativity) and **Gold** (Energy) provide high contrast, while **Teal** (Structure/Nature) grounds the system.

### A. Unge Vil (Main Brand)

_Playful, Inclusive, Creative._

Token Name

HEX

Tailwind Class

Usage

**Primary Purple**

`#9333EA`

`purple-600`

Hovedfarge, knapper, highlights.

**Creative Coral**

`#FB7185`

`rose-400`

Sekundærfarge for myke/kreative elementer.

**Background Tint**

`#FBF7FF`

N/A

Lys lilla bakgrunn (Section backgrounds).

### B. ATLAS (System Brand)

_Professional, Structured, Public Sector Friendly._

Token Name

HEX

Tailwind Class

Usage

**Atlas Dark**

`#0F172A`

`slate-900`

Primærfarge (Slate/Navy). Profesjonell base.

**Atlas Base**

`#334155`

`slate-700`

Sekundær/Border farge.

**Atlas Teal**

`#0D9488`

`teal-600`

Aksentfarge (Vekst/Struktur/Balanse).

**Atlas Light**

`#F1F5F9`

`slate-100`

Bakgrunnsfarge for dokumentasjon.

### C. Create A Spark (Energy Brand)

_High Voltage, Innovation, Speed._

Token Name

HEX

Tailwind Class

Usage

**Spark Gold**

`#FBBF24`

`amber-400`

Primærfarge (Energi/Lys).

**Gold Dark**

`#F59E0B`

`amber-500`

Gradient end-stop / Hover states.

**Void Black**

`#000000`

`black`

Bakgrunn for maksimal kontrast.

**Spark Gradient**

`#FBBF24` -> `#F59E0B`

Linear gradient (135deg).

## 3. Typography

**Primary Font Family:** `Inter` (Google Fonts) **Fallback Font:** `Arial`, sans-serif (For Google Docs/System default)

### Type Scale & Weights

-   **Headlines (Display):** Inter Black (`font-weight: 900`). Tracking: Tighter (`-0.05em`).
    
-   **Subheadlines:** Inter Bold (`font-weight: 700`).
    
-   **Body Text:** Inter Regular (`font-weight: 400`). Line-height: `1.5` or `1.6`.
    
-   **Spark Headline:** Inter Black Italic (`font-weight: 900`, `font-style: italic`). Used for high-impact statements.
    

## 4. Logo & Assets

### Files

-   `UngeVil-dark-line.png`: Mørk logo (tekst + ikon). Brukes på lyse bakgrunner.
    
-   `UngeVil-light-line.png`: Lys logo (tekst + ikon). Brukes på mørke/fargede bakgrunner.
    
-   `favicon.png`: Ikon alene. Brukes som profilbilde eller der plassen er kvadratisk.
    

### Usage Rules

-   **Contrast:** Sørg alltid for WCAG AA kontrast.
    
-   **Brand Background:** På lilla bakgrunn (`#9333EA`), bruk `UngeVil-light-line.png` med CSS-filter `brightness(0) invert(1)` for å tvinge logoen til å bli 100% hvit (dersom lilla elementer krasjer med bakgrunnen).
    

## 5. Iconography

**Library:** [Lucide Icons](https://lucide.dev/ "null")

**Style Guidelines:**

-   **Stroke Width:** 2px (Consistent)
    
-   **Corners:** Rounded (Line caps/joins: round)
    
-   **Color:** Matcher konteksten (Lilla for Unge Vil, Teal for Atlas, Gull for Spark).
    

**Key Icons:**

-   `users`, `heart`, `smile` (Community)
    
-   `zap`, `lightbulb`, `monitor` (Gaming/Spark/IdéLab)
    
-   `layout-template`, `clipboard-check`, `building-2`, `book` (ATLAS/Structure)
    

## 6. Sub-Brands & Implementation

### A. ATLAS-modellen (System & Struktur)

**Konsept:** Navigasjon, kartlegging, økosystem. ATLAS er dokumentasjonen og "operativsystemet". **Context:** Hosted on GitBook.

**Core Modules:**

1.  **Blanke Ark:** Behovskartlegging uten føringer. (Icon: `book-open`)
    
2.  **Gi det videre:** Ung-til-ung læring og bærekraft. (Icon: `hand-metal` / `repeat`)
    
3.  **IdéLab:** Verkstedmetodikk for idéutvikling. (Icon: `lightbulb`)
    
4.  **Forståelse:** Rammeverk og kontekst. (Icon: `puzzle` / `brain`)
    

**Visual Style:**

-   **Aesthetic:** Clean, documentation-focused, blueprint feeling.
    
-   **Patterns:** Grids, dashed lines, timelines.
    
-   **Motion:** Presis, flytende, logisk (`ease-out`).
    

### B. Create A Spark (Energi & Innovasjon)

**Konsept:** Gnisten. Startfasen. Rask, uredd og energisk.

**Naming Convention:**

-   **Global Concept:** "Create A Spark"
    
-   **Local Venue:** "Kollektivet [Stedsnavn]" (e.g., _Kollektivet Haugalandet_).
    

**Elements:**

-   **IdéLab Deck:** Firkantet kortstokk brukt i workshops. Symbol: Lysende pære.
    
-   **Visual Style:** High contrast (Black/Gold), Stickers, "Hazard tape" patterns, Noise textures.
    
-   **Motion:** Rask, snappy, elektrisk (`ease-out-expo` / `spring`).
    

## 7. Brand Cohesion: "Powered by..."

Selv om sub-brands har sterke egne identiteter, må de knyttes til moderskipet.

**Regler:**

1.  **Typography:** Alle brands bruker **Inter** som base.
    
2.  **Logo Presence:** Unge Vil-logoen skal alltid være tilstede som avsender.
    
    -   **Nettsider:** I footer eller som "tag" i hjørnet.
        
    -   **Print:** Nederst på plakater/rollups med teksten "Et tilbud fra" eller "Powered by".
        
3.  **Cross-linking:** Farger kan lånes på tvers som små aksenter (f.eks. en lilla knapp på en Atlas-side) for å vise slektskap.
    

## 8. Web Design Tokens

For utviklere og designere.

### A. Border Radius

-   **Buttons:** `rounded-full` (Pill shape).
    
-   **Cards (Large):** `rounded-[2rem]` (32px) - Soft and friendly.
    
-   **Cards (Small):** `rounded-xl` (12px).
    
-   **Spark Exception:** Kan bruke skarpere hjørner eller roterte elementer for effekt.
    

### B. Shadows

-   **Light Mode:** `box-shadow: 0 10px 40px -10px rgba(147, 51, 234, 0.15);` (Purple tint).
    
-   **Dark Mode:** Subtle borders (`1px solid rgba(255,255,255,0.1)`) instead of drop shadows.
    

### C. Spacing

-   **Generous:** Bruk mye luft (`p-8`, `p-12`) for å unngå rot.
    

## 9. Canva & Graphics Guidelines

Tips for ikke-designere som lager innhold.

### Søkeord i Canva (Keywords)

-   **Unge Vil:** `Organic shapes`, `Soft gradient`, `Doodle line`, `Minimalist`.
    
-   **Create A Spark:** `Grunge texture`, `Tape`, `Sticker`, `Distorted`, `Grainy gradient`.
    
-   **ATLAS:** `Geometric grid`, `Technical line`, `Blueprint`, `Isometric`.
    

### Emoji-bruk

-   Bruk standard Apple/iOS emojis for et "folkelig" og rent uttrykk.
    
-   Unngå 3D-renderte "clay"-emojis som krasjer med stilen.
    
-   Bruk emojis som punktmerking eller reaksjoner, ikke som hovedbilde.
    

### Former

-   **Unge Vil:** Runde, myke former.
    
-   **Spark:** Skarpe kanter, stjerner, lyn, "eksplosjoner".
    
-   **ATLAS:** Rektangler, linjer, koblinger.
    

## 10. Social Media Presence

**Story Templates:**

1.  **Event Promo:** Bilde i bakgrunn (sorthvitt eller farget), stor typografi, "Link i bio"-sticker.
    
2.  **Q&A / Interaksjon:** Lilla bakgrunn, spørsmålsboks, emojier.
    
3.  **Takeover / Behind the scenes:** Råbilder/video med sort overlay og hvit tekst. "Tag" personen som har takeover.
    
4.  **Sitat:** Hvit bakgrunn, lilla sitattegn, stor sort tekst.
    

## 11. CSS Utility Classes (Reference)

```
/* Unge Vil */
.bg-brand { background-color: #9333EA; }
.text-brand { color: #9333EA; }
.font-display { font-family: 'Inter', sans-serif; font-weight: 900; letter-spacing: -0.05em; }

/* Atlas */
.atlas-theme { @apply bg-[#0F172A] text-white; }
.atlas-accent { @apply text-[#0D9488]; }
.atlas-card { @apply bg-white/5 backdrop-blur-md border border-white/10; }

/* Spark */
.spark-theme { @apply bg-black text-[#FBBF24]; }
.spark-font { @apply font-black italic; }
.spark-gradient { background: linear-gradient(135deg, #FBBF24 0%, #F59E0B 100%); }

```
