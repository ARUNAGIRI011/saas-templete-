# Design system

## Design direction
Premium light enterprise. Use deep navy for structure, teal for action and soft mint/blue surfaces for calm visual hierarchy. Avoid generic neon gradients and excessive glassmorphism.

## Colour tokens
- Ink / primary text: `#102A36`
- Deep navy: `#123746`
- Teal / primary action: `#087E80`
- Teal hover: `#06696B`
- Soft mint surface: `#EAF5F2`
- Pale blue surface: `#EFF5F8`
- Canvas: `#FAFCFC`
- White: `#FFFFFF`
- Secondary text: `#536873`
- Muted border: `#DCE7E8`
- Warning: `#A45A19`
- Error: `#A83E46`
- Focus ring: `#1B8F91`

Check contrast for all final text/background combinations; do not rely on colour alone to communicate status.

## Typography
- Display: Manrope (or buyer-selected licensed/available alternative)
- Body/UI: Inter
- H1: clamp(2.75rem, 5.5vw, 5.25rem), 1.02 line-height, -0.045em tracking
- H2: clamp(2rem, 3.8vw, 3.25rem), 1.1 line-height
- H3: 1.35–1.75rem
- Body large: 1.125rem / 1.65
- Body: 1rem / 1.65
- Caption: 0.8125rem / 1.45

## Layout and spacing
Use a 4px base scale: 4, 8, 12, 16, 24, 32, 40, 48, 64, 80, 96, 120.
- Content max width: 1200px
- Reading width: 720px
- Desktop side padding: 40–64px
- Tablet side padding: 28–36px
- Phone side padding: 20–24px
- Section vertical spacing: desktop 96–120px; tablet 72–88px; phone 56–72px
- Card radius: 16px; large panels: 24px; pill buttons: 999px
- Border: 1px solid muted border
- Shadows: restrained, soft and low contrast

## Responsive rules
- Desktop: 12-column grid; max content 1200px.
- Tablet: 8-column grid; collapse 3-column cards to 2 columns when needed.
- Phone: 4-column grid; all multi-column feature areas become one column unless a compact horizontal scroller is genuinely better.
- Never reduce body text below 15–16px for normal reading.
- Navigation becomes an accessible menu; ensure focus order and escape/close behavior.
- Avoid fixed heights for text-containing cards and hero sections.

## Component inventory
Buttons (primary, secondary, text), header, mobile menu, announcement bar, badges, feature cards, metric-free product preview, workflow stepper, quote block (only buyer-supplied quote), integration card, resource card, pricing card, FAQ accordion, form fields, CTA band, footer, breadcrumbs, tabs, modal/dialog and CMS list/detail templates.

## Motion
Use subtle opacity/translate transitions (160–240ms). Respect reduced-motion preferences. Avoid scroll hijacking and autoplaying audio/video. Any video must have controls or a clear pause mechanism.

## Accessibility
Semantic headings, descriptive links, visible keyboard focus, labels and error text for forms, adequate contrast, alt text, keyboard-operable menus/tabs/accordions and reduced-motion support.
