# maintance-calendar

Interactive prototype of the **SAP for Me → Calendar** page with a **Create event** flow and a **customer hierarchy selector**.

Open `index.html` in a browser — it's a single self-contained file (React + Babel via CDN, SAP Horizon styling, the "72" font).

## What's in it

- **SAP for Me shell** — shell bar, left navigation (Calendar active), page header, and the week-view planning calendar rebuilt from the live SAP for Me calendar.
- **Customer hierarchy selector** — next to the "Calendar" page title (`Calendar | Scott Electronics Global ▾`). Opens a popover list of accessible entities, updates the header on select, and follows the [customer hierarchy guidelines](https://boyanpetkovsap.github.io/customer-hierarchy/) (combobox/listbox ARIA, chevron rotation, polite live-region announcement, focus returned to the trigger).
- **Create event flow** — the primary **Create event** button opens a popover form with: event name, all-day toggle, start date/time, end date/time, event type (6 SAP event types), and tags. On submit the event is placed on the calendar grid, colored by its event type and positioned by date/time (all-day events span to the all-day row).

Event types and colors, the seeded events, and the week shown (29 Nov – 5 Dec 2026) mirror the SAP for Me calendar reference.
