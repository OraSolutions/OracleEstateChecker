# Oracle Classic Estate Check

An adaptive self-diagnostic for teams running Oracle E-Business Suite,
PeopleSoft, Siebel or JD Edwards.

Since 28 May 2026 Oracle ships a monthly Critical Security Patch Update (CSPU)
in addition to the four quarterly Critical Patch Updates (CPU). Customer managed
estates went from four patch events a year to twelve. This check helps a support
team work out whether its run model absorbed that change.

Twelve questions, scored out of 24, adapted to the applications the respondent
runs and to where those applications are hosted.

## Running locally

Open `index.html` in any browser. No build step, no dependencies, single file.

## Before publishing

Two constants at the top of the `<script>` block in `index.html`:

```js
const LINK_EVENT = "#";   // scheduling page for the AI World meeting room
const BOOTH      = "";    // booth number in the AI World Hub
```

Left unset, both render as visible gold placeholders, so the tool cannot go
live with a dead button by accident.

Also confirm DXC brand and marcom approval for public hosting.

## Design system

Built on the DXC Oracle AI Agent Portfolio web design system: token layer,
fluid type scale, six named surfaces, act rail, journey stepper, maturity
bars, stage cards and drill-down sheet.

This follows the portfolio web system, not the DXC PPTX generation rules.
The portfolio itself already departs from those rules, and GT Standard L
Extended cannot lawfully be embedded as base64 in a public file. Headings
are Inter 800 with tightened letter-spacing, as in the portfolio.

Inter is bundled as base64 in five weights (300, 400, 600, 700, 800).
The page makes no network requests of any kind and works offline.

## Privacy

Answers are scored in the browser. Nothing is collected and nothing is
transmitted. Of the three closing options, only option 1 shares the result.
Option 2 deliberately carries no score, no pattern and no estate detail,
not even in the subject line.

## Project

AIWorld26 Marcom, DXC Oracle Practice.
