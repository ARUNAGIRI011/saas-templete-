# Build order and section-by-section QA

## Phase 0 — Project access and setup
1. Confirm the Framer project URL and editor access.
2. Confirm whether the project is blank or contains existing work.
3. Set up the official Framer Agent only in an environment where Node.js/npm and authenticated project access are available.
4. Load current Framer skill/documentation and verify available commands.
5. Create a restore point/duplicate before major changes.

## Phase 1 — Foundations
1. Set colour and typography tokens.
2. Define desktop, tablet and phone breakpoints.
3. Build global container, spacing and grid rules.
4. Build buttons, cards, form fields and icon styles.
5. Validate keyboard focus and reduced-motion behavior.

## Phase 2 — Global shell
1. Header and desktop navigation.
2. Mobile navigation.
3. Footer.
4. Global CTA and announcement bar (optional).
5. Test all three breakpoints before continuing.

## Phase 3 — Home sections
For every section, build desktop/tablet/phone together, capture screenshots at each breakpoint, inspect overflow, wrapping, hierarchy, spacing and accessibility, fix defects, then proceed:
1. Hero
2. Trust/positioning note
3. Workflow overview
4. Platform feature grid
5. Product preview
6. Oversight and security
7. Use cases
8. Resources preview
9. FAQ
10. Final CTA

## Phase 4 — Inner pages
Build Platform, Clinical Workflows, Analytics, Research, Security & Privacy, Integrations, Pricing, About, Contact, Blog index/detail and 404. Reuse components and CMS templates.

## Phase 5 — CMS and interactions
1. Create Articles, Use Cases, Research and Integrations collections.
2. Bind collection pages and lists.
3. Implement tabs, accordions, mobile menu and form states.
4. Connect real form destination only after buyer provides service and credentials.
5. Add meaningful empty, success and error states.

## Phase 6 — QA
- Desktop, tablet and phone screenshots for each page.
- Check horizontal overflow, clipped text, tap targets and menu behavior.
- Check all internal links, CMS routes, 404 and form validation.
- Keyboard-only navigation and screen-reader labels.
- Contrast and reduced motion.
- Optimize images and verify loading.
- Confirm all demo data is labelled.
- Search for unsupported claims, placeholder links, fake logos and fake metrics.

## Required section QA record
Record: page/section, breakpoint, screenshot URL or file, issue, fix, retest result and date. Do not claim screenshot review unless screenshots were actually captured and inspected.
