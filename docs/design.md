# Design System: Editorial Romance

## 1. Overview & Creative North Star: "The Digital Keepsake"
This design system rejects the "cookie-cutter" wedding template in favor of a high-end editorial experience. Our Creative North Star is **The Digital Keepsake**—an aesthetic that treats the web browser like the pages of a bespoke, tactile invitation.

To achieve this, we move away from rigid, centered grids. We embrace **intentional asymmetry**, where images and text blocks overlap, and **tonal depth**, where elements breathe through white space rather than structural lines. The goal is to feel "airy" yet "grounded," using the primary brand color (`#c05178`) not as a background, but as a surgical strike of energy against the soft, romantic backdrop.

---

## 2. Colors: Tonal Sophistication
Our palette is rooted in the interplay between soft neutrals and high-energy accents. We use color to guide the eye, not to trap it in boxes.

### Palette Strategy
*   **The "No-Line" Rule:** Direct sectioning via 1px solid borders is strictly prohibited. Boundaries must be defined by shifts in surface tones—for example, transitioning from `surface` to `surface-container-low`.
*   **Surface Hierarchy & Nesting:** Treat the UI as layers of fine vellum paper. Nest a `surface-container-lowest` card inside a `surface-container` section to create a natural, soft-edged lift.
*   **The "Glass & Gradient" Rule:** For floating navigation or modal overlays, use **Glassmorphism**. Apply `surface` with 70% opacity and a `20px` backdrop-blur.
*   **Signature Textures:** Main CTAs should utilize a subtle linear gradient (45-degree) from `primary_container` to `primary` (`#c05178`) to provide a "lit from within" glow.

---

## 3. Typography: The Editorial Voice
The tension between the serif and sans-serif is where the brand’s "Modern Romantic" personality lives.

*   **Display & Headlines (Noto Serif):** Used for names, declarations, and emotional anchors. Use `display-lg` for hero sections with tight letter-spacing (-0.02em) to mimic high-end fashion mastheads.
*   **Body & Titles (Manrope):** A clean, architectural sans-serif. It provides the "modern" counter-balance to the serif. Use `body-lg` for storytelling and `label-md` (all caps, +0.1em tracking) for utility text like dates and locations.
*   **Visual Hierarchy:** Headlines should never feel "bolted on." Overlap `display-md` text slightly over the edge of an image to break the grid and create depth.

---

## 4. Elevation & Depth: Tonal Layering
We do not use heavy shadows. We use light.

*   **The Layering Principle:** Depth is achieved by stacking. A `surface-container-highest` element should feel like the most "important" piece of paper on the desk.
*   **Ambient Shadows:** If an element must float (like a "Save the Date" FAB), use a shadow color derived from `on-surface` at 5% opacity with a `40px` blur and `10px` Y-offset. It should feel like a soft glow, not a dark weight.
*   **The "Ghost Border" Fallback:** If a border is required for clarity (e.g., input fields), use `outline-variant` at 20% opacity. 100% opaque borders are forbidden.
*   **Creative Lines:** While standard borders are out, "Decorative Lines" are in. Use the `secondary` (`#9f6777`) color for ultra-thin (0.5px), long horizontal lines that bleed off the edge of the screen to create a sense of continuity.

---

## 5. Components: Fluidity and Grace

### Buttons
*   **Primary:** Gradient fill (`primary_container` to `primary` (`#c05178`)), `roundedness` 2, and `title-sm` typography.
*   **Secondary:** Ghost style. No fill, `outline-variant` (20% opacity) border, and `secondary` (`#9f6777`) colored text.
*   **Interaction:** On hover, primary buttons should scale slightly (1.02) and increase shadow diffusion.

### Cards & Imagery
*   **The Frame:** Do not use borders for cards. Use `surface-container-low` and a `lg` (1rem) corner radius.
*   **Dynamic Borders:** Instead of a border *around* the card, use a 2px `primary` (`#c05178`) line that only runs along the *top-left* corner (forming an 'L' shape) to frame the content within.

### Input Fields
*   **Styling:** Use `surface-container-lowest` as the fill. The label should use `label-md` in `on-surface-variant`.
*   **Focus State:** The bottom border should animate from `outline-variant` to `primary` (`#c05178`) upon focus.

### Additional Signature Components
*   **The Scroll Scrubber:** A thin, vertical `secondary` (`#9f6777`) line on the right side of the screen that grows as the user scrolls, acting as a progress indicator.
*   **The Floating Keepsake:** A small, circular chip (`primary_fixed`) that stays fixed in a corner, containing a countdown or a "Registry" quick-link.

---

## 6. Do’s and Don’ts

### Do
*   **Do** use asymmetrical margins. If the left margin is 10%, make the right margin 15% for an editorial feel.
*   **Do** use "White Space" as a functional element. Allow sections to breathe with at least 120px of vertical padding.
*   **Do** use `notoSerif` for large numeric dates to make them feel like design elements.

### Don't
*   **Don't** use standard 1px grey dividers between list items; use a `surface-container` color shift instead.
*   **Don't** use pure black (#000000) for text. Use `on-surface` (#1f1a1d) to maintain the soft, organic feel.
*   **Don't** use sharp corners. Everything should have at least a `sm` (0.25rem) radius to feel approachable and romantic.