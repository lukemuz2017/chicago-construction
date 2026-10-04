# Chicago Construction Tracker — Agent Context

## Concept
A public-facing landing page for the City of Chicago that surfaces active and upcoming
construction and maintenance projects across the city.

## Audience
Chicago residents and commuters who want to know what is being built near them, why it
is happening, and how long it will last.

## What a visitor should understand or do
- Discover construction sites near them or in areas they care about
- Understand the type and purpose of each project
- See current status and timeline at a glance
- Know what hours of day work is active

## Key data points to display
- **Location** — neighborhood, street address, or map pin
- **Construction type** — road resurfacing, utility work, building permit, bridge repair,
  water main, sewer, transit, parks & rec, etc.
- **Purpose/reason** — why the work is happening (routine maintenance, infrastructure
  upgrade, emergency repair, new development, ADA compliance, etc.)
- **Timeline** — start date, estimated end date, percent complete
- **Current status** — Not Started / In Progress / Paused / Complete
- **Work hours** — typical hours of day when crews are active (e.g. 7 AM–5 PM weekdays)
- **Impact** — lane closures, sidewalk closures, noise/vibration advisories
- **Responsible agency** — CDOT, ComEd, MWD, private developer, etc.
- **Permit number** — for reference and transparency
- **Community district / ward** — political geography context

## Additional brainstormed data points
- Nearby transit impact (which CTA lines or stops are affected)
- 311 complaint or service request reference number
- Before/after imagery placeholder
- Community meeting or public notice dates (for large projects)
- Budget or cost estimate
- Weather delay log
- Inspector or project manager contact (optional)
- Carbon/disruption footprint estimate
- Seasonal constraints (e.g. winter pause expected)

## Technical constraints
- Pure HTML, CSS, JavaScript only — no frameworks or build tools
- Fully static files, no backend or API calls
- No functional internal navigation links within individual version pages
  (pages are design explorations, not working prototypes)
- Gallery (index.html) links to each static version page
- Target deployment: Vercel

## Iteration arc — 25 versions
Each page builds toward the final design. The arc moves from raw structure → visual
language → layout complexity → interactivity hints → full polish.

| # | Title | Focus |
|---|-------|-------|
| 1 | Raw Text | Unstyled HTML — plain data, no CSS |
| 2 | Basic Structure | Semantic headings and sections |
| 3 | First Styles | CSS baseline — clean white, readable fonts |
| 4 | Chicago Palette | City flag colors introduced |
| 5 | Card Grid | Each construction site as a card |
| 6 | Status System | Color-coded badges for project status |
| 7 | Map Hero | Placeholder map as the page focal point |
| 8 | Navigation | Header with city branding and nav bar |
| 9 | Filter UI | Category and status filter controls |
| 10 | Timeline View | Horizontal timeline per project |
| 11 | Data Table | Tabular layout for side-by-side comparison |
| 12 | Icon Language | Icons per construction type |
| 13 | Search First | Search bar as the primary interface |
| 14 | Hero Moment | Full-width city photography hero section |
| 15 | Sidebar Layout | Persistent left-side filter panel |
| 16 | Responsive Grid | Mobile-ready card grid |
| 17 | Dark Theme | Night-mode color scheme variant |
| 18 | At-a-Glance Stats | KPI summary row above content |
| 19 | Progress Indicators | Visual completion bars per project |
| 20 | Micro-interactions | Hover and focus effects throughout |
| 21 | Motion | Subtle entrance animations on scroll |
| 22 | Mobile-First | Phone-optimized compact layout |
| 23 | Accessibility | High contrast, ARIA-aware design pass |
| 24 | Brand Refinement | Polished Chicago visual identity |
| 25 | Final Design | Complete, production-ready landing page |

## Notes for agents
- Each version lives at pages/v01.html through pages/v25.html
- The gallery lives at index.html
- When building a new version, review the previous version for continuity
- Chicago flag palette: blue #0076C0, red #E31837, white #FFFFFF
- Prefer real-feeling placeholder data (Chicago street names, realistic timelines)
- Do not add JavaScript interactivity unless the version description calls for it
