# LUMIVERSION · Astaxanthin Decision Studio

Interactive demo of LUMIVERSION's decision support for *Haematococcus pluvialis* astaxanthin production: when to move cultures from green to red, when to harvest, and when to hold back.

**Live demo:** https://lynee1.github.io/Astaxanthin-demo-ENG/

## What the demo shows

- **Batch planner**: recommended transfer and harvest days for a set of process conditions, with the likely range.
- **Safeguards**: how recommendations step down to conservative advice, or hand the decision to operators, during heatwaves, dull weather, missed measurements, equipment faults or suspected contamination.
- **Your data**: upload batch records as CSV; columns are matched, units and gaps are checked, and each batch's harvest window is estimated when there are enough measurements.
- **Business case**: annual output, cost per kilogram and profit for current practice against the optimised plan.
- **Pilot programme**: how a 16-week pilot runs alongside current practice before anything changes in production.

Figures are model estimates with example settings until the model is calibrated on a producer's own batches. Sample datasets in the demo are synthetic.

## Privacy

This is a static website. All calculations run in the visitor's browser; uploaded files are never sent anywhere. Saved business-case scenarios are kept only in the visitor's own browser.

## Run locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Publish with GitHub Pages

Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`.

## Maintenance

To show an email button on the Pilot page, set `CONTACT_EMAIL` near the top of the script in `index.html`.

## Licence

© 2026 LUMIVERSION. All rights reserved.
Fonts: Barlow, SIL Open Font License 1.1 (see `fonts/LICENSE-OFL.txt`).
