# Morning Board

A frame-friendly home dashboard inspired by Wes Bos’s [photo-frame-dashboard](https://github.com/wesbos/photo-frame-dashboard), designed for a 1920 × 1080 landscape display.

## What is ready

- Live local forecast from the National Weather Service for ZIP 45103 (Batavia, Ohio), with a Cincinnati radar loop.
- Scrollable seven-day agenda, editable directly on the dashboard.
- School morning preparation checklist with saved completion state.
- BusZone panel and Alexa announcement plan, ready for a future connection.
- Layout adapts to a phone or tablet for editing.

Open `index.html` in a modern browser. The page stores its editable agenda, checklist, and display preferences in that browser’s local storage. Weather refreshes automatically when the page has internet access; the radar image refreshes every five minutes.

## Connections still to set up

Calendar entries are sample data until a calendar connection is configured. The BusZone panel does not yet receive live bus location or app alerts, and the Alexa panel is a display-only announcement plan. Getting BusZone notifications to an Echo will need a relay that can read the phone’s BusZone notifications; Home Assistant is a candidate for a later phase. The photo frame has not been changed as part of preparing this dashboard.

The forecast and radar use public National Weather Service endpoints. No account credentials or API keys are included in this package.

