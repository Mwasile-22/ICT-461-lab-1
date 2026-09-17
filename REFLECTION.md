# Reflection — ICT461, Unit 1

For this task I built a one-page course registration form for ICT461 using plain HTML, CSS, and JavaScript — no frameworks, since the point was to understand the fundamentals before we get into HTTP next lecture.

I structured the page with proper semantic tags instead of just wrapping everything in divs — header, main, footer, and fieldset/legend to group the student details and section selection. Every input has a label properly linked to it, so a screen reader (or just tabbing through with the keyboard) makes sense of the form without any extra explanation. I made sure I could complete the whole form using only the keyboard, and that the focus outline is always visible, since that's something that's easy to accidentally strip out with CSS and forget about.

For the JavaScript, I went with a seat-availability check tied to the section dropdown. When you pick a section, it pulls the seat count and capacity straight off the option and shows it live — and if a section is full, it disables the register button instead of letting you submit and only failing later. I also added validation for the name, student ID format, and email, with error messages that actually explain what's wrong instead of just turning the border red.

The CSS is responsive with a fluid layout and clamp() for text sizing, so it holds up from a phone screen to a full desktop without needing separate breakpoints for everything.

If I were to improve it, I'd add proper server-side validation, since right now everything only checks in the browser — which ties in well with what's coming next: HTTP fundamentals, and actually sending this data somewhere real.
