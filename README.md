# ICT461 — Course Registration Page

**Unit 1, Lecture 1 assessment — Mulungushi University, School of Engineering**

A single-page course registration interface for ICT461 (Web Systems and Technology), built with semantic HTML, responsive CSS, and one core JavaScript interaction.

## What's here

- `index.html` — the full page (structure, styles, and script in one file for easy review)

## Features

- Semantic structure: `header`, `main`, `form`, `fieldset`/`legend`, `footer`, and a skip link for keyboard users
- Labelled, keyboard-operable controls (`label for`, visible focus outlines, no keyboard traps)
- Responsive layout down to narrow phone widths (single fluid column, `clamp()` type sizing)
- Client-side validation for name, student ID format, and email, with visible inline error messages and `role="alert"` so screen readers announce them
- One core JS interaction: choosing a tutorial section shows live seat availability pulled from the selected `<option>`'s data, and disables registration for a full section

## Running it

Open `index.html` directly in a browser — no build step or server required.

## Accessibility checks performed

- Tabbed through the entire form using only the keyboard; focus order matches visual order and every control has a visible focus ring
- Confirmed every input has a programmatically associated label
- Confirmed error messages are exposed via `role="alert"` / `aria-live` and `aria-invalid` is toggled correctly
- Checked color contrast of text and error/success states against their backgrounds

## Assessment evidence

See the submission notes for the DevTools Elements and Network screenshots and the reflection.
