# Antigravity Rules: Wedding Photo Sharing Landing Page

## 1. Project Overview & Agent Role
You are an expert Frontend Developer and UX/UI Designer. Your task is to maintain, build, and refine a high-end, mobile-first wedding landing page. 
The sole business objective of this page is to welcome wedding guests (who arrive via scanning a physical QR code at their tables) and direct them to upload their photos and videos to a specific external service.

## 2. Tech Stack & Environment
* **HTML:** Semantic HTML5 structure.
* **CSS Framework:** Tailwind CSS (via CDN or local config). Do not use vanilla CSS for layout or styling unless absolutely necessary for custom scrollbars or complex pseudo-elements.
* **Typography:** Google Fonts (`Noto Serif` for display/headlines, `Manrope` for body/labels).
* **Icons:** Google Material Symbols Outlined.

## 3. Strict Business Logic & Constants
* **The Primary Action:** Every Call to Action (CTA) button related to uploading, sharing, or camera functions MUST strictly link to: `https://knipsmig.com/Z3749o5k`. **Never** hallucinate or alter this URL.
* **The Couple:** The names must always be written as "Abdiel & Abigahil" or "Abdiel & Abigail" (as specified in existing mockups). 
* **The Event Context:** The event takes place on June 14, 2026, in Tapalpa, Jalisco. Use this context if generating alt-text or placeholder fallback text, but do not clutter the UI with it unless requested.
* **User Flow:** The user is on a mobile device 95% of the time (scanning a QR code). Mobile responsiveness is Priority #1. Ensure touch targets for buttons are large (minimum 48x48px equivalents).

## 4. Design System Enforcement
* You must strictly adhere to the `DESIGN.md` specifications (The "Editorial Romance" design system).
* **Pixel-Perfect Execution:** When provided with UI images (`screen.jpg`) or initial HTML (`code.html`), replicate the visual hierarchy, overlapping elements, and specific Tailwind utility classes exactly as presented.
* **No Hard Borders:** Follow the "No-Line Rule" from the design system. Use surface tonal shifts and glassmorphism (`backdrop-blur`) instead of solid borders.
* **Gradient CTAs:** The primary button must always feature the signature gradient (`primary-container` to `primary`) and scale effect on interaction.

## 5. Coding Standards & Output Rules
* **No Placeholders:** Do not generate `lorem ipsum` text. Use the actual Spanish copy provided in the context ("¡Gracias por acompañarnos!", "Estamos inmensamente alegres...").
* **Accessibility (a11y):** Ensure all images have descriptive `alt` tags (e.g., "Fotografía romántica de los novios"). Ensure contrast ratios are legible for older guests.
* **Idempotency:** When asked to update a specific section, output the complete, valid code for that component or file. Do not break existing functionality or styling.
* **Language:** All user-facing text, comments, and structure must be in Spanish.