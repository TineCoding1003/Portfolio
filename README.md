# Tinevimbo Munjoma — Profile & Mini-Portfolio

A semantic HTML5 profile and mini-portfolio page.

## View the Page

Open `index.html` in any browser, or enable GitHub Pages on this repository
and link the published URL here: `[link once enabled]`

## AI-Assisted Content

See [PROMPT_LOG.md](./PROMPT_LOG.md) for the prompt used to draft the
About-section bio, the AI's raw output, my final edited version, and a
short reflection on what I changed and why.

## Accessibility Review

**Issue found by peer reviewer (Thursday's practical session):**
PLACEHOLDER — describe exactly what your reviewer flagged. Example: "My
phone input had no associated `<label>`, so a screen reader announced it
only as an unlabeled text field."

**Fix applied:**
PLACEHOLDER — describe exactly what you changed in response. Example:
"Added `<label for="phone">Phone Number</label>` tied to the input's
`id="phone"`, and re-checked with the reviewer that it now announces
correctly."

## Tech Stack

- Semantic HTML5
- Vanilla CSS (responsive layout + Tailwind CSS coming in the Unit III assignment)
- Native HTML5 form validation — `required`, `type="email"`, `pattern`, `minlength` (no JavaScript)

## Course Info

- **Course:** Web Technologies (WT) – CIS2103, Africa University
- **Assignment:** Practical Assignment 1 — Semantic HTML5 Profile & Mini-Portfolio Page
- **Programme:** SE & CIS, Year 2, Sem 1

## Responsive Notes

### Breakpoints tested
I tested the page in Chrome's device toolbar at 375px (mobile), 768px (tablet) and 1280px (desktop). There is no sideways scrolling at any of them.

My own media queries are at 768px and 1120px. I wrote the mobile styles first and used `min-width` to change the layout for bigger screens.

### Flexbox vs Grid
- **Grid:** I used Grid for the main page layout, because the sections need to move in rows and columns. It is one column on mobile, two columns on tablet, and on desktop the Contact section moves to the side. I also used Grid for the skills list so the boxes fit across the screen by themselves.
- **Flexbox:** I used Flexbox for the header and the nav links, because they sit in one line and wrap on small screens. I also used it to put each label above its input in the form.

### Where I used Tailwind
I used Tailwind for the header/nav and the contact form. I used the `sm:`, `md:` and `lg:` variants, for example `md:flex-row` to put the header text and image side by side on bigger screens.

### CSS and Tailwind split
- `styles.css` styles everything else: colours, fonts, spacing, the page layout, the skills grid and the footer.
- Tailwind styles the header/nav and the contact form only.
- I turned off Tailwind's Preflight reset because it was overriding my own CSS.