# Saved Deals — Take-home (Frontend Engineer Intern)

A single-screen "saved deals" app built with plain HTML, CSS, and vanilla JavaScript (no frameworks, no build step).

Open `index.html` in any modern browser.

## Features

- Hardcoded list of 5 product deals
- Each deal shows: name, current price, original price (struck through), and % off
- Click a deal → modal detail view with “Notify me when this drops below $X” input
- Loading state (simulated network delay)
- Empty state (use the “Show Empty” button in the header to demo it)

## Design decisions

### One design decision I’m proud of
I treated loading and empty states as first-class UI instead of afterthoughts. The list never just “appears” — there’s a short simulated load, and the empty state has a clear recovery action (“Load sample deals”). The modal also does lightweight validation so the notify input isn’t a silent no-op.

### One thing I’d do differently with more time
- Persist notify preferences (localStorage or a real backend)
- Add subtle enter/exit animations and better focus management (trap focus inside the modal)
- Extract the deal data and rendering into small, testable functions
- Make the layout more resilient on very small screens and add a proper skeleton loader instead of only a spinner

### Anything I’d want feedback on
- Whether the modal + validation approach feels right for a production “notify me” flow
- How much polish vs. clarity you’d expect at the intern level for a 1–2 hour exercise
- Any patterns you’d prefer for handling loading/empty states in a real codebase

## How to run

Just open `index.html` in a browser. No install or build required.
