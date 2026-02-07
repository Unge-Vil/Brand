# Brand System Specification: Unge Vil

**Version:** 0.9 ALPHA **Status:** Work in Progress **Last Updated:** Feb 2026

## 1. Core Identity

**Name:** Unge Vil **Tone of Voice:** Ungdommelig, men profesjonell. Inkluderende, energisk og strukturert. **Role:** Barne- og ungdomsorganisasjon. Fasilitator for unges ideer.

## 2. Color Palette (Tailwind CSS Config)

Alle farger er definert for bruk i både Light Mode og Dark Mode.

### Primary Colors

**Token Name**

**HEX**

**Tailwind Class (Approx)**

**Usage**

**Primary Purple**

`#9333EA`

`purple-600`

Hovedfarge, knapper, highlights, brand-bakgrunner.

**Primary Dark**

`#7E22CE`

`purple-700`

Hover-states, dypere kontraster.

**Background Tint**

`#FBF7FF`

N/A

Lys bakgrunn i seksjoner (Light Mode).

### Secondary / Functional Palette

**Token Name**

**HEX**

**Tailwind Class**

**Usage**

**Deep Navy**

`#1E1B4B`

`indigo-950`

Tekst (mørk), footer, ATLAS primærfarge.

**ATLAS Mint**

`#2DD4BF`

`teal-400`

Aksent for ATLAS-modellen, navigasjon, vekst.

**Spark Gold**

`#FBBF24`

`amber-400`

Aksent for "Create A Spark", energi, advarsler.

**Creative Coral**

`#FB7185`

`rose-400`

Kreative elementer, kultur, lek.

### Semantic Colors

-   **Text (Light Mode):** `#1F2937` (Gray-800) or `#111827` (Gray-900)
    
-   **Text (Dark Mode):** `#F3F4F6` (Gray-100) or `#FFFFFF` (White)
    
-   **Background (Light):** `#FFFFFF` (White) or `#F9FAFB` (Gray-50)
    
-   **Background (Dark):** `#030712` (Gray-950) or `#111827` (Gray-900)
    

## 3. Typography

**Primary Font Family:** `Inter` (Google Fonts) **Fallback Font:** `Arial`, sans-serif

### Type Scale & Weights

-   **Headlines (Display):** Inter Black (`font-weight: 900`). Tracking: Tighter (`-0.05em`).
    
-   **Subheadlines:** Inter Bold (`font-weight: 700`).
    
-   **Body Text:** Inter Regular (`font-weight: 400`). Line-height: `1.5` or `1.6`.
    
-   **UI Labels / Buttons:** Inter SemiBold (`font-weight: 600`). Uppercase tracking: `0.05em`.
    

## 4. Logo & Assets

### Files

-   `UngeVil-dark-line.png`: Mørk logo (tekst + ikon). Brukes på lyse bakgrunner.
    
-   `UngeVil-light-line.png`: Lys logo (tekst + ikon). Brukes på mørke/fargede bakgrunner.
    
-   `favicon.png`: Ikon alene. Brukes som profilbilde eller der plassen er kvadratisk.
    

### Usage Rules

-   **Contrast:** Sørg alltid for WCAG AA kontrast.
    
-   **Brand Background:** På lilla bakgrunn (`#9333EA`), bruk `UngeVil-light-line.png`.
    
    -   **Viktig:** Hvis logoen inneholder lilla elementer som "forsvinner" mot lilla bakgrunn, bruk CSS-filter: `brightness(0) invert(1)` for å tvinge logoen til å bli 100% hvit.
        

## 5. Iconography

