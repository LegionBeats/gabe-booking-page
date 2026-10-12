# Gabe Booking Page

A scheduling page for friends: "We said we'd talk. Let's actually do it." It embeds the GHL group calendar (20-min and 45-min "Chat with Gabe") so nobody has to text back and forth to find a time.

## Files

| File | What it is |
| --- | --- |
| `ghl-embed.html` | **The one to use in GoHighLevel.** Paste the whole file into a Custom JS/HTML element. |
| `index.html` | Standalone version for hosting on its own (Netlify, Vercel, any static host). |

Both are a single file with no build step and no dependencies.

## Using it in GoHighLevel

1. Add a **Custom JS/HTML** element to a blank page.
2. Paste the full contents of `ghl-embed.html`.
3. On that section, set the background to dark (`#07070a`) and padding to 0 so no GHL color shows around it.
4. Preview, then book a test slot to confirm the calendar loads.

It is scoped to one `#gb` container, breaks out of the column to full width, and never touches the page's `html` or `body` styles.

## Hosting it standalone

Connect this repo to Netlify or Vercel (publish directory is the repo root), or drag the folder into Netlify Drop. Use `index.html`.

## Changing the calendar

Both files embed the same GHL calendar. To point at a different one, replace the iframe `src` and its `id` with the new embed code from GHL, in whichever file you use.

## Effects

- Headline letters blur in and flip up one by one; the second line is gold/red with a shine sweep
- A dim grid with a brighter amber grid that shows only around the cursor
- Ember particles that drift upward and get pushed away by the cursor
- A spinning red/gold gradient border with a blurred glow around the calendar, plus a glare that follows the cursor

The animations are skipped for visitors who have reduced motion turned on.
