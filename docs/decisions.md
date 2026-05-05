# Decisions

## Completed tasks stay visible in quadrants (not removed)
Completed tasks remain in their quadrant, faded and struck through, rather than being deleted or moved to a separate list. This preserves a sense of momentum — you can see what you've already done alongside what's left.

## Max 3 completed tasks shown inline, rest in trash drawer
Showing all completed tasks inline would push active tasks down and clutter the view as the day progresses. Capping at 3 (most recent) keeps quadrants scannable. Older completions are still accessible via the trash drawer rather than hidden entirely, so nothing is lost.

## Completed tasks ordered oldest-first in trash drawer
The trash drawer shows overflow completed items in the order they were added (oldest first), since the 3 most recent are already visible inline. This avoids duplication and gives a natural chronological archive.

## No persistence (no localStorage)
Tasks reset on page refresh. Intentional for now — keeps the implementation simple and stateless. Adding localStorage is in ideas.md for a future session.
