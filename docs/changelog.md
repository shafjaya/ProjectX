# Changelog

## 2026-05-08
- Added mountain bike carousel below Add Task section
  - 7 bikes from Trek, Specialized, Giant, Cannondale, Canyon, Santa Cruz, Kona
  - Each card shows bike image, name, retailer, price, and a View More button
  - View More opens the retailer's page in a new tab
  - Left/right arrow nav buttons; horizontal scroll-snap carousel
- Added drag-and-drop to move tasks between quadrants
  - Tasks are draggable; dropping onto any quadrant's task list moves the task
  - Dashed outline highlights the target quadrant on drag-over
  - Trash drawer tasks are not draggable
- Added Unsplash background image at 20% opacity via fixed body::before pseudo-element
- Quadrant cards set to 90% opacity to let background show through
- Added motivational quote section below the Add Task form
  - 10 task-completion quotes, one chosen at random on each page load
  - Styled muted/italic to sit quietly beneath the form


- Made layout responsive across browser sizes
  - Matrix switches from 2-column to 1-column grid below 640px
  - Body padding reduces at 900px and 640px breakpoints
  - Quadrant select stretches to fill available width on mobile
  - h1 font-size reduced to 22px on small screens
- Added 5rem bottom padding to body so Add Task section has breathing room

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
