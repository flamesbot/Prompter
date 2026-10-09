## 2024-05-17 - aria-label Overriding Inner Content
**Learning:** Adding an `aria-label` to an interactive element (like `role="button"`) completely overrides its inner content for screen readers. In the Prompt Machine app, adding `aria-label="Tap to copy this prompt"` to the main card prevented screen readers from ever reading the actual prompt text inside it.
**Action:** Use `aria-describedby` linked to external hint text instead of `aria-label` when an element contains important dynamic text that must be read by screen readers.
## 2024-05-18 - Missing Hover States on Retro UIs
**Learning:** Even when building intentionally "retro" 3D interfaces (like Windows 9x styling), modern users rely on contemporary interaction cues like pointer cursors and smooth background color transitions on hover. Without them, interactive elements can feel "dead" or undiscoverable until clicked.
**Action:** Always overlay modern UX affordances (`cursor: pointer`, `:hover` background shifts, `transition` on hover properties) onto retro styling to maintain discoverability and confidence in interaction.
