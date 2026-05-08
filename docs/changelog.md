# Changelog

## 2026-05-08
- Made layout responsive across browser sizes
  - Matrix switches from 2-column to 1-column grid below 640px
  - Body padding reduces at 900px and 640px breakpoints
  - Quadrant select stretches to fill available width on mobile
  - h1 font-size reduced to 22px on small screens
- Added 5rem bottom padding so the Add Task section has breathing room
- Added Unsplash background image (mountain landscape) at 20% opacity via fixed `body::before` pseudo-element
- Set quadrant cards to 90% opacity so the background shows through without affecting content readability
- Added motivational quote section between the matrix and Add Task
  - 10 task-completion quotes, one chosen at random on each page load
  - Styled muted and italic to sit quietly below the matrix
- Added drag-and-drop to move tasks between quadrants
  - Tasks are draggable; dropping onto any quadrant's task list moves the task
  - Dashed outline highlights the target quadrant on drag-over
  - Trash drawer tasks are not draggable
- Added "Found some free time?" carousel below the Add Task section
  - 16 cards total: Pizza Hut Singapore first, then 15 gravel bikes
  - Gravel bike retailers: Trek, Specialized, Giant, Cannondale, Canyon, Orbea, BMC Switzerland, Scott Sports, Marin Bikes, Salsa Cycles, Ribble Cycles, Cervelo, Norco, Kona, Surly
  - Each card shows a verified Unsplash photo, product name, retailer, price, and a View More button that opens the retailer in a new tab
  - Left/right arrow navigation, horizontal scroll-snap, onerror fallback placeholder (🚵) for any failed images

## 2026-05-05
- Built morning todo dashboard (`index.html`)
  - Eisenhower matrix 2x2 grid layout
  - Dark slate theme with CSS variables
  - Four quadrants: Do First, Schedule, Delegate, Drop
  - Tasks with checkbox, optional mind-heavy indicator, completed state
  - Add task form with quadrant select, mind-heavy toggle, Enter key support
  - 8 example tasks pre-loaded across all quadrants
- Redesigned dashboard with refined spec
  - Real-time Done/Left counts per quadrant
  - Border radius on quadrants and form elements
  - Clicking anywhere on task row toggles completion
  - Improved hover states and completed task styling
  - Mind-heavy button label: `+ Mind-heavy` / `🧠 Mind-heavy`
- Added current date display next to "Today" heading (muted, smaller text)
- Added trash drawer for overflow completed tasks
  - Max 3 most recent completed tasks shown inline per quadrant
  - Older completed tasks collapse behind a trash icon with count
  - Clicking trash icon toggles a drawer listing overflow items
  - Items in drawer can still be unchecked to restore them