**Library:** [Lucide Icons](https://lucide.dev/ "null")

**Style:**

-   **Stroke Width:** 2px (Consistent)
    
-   **Corners:** Rounded (Line caps/joins: round)
    
-   **Color:** Matcher konteksten (f.eks. Mint for tech/atlas, Gold for energi).
    

**Common Icons:**

-   `users`, `heart`, `smile` (Community)
    
-   `zap`, `gamepad-2`, `monitor` (Gaming/Spark)
    
-   `map`, `compass`, `anchor`, `layers` (ATLAS/Structure)
    

## 6. Sub-Brands & Motion Principles

Her defineres særpreget for de to hovedretningene under Unge Vil-paraplyen.

### A. ATLAS-modellen (System & Struktur)

**Konsept:** Navigasjon, kartlegging, økosystem. ATLAS er "operativsystemet" for hvordan Unge Vil bygger bærekraftig frivillighet. Det skal føles trygt, vitenskapelig og oversiktlig.

-   **Primary Color:** Navy (`#1E1B4B`)
    
-   **Accent Color:** Mint (`#2DD4BF`)
    
-   **Visual Style:**
    
    -   **Blueprint Aesthetics:** Bruk rutenett (grids) eller tynne linjer i bakgrunnen for å signalisere struktur.
        
    -   **Modularitet:** Innhold presenteres i tydelige "moduler" eller kort (Bento-grid stil).
        
    -   **Technical Typography:** Gjerne bruk av monospace-fonter (eller Inter med tall-spacing) for data, faser (`Fase 01`) og etiketter.
        
    -   **Glassmorphism:** Frosted glass-effekter på mørke flater for å skape dybde og lagdeling.
        
-   **Motion & Animasjon (CSS/JS):**
    
    -   **Stemning:** _Presis, Flytende, Logisk._
        
    -   **Transitions:** Bruk `ease-out` kurver. Elementer skal gli på plass som brikker i et puslespill.
        
    -   **Load-in:** Linjer og grids tegnes opp først, deretter fader innholdet inn.
        
    -   **Interaksjon:** Hover-effekter skal være subtile – f.eks. en svak "glow" i Mint-farge eller et kort som løftes rolig opp.
        

### B. Create A Spark (Energi & Innovasjon)

**Konsept:** Gnisten. Startfasen. Rask, uredd og energisk. Dette brandet appellerer til skaperglede og "just do it"-mentalitet.

-   **Primary Color:** Spark Gold (`#FBBF24`)
    
-   **Contrast Color:** Black (`#000000`) or Dark Gray (`#111111`)
    
-   **Visual Style:**
    
    -   **High Contrast:** Sort bakgrunn med sterke gule/gull elementer.
        
    -   **Typography:** Inter **Black Italic** (foroverbøyd). Tekst kan være enorm og bryte rammer.
        
    -   **Stickers & Badges:** Grafiske elementer som ser ut som klistremerker ("New", "Beta", "Go") plassert litt skjevt/rotert.
        
    -   **Texture:** Bruk gjerne støy (noise) eller grove teksturer for å unngå at det ser for "corporate" ut.
        
-   **Motion & Animasjon (CSS/JS):**
    
    -   **Stemning:** _Rask, Snappy, Elektrisk._
        
    -   **Transitions:** Bruk `ease-out-expo` eller `spring` fysikk. Ting skal skje momentant.
        
    -   **Oppførsel:** Tekst kan "krasje" inn i bildet fra siden.
        
    -   **Effekter:** Bruk "glitch"-effekter ved hover, eller elementer som vibrerer/rister svakt for å vise ladet energi.
        
    -   **Looping:** Bakgrunner kan ha raske, repeterende mønstre (f.eks. diagonale striper som scroller evig).
        

## 7. UI Components (Web Specs)

### Buttons

-   **Primary:** Bg: `#9333EA`, Text: `White`, Rounded: `Full` (Pill shape).
    
-   **Secondary:** Border: `2px solid #9333EA`, Text: `#9333EA`.
    
-   **Hover States:** Darken background by 10% (e.g., `#7E22CE`).
    

### Cards & Containers

-   **Border Radius:** `1rem` (16px) or `1.5rem` (24px) for large containers.
    
-   **Shadows:** Soft, diffuse shadows.
    
    -   `box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);`
        
-   **Dark Mode Cards:** Bg: `#1F2937` (Gray-800) with Border: `1px solid #374151` (Gray-700).
    

### Gradients

-   **Purple Haze:** `linear-gradient(135deg, #9333EA 0%, #7E22CE 100%)`
    
-   **Atlas Deep:** `linear-gradient(to bottom, #1E1B4B, #111827)`
    
-   **Spark Energy:** `linear-gradient(45deg, #FBBF24, #F59E0B)`
    

## 8. CSS Classes (Tailwind Reference)

For rask implementering i kode:

```
/* Custom Utilities */
.bg-brand { background-color: #9333EA; }
.text-brand { color: #9333EA; }

.font-display { font-family: 'Inter', sans-serif; font-weight: 900; letter-spacing: -0.05em; }
.font-body { font-family: 'Inter', sans-serif; font-weight: 400; }

/* Sub-brand Helpers */
.atlas-theme { @apply bg-[#1E1B4B] text-white; }
.atlas-accent { @apply text-[#2DD4BF]; }
.atlas-card { @apply bg-white/5 backdrop-blur-md border border-white/10; }

.spark-theme { @apply bg-black text-[#FBBF24]; }
.spark-font { @apply font-black italic; }
.spark-btn { @apply bg-[#FBBF24] text-black font-black uppercase tracking-widest hover:scale-105 transition-transform; }

```
