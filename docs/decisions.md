# Decisions

## Completed tasks stay visible in quadrants (not removed)
Completed tasks remain in their quadrant, faded and struck through, rather than being deleted or moved to a separate list. This preserves a sense of momentum — you can see what you've already done alongside what's left.

## Max 3 completed tasks shown inline, rest in trash drawer
Showing all completed tasks inline would push active tasks down and clutter the view as the day progresses. Capping at 3 (most recent) keeps quadrants scannable. Older completions are still accessible via the trash drawer rather than hidden entirely, so nothing is lost.

## Completed tasks ordered oldest-first in trash drawer
The trash drawer shows overflow completed items in the order they were added (oldest first), since the 3 most recent are already visible inline. This avoids duplication and gives a natural chronological archive.

## No persistence (no localStorage)
Tasks reset on page refresh. Intentional for now — keeps the implementation simple and stateless. Adding localStorage is in ideas.md for a future session.

## Background image applied via body::before at 20% opacity
Using a pseudo-element rather than setting opacity on the body itself means the image sits behind all content without affecting text or card readability. 20% keeps it atmospheric without competing with the UI.

## Carousel Unsplash images verified individually with onerror fallback
Unsplash photo IDs were looked up and confirmed one by one via page fetches rather than guessed. An onerror handler replaces any failed image with a gradient placeholder (🚵) so cards always render correctly even if a URL breaks in future.

## Carousel mixes gravel bikes and a Pizza Hut Singapore card
The carousel is a personal discovery section — not strictly task-related. Mixing in a pizza order option next to bike browsing reflects the user's actual interests and makes the dashboard feel personal rather than generic.
