# Morning Board

A frame-friendly home dashboard inspired by Wes Bos’s [photo-frame-dashboard](https://github.com/wesbos/photo-frame-dashboard), designed for a 1920 × 1080 landscape display.

## What is ready

- Live local forecast from the National Weather Service for ZIP 45103 (Batavia, Ohio), with a Cincinnati radar loop.
- Live public Clermont Northeastern district events in a scrollable seven-day agenda; the ParentSquare calendar subscription URL still needs to be added.
- A special-reminders card for occasional school requests such as bringing show and tell; routine prep checklist removed.
- Weekday leave-for-bus countdown, set to 8:15 a.m., with a spoken reminder that can be turned off if the frame’s speech engine supports it.
- BusZone countdown and Alexa announcement status; live BusZone tracking remains on the phone because this frame reports Google Play services are unsupported.
- Layout adapts to a phone or tablet for editing.

Open `index.html` in a modern browser. The page stores its editable agenda, special reminders, and display preferences in that browser’s local storage. Weather refreshes automatically when the page has internet access; the larger radar image refreshes every five minutes.

## Connections still to set up

The district agenda reads public event data from the Clermont Northeastern website. ParentSquare calendar subscriptions and teacher messages are not imported yet. The frame firmware reports that Google Play services are unsupported, so BusZone's live map works on the phone instead. Alexa announcements will need a relay that can read the phone’s BusZone notifications; Home Assistant is a candidate for a later phase. The optional frame voice reminder uses browser speech synthesis, if the frame’s speech engine supports it.

The forecast and radar use public National Weather Service endpoints. No account credentials or API keys are included in this package.

