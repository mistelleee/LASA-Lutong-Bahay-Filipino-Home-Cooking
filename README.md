# LASA-Lutong-Bahay-Filipino-Home-Cooking
## Lasa — Lutong Bahay

### What It Is

**Lasa** is a personal Filipino recipe book web application — a digital cookbook designed specifically for Filipino home cooking. Built entirely with vanilla HTML, CSS, and JavaScript with zero dependencies, no frameworks, and no backend. It runs in any browser, stores everything locally, and works offline.

The name *Lasa* means "flavor" or "taste" in Filipino — fitting for an app that treats recipes not as data entries but as cultural artifacts worth preserving.

---

### The Problem It Solves

Filipinos search for recipes across YouTube, Facebook groups, blogs, and Google — and the results are scattered, inconsistent, and often buried under ads. There is no clean, personal tool for Filipino home cooks to **collect**, **organize**, and **actually cook** from their own curated recipe collection.

Lasa fills that gap. It is not a recipe aggregator. It is **your** recipe book — pre-loaded with authentic Filipino dishes and expandable with your family's own heirloom recipes.

---

### Design Philosophy

The visual identity is rooted in the **Filipino kubo (nipa hut)** and the warmth of a **karinderya (neighborhood eatery)**. Dark wood tones, sawali weave patterns, and warm amber accents create an atmosphere of a kitchen at golden hour. Typography pairs handwritten Caveat (for titles and labels, evoking chalkboard menus) with Lora serif (for readable body text) and DM Mono (for data and measurements).

Every recipe card is rendered as a **book** — with a visible spine, stacked page edges, and an inner frame border. On hover, cards lift and rotate in 3D perspective, simulating the act of pulling a book from a shelf. The detail view opens as a **two-page spread** on cream-colored paper with a center fold shadow, like reading an actual cookbook.

All icons are **illustrated, not emoji** — CSS-drawn gold initials in gradient circles, inspired by illuminated medieval manuscripts. No emojis anywhere in the interface.

---

### Core Features

**8 Authentic Filipino Recipes** — Adobo, Sinigang, Kare-Kare, Tinola, Lechon Kawali, Bicol Express, Pancit Canton, and Leche Flan. Each recipe includes:
- Ingredient list with precise measurements
- Step-by-step cooking procedure
- Cultural story ("Kwento") about the dish's origins and significance
- Cooking tip from Lola ("Tip ni Lola")

**Book-Style Cards** — Every recipe appears as a physical book on a wooden shelf. The CSS 3D perspective transform creates a lifelike tilt on hover. Staggered entrance animations make cards cascade in one by one.

**Open Book Detail View** — Clicking a recipe opens a cream-paper two-page spread. The left page contains ingredients and serving controls. The right page contains the procedure, story, and tips. A realistic center fold shadow splits the pages.

**Serving Adjuster** — Tap plus or minus to scale all ingredient quantities up or down. Fractions display beautifully using Unicode vulgar fractions (½, ¼, ¾, ⅓, ⅔, ⅛).

**Ingredient Checkboxes** — Tap any ingredient while prepping to cross it off. Checked state persists across sessions.

**Guided Cooking Mode** — Tap "Luto Na" and the screen transforms into a dark, focused kitchen environment with a warm candlelight glow effect. Features:
- **Mise en Place checklist** — auto-generated from the ingredient list, so you prep everything before the stove is on
- **Step-by-step display** — large, readable text that works from across the kitchen counter
- **Auto-detected timers** — if a step mentions "35 minutes" or "1 hour", the app highlights the time and offers a countdown timer with an audio alert
- **Progress bar** — visual indicator of how far through the recipe you are

**Shopping List ("Pamilihan")** — ingredients from any recipe compile into a grouped shopping list, automatically sorted by wet market section:
- Karne at Isda (Meat & Seafood)
- Gulay (Vegetables)
- Bigas at Iba Pa (Rice & Dry Goods)
- Sawsawan (Sauces & Condiments)
- Gatas at Itlog (Dairy & Eggs)

Each item shows an **estimated Philippine Peso price** based on average palengke rates. A running total appears at the bottom.

**Add Your Own Recipes** — Lola's secret adobo? Your mom's special kare-kare? Add it to your personal collection through a structured form with ingredients and steps.

**Favorites** — heart any recipe for quick access. Persisted across sessions.

**Category Filtering** — browse by Ulam, Merienda, or Panghimagas. Full-text search across names, descriptions, and alt names.

---

### Technical Details

- **Zero dependencies** — no React, no Vue, no jQuery, no npm packages. Pure vanilla JavaScript (ES5-compatible where possible for maximum browser support).
- **localStorage persistence** — favorites, custom recipes, shopping list, ingredient checkboxes, and shopping list checks all survive page refreshes and browser restarts.
- **Responsive** — adapts from desktop to mobile with CSS grid and media queries. The book spread stacks vertically on small screens.
- **Accessible** — keyboard-navigable (Escape to close modals and cooking mode), semantic HTML, proper contrast ratios.
- **Single file** — the entire application is one self-contained HTML file. No build step, no server required. Open the file in a browser and it works.
- **Custom CSS animations** — 3D book hover transforms, staggered grid entrances, candlelight flicker, sign sway, timer pulse, and view crossfades. All CSS, no animation libraries.
- **Audio feedback** — Web Audio API generates a tone when cooking timers complete. Works in all modern browsers without any sound files.

---

### What Makes It Different

There is no other tool that does what Lasa does for Filipino home cooking. Recipe websites give you one recipe at a time. Meal planning apps treat food as data. Lasa treats recipes as **stories** — with cultural context, family wisdom, and the physicality of a real cookbook.

It is the digital equivalent of your lola's handwritten recipe notebook — except it can adjust servings, build your shopping list, walk you through each step, and keep time while you cook.
