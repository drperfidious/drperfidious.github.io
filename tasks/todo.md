# HORT 1230 Annuals Quiz 2 Repurpose

## Plan

- [x] Replace the tree species deck with the 15 annuals entries from the supplied Quiz 2 PDF, retaining photo identification.
- [x] Retheme the interface and manifest from Tree ID to Annuals ID, preserving photo controls.
- [x] Keep common/scientific-name scoring, split the two marigolds, and accept course/current scientific-name aliases.
- [x] Preserve the mobile layout and reveal course pronunciation cues and naming notes after answering.
- [x] Verify source integrity, run a local static-server smoke test, and exercise the quiz behavior in a browser.

## Review

Plan self-reviewed following the user's confirmation: preserve the existing photo game instead of replacing it with a name-clue/pronunciation test.

- Validated JavaScript syntax and manifest JSON, all 15 plant entries and their grading aliases, hybrid spacing/quotes, the Victoria Blue cultivar requirement, tree-answer rejection, and shuffled-deck coverage without an immediate boundary repeat.
- All 15 iNaturalist lookups returned photo observations. Million bells uses cultivated observations identified at genus level to avoid wild species results.
- Verified live photo display, another-photo loading, wrong-answer feedback, score update, pronunciation/naming-note reveal, and next-round reset in the in-app browser. No browser console errors.
- Checked the game at 390px phone width: no horizontal overflow. Inspected the rendered game and restored the browser viewport afterward.
- Static preview running at http://127.0.0.1:8766/; screenshot saved to /tmp/hort-quiz-render/annuals-preview.png. No commit, push, or deployment performed.

Known photo scope: Salvia farinacea photos do not verify Victoria Blue; cultivated Calibrachoa photos do not verify a named hybrid. These limitations are disclosed in the interface.

## Publication

- [x] Confirm GitHub Pages publishes the repository root from main and synchronize remote state.
- [x] Commit and push the annuals update to main.
- [x] Verify the GitHub Pages deployment and live annuals page.

Published application commit: 6e3f213. GitHub Pages run 39687532801 succeeded. Public index and manifest returned HTTP 200 and matched the local files exactly. The public page loaded an annual photo and enabled Check answer in the browser at https://drperfidious.github.io/.
