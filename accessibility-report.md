# Accessibility Report — index.html

This document lists accessibility issues found (manual review) and how they were fixed. It also explains how to run the Lighthouse accessibility audit.

## Issues found and fixes applied

1. Missing lang attribute on <html>
   - Fix: added lang="en" to <html> so screen readers announce the correct language.

2. Images missing alt text
   - Fix: added descriptive alt text to all images (placeholder images included have alt attributes).

3. Non-semantic structure
   - Fix: used semantic elements (<header>, <nav>, <main>, <section>, <footer>) to improve landmarks and navigation for assistive tech.

4. Form fields without labels
   - Fix: ensured every input has a <label> and used fieldset/legend to group related controls.

5. Color contrast (manual check recommended)
   - Suggestion: verify color contrast with Lighthouse or other tools and adjust colors to meet WCAG AA.

## How to run Lighthouse accessibility audit

1. Open the page in Chrome.
2. Open DevTools (F12 or Ctrl+Shift+I) and go to the "Lighthouse" panel.
3. Choose "Accessibility" (and other categories if desired) and click "Generate report".
4. Record the resulting accessibility score here.

> Final Lighthouse accessibility score: (run Lighthouse in your browser and paste the score here)

## Additional recommendations
- Ensure link text is descriptive (avoid "click here").
- Add skip link to allow keyboard users to jump to main content (e.g., <a class="skip-link" href="#main">Skip to main content</a>).
- Validate forms with server-side checks in addition to client-side validation.

