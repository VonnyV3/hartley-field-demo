# Hartley Field Capture — demo

Single-file HTML field capture demo for Hartley Concrete and Hartley
Dirtworks. Everything lives in `index.html`; it deploys to GitHub Pages by
pushing to `main`.

## Standing rules

- **The CONFIG block is the only place data lives.** ROSTER, CREWS, JOBS,
  FLAT_EL, FND_IT and friends stay in the CONFIG block at the top of
  `index.html` — never scatter data into the form code.
- **Crew-to-form assignments in ROSTER are unconfirmed** — confirm with the
  dig foreman (he runs dispatch; the field super and the scheduler support him).
- **JOBS is sample data.** Real lots carry real addresses and never go into
  this public repo.
- **No real employee names and no real lot street addresses** in anything
  under field-demo or anywhere else that publishes publicly. Use pseudonyms
  for people and registry-checked fabricated identifiers for lots (scan
  addresses, lot/block keys AND house numbers against the registry before
  pushing — a swapped street name with a real house number is not scrubbed).
- **Commit and push after every completed change.**

## Operations context

How scheduling actually works (the 10 Sept 2026 interview) lives in the
PRIVATE main repo: `docs/operations_interview_2026-09-10.md` — it names
employees, which this public repo must not.
