# Hartley Field Capture — demo

Single-file HTML field capture demo for Hartley Concrete and Hartley
Dirtworks. Everything lives in `index.html`; it deploys to GitHub Pages by
pushing to `main`.

## Standing rules

- **The CONFIG block is the only place data lives.** ROSTER, CREWS, JOBS,
  FLAT_EL, FND_IT and friends stay in the CONFIG block at the top of
  `index.html` — never scatter data into the form code.
- **Crew-to-form assignments in ROSTER are unconfirmed** — confirm with
  the dig foreman (dig foreman, runs dispatch), with the field super and the scheduler supporting.
- **JOBS is sample data.** Real lots carry real addresses and never go into
  this public repo.
- **No real employee names and no real lot street addresses** in anything
  under field-demo or anywhere else that publishes publicly. Use pseudonyms
  for people and registry-checked fabricated identifiers for lots (scan
  addresses, lot/block keys AND house numbers against the registry before
  pushing — a swapped street name with a real house number is not scrubbed).
- **Commit and push after every completed change.**

## Operations — how scheduling actually works (the scheduler interview, 10 Sept 2026)

These correct assumptions the project had been building on.

- **The Master Job Schedule is a back-office job list and completion log,
  NOT a schedule.** Crews never look at it. the scheduler enters Builder Dig Date
  when the builder email arrives; every other date is entered after the
  work is done. Zero future dates is by design.
- **Dispatch is done by the dig foreman, the dig foreman, on paper, at the shop.**
  the field super and the scheduler support him. Each downstream phase lead (utilities,
  backfill, flatwork) sequences their own work off the dig. Written down at
  a Friday morning meeting. Nothing digital exists.
- **the backfill lead**: backfill lead, runs Tamarack excavation, owns columns K–N in
  the schedule, comfortable with technology. the scheduler owns the earlier columns.
  the overseer oversees and occasionally enters.
- **Completion chain**: crew finishes → texts one of ~10 group chats → the scheduler
  or the backfill lead types into the sheet → the office verifies field paperwork against
  the sheet → bills. the office is blocked when the sheet lags.
- **Builder scheduling emails** arrive weekly, one week ahead, as mass
  emails to all trades. Toll and Alturas send Monday; Avimor Friday or
  Monday. the scheduler hand-copies lot/block/address; transcription errors here are
  the #1 reason the office calls him.
- **Scope varies per job.** Tresidio: Hartley does excavation only, another
  contractor does foundation, Hartley sometimes returns for flatwork. Toll
  at Valor: Hartley excavation, Riverstone foundation. The builder email
  states what Hartley is doing.
- **Crews clock in/out at the shop** (find out if digital). Per-job hours
  are self-reported on paper; the scheduler called the splits unrealistic. Day total
  is measured; per-lot is allocation.
- **Dig capacity**: 3 operators, 2–3 houses each per day.
- **Partial flatwork pours in winter**; return weeks later. Column Q is
  Y/N/P.
- **the scheduler also maintains**: permitting sheet (daily), job count for the exec
  (weekly), six-month sales forecast. Future modules, not now.
- **The shop wants a TV showing the schedule.**
