# World Cup 2026 — Interactive Predictor & Tracker

A single self-contained web page for predicting and following the 2026 FIFA World Cup:
enter group-stage scores, decide who qualifies, click your way through the knockout
bracket, and watch it flow to the final — with model-based odds on every match.

**▶ Open it: https://porcineoctopus-sudo.github.io/world-cup-2026-tracker/**

Works on phones and desktops. Everything runs in your browser — there's no server,
no account, and nothing is uploaded.

## How to use it

1. **Group stage.** Each of the 12 groups has its six matches with score boxes. Type
   the scores and the standings (points, goal difference, goals for) update live. The
   top two of each group are highlighted as qualifiers; the best third-placed teams are
   highlighted too.

2. **Qualification — who goes through.** Open this collapsible section to confirm who
   advances. It's pre-filled from your scores, but real tournaments break ties with
   things this tool deliberately doesn't track (head-to-head, fair-play points, drawing
   of lots), so you can:
   - force each group's **1st / 2nd / 3rd** placing, and
   - pick the official **eight best third-placed teams** (exactly eight).

3. **Knockout bracket.** The Round of 32 is seeded automatically from the group results
   and the eight third-placed teams — including FIFA's official rule for *which* third
   goes into *which* match. Click a team to advance it; the pick flows through to the
   final, and the champion is shown at the end. Click again to undo.

4. **It saves itself.** Your scores and picks are stored in your browser, so you can
   close the tab and come back later. The **Reset all** button clears everything.

## Where the odds come from

Before you enter any results, every team carries a **strength** rating seeded by a
statistical model of historical World Cup performance. From those ratings the page
computes, right in your browser:

- each team's chance of advancing (shown as a small % next to its name), and
- win probabilities for every knockout match (the % beside each team in the bracket).

These are the model's starting estimates. As you enter scores and click winners, the
bracket reflects **your** inputs — the percentages are just there to suggest the
favourite in any matchup you haven't decided yet.

## Privacy

The page is one static HTML file. It makes no network requests, sets no cookies, and
sends nothing anywhere. Your scores and picks live only in your own browser's local
storage (and are specific to this page's address). Clearing your browser data or
hitting **Reset all** removes them.

## Notes

- The bracket structure and the third-place allocation follow FIFA's published 2026
  format (12 groups; top two of each group plus the eight best third-placed teams make
  the 32-team knockout round).
- This page is a generated, self-contained snapshot. Predictions reflect the model at
  the time it was published.
