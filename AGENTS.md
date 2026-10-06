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

## Concept (expanded)
Chicago Builds is both a **tracker** and a **community platform**. It surfaces official
government construction data AND gives residents a channel to report what the city has
missed — unreported hazards, work outside permitted hours, dangerous conditions,
or projects not yet in any public database. Community reports are reviewed and shared
with the relevant city agency.

## Landing page content structure
Every version of the landing page should include these content zones:

- **Hero / header image** — A striking visual establishing Chicago identity (skyline, flag,
  construction-site imagery). Can be photo, CSS gradient, SVG illustration, or CSS art.
  Experiment across versions with different treatments.
- **"Chicago Builds." brand mark** — The site name displayed prominently at the top of
  every page, styled to match each version's visual language.
- **Mission statement** — 2–3 sentence intro explaining what the tracker is, who it serves,
  and that it is a community platform (not just a government data mirror).
- **Search bar** — Prominent input letting residents find projects by street, neighborhood,
  ZIP code, or keyword.
- **8 construction categories** — Visual links letting users browse by type of work.
- **City stats** — High-level numbers showing the scale of Chicago's construction activity.
- **Community feedback section** — A resident-facing reporting form near the bottom of the
  page. See the "Community feedback section" spec below.

## 8 construction categories
Consolidate all project types into these eight:

| Category | Covers |
|---|---|
| Roads & Pavement | Resurfacing, pothole repair, curb/gutter, alley paving |
| Water & Sewer | Water main replacement, sewer repair, flood infrastructure |
| Transit & CTA | Train station upgrades, bus lane work, track replacement |
| Highways & Expressways | IDOT/ISTHA expressway and ramp projects |
| Utilities | ComEd, Peoples Gas, telecom conduit, streetlights |
| Parks & Recreation | Chicago Park District projects, trails, fieldhouses |
| New Development | Private building permits, demolition, new construction |
| Bridges & Structures | Bridge deck repair, viaducts, overpasses, retaining walls |

## Community feedback section
Every version of the landing page must include a community reporting section. It is a
core feature of the site, not optional. Spec:

**Purpose** — Let residents flag anything missing from official city records:
unreported hazards, dangerous sidewalk/road conditions, construction running outside
permitted hours, projects not listed in the database, noise/vibration complaints.

**Required elements:**
- Section header: "See something the city missed?" (or equivalent)
- Short description: explain this is a community platform, reports go to editors and
  the relevant city agency, and may be published publicly
- Report type selector: Unreported hazard · Hours violation · Project missing from
  database · Road/sidewalk damage · Noise/vibration complaint · General feedback
- Location field: street address or intersection
- Description textarea: "What did you observe? Be as specific as possible."
- Optional contact field: email or phone for follow-up
- Submit button
- Disclaimer: "For emergencies call 911. Non-emergency city services: call 311."

**Community impact stats to display alongside the form:**
- 847 community reports submitted this year
- 312 escalated to city agencies
- 94% agency acknowledgment rate

**Style guidance:** The feedback section should match the visual language of each
version — dark themed for dark pages, clean civic for light pages, minimal for ledger
pages. It should feel like a natural extension of the page, not a separate widget.

## City stats to display
Use these placeholder figures (update when real data is available):
- **1,247** active projects
- **28,400+** union workers on-site
- **389** projects completed this year
- **77** neighborhoods impacted
- **$2.4B** in active contracts
- **12** city agencies involved

## Gallery
The design gallery lives at `gallery-option-c.html` (settled design). It links to
`pages/v01.html` through `pages/v25.html`. The `index.html` at root is reserved for
the actual production landing page when it is ready.

## Iteration arc — 25 versions
Versions 01–04 are full landing page design explorations — distinct visual directions
experimenting with hero treatment, layout, and tone. Versions 05–25 iterate on the
chosen direction, adding complexity and polish toward the final page.

| # | Title | Focus |
|---|-------|-------|
| 1 | Bold Editorial | Dark navy hero, SVG skyline silhouette, large italic serif type |
| 2 | Civic Standard | Sky-blue official header, white floating search card, card grid |
| 3 | Site Yellow | Amber construction-energy hero, bold sans-serif, tile categories |
| 4 | White Ledger | Minimal white, giant stat number as hero, clean ledger-style list |
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
- The gallery lives at gallery-option-c.html
- When building a new version, review the previous version for continuity
- Chicago flag palette: blue #0076C0, red #E31837, white #FFFFFF
- Prefer real-feeling placeholder data (Chicago street names, realistic timelines)
- Do not add JavaScript interactivity unless the version description calls for it
