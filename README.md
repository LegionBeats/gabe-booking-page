# Gabe Booking Page

Single static file (`index.html`), no build step and no dependencies. It a no-back-and-forth scheduling page for friends. Embeds the GHL group calendar (20-min and 45-min "Chat with Gabe").

Deploy: drag the folder into Netlify Drop, connect the repo on Vercel or Netlify, or paste the contents of `index.html` into a GHL funnel custom-code element.

Effects (modeled on the Stash component library):
- Headline letters blur in and flip up one by one; the second line is gold/red with a shine sweep
- A dim grid with a brighter amber grid that shows only around the cursor
- Ember particles that drift upward and get pushed away by the cursor
- A spinning red/gold gradient border with a blurred glow around the calendar, plus a glare that follows the cursor

The animations are skipped for visitors who have reduced motion turned on.
