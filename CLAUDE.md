# Hartley Field Capture — demo

Single-file HTML field capture demo for Hartley Concrete and Hartley
Dirtworks. Everything lives in `index.html`; it deploys to GitHub Pages by
pushing to `main`.

## Standing rules

- **The CONFIG block is the only place data lives.** ROSTER, CREWS, JOBS,
  FLAT_EL, FND_IT and friends stay in the CONFIG block at the top of
  `index.html` — never scatter data into the form code.
- **Crew-to-form assignments in ROSTER are unconfirmed** — confirm with
  Alejandro (dig foreman, runs dispatch), with Enrique and Kyle supporting.
- **JOBS is sample data.** Real lots carry real addresses and never go into
  this public repo.
- **Commit and push after every completed change.**

## Operations — how scheduling actually works (Kyle interview, 10 Sept 2026)

These correct assumptions the project had been building on.

- **The Master Job Schedule is a back-office job list and completion log,
  NOT a schedule.** Crews never look at it. Kyle enters Builder Dig Date
  when the builder email arrives; every other date is entered after the
  work is done. Zero future dates is by design.
- **Dispatch is done by Alejandro, the dig foreman, on paper, at the shop.**
  Enrique and Kyle support him. Each downstream phase lead (utilities,
  backfill, flatwork) sequences their own work off the dig. Written down at
  a Friday morning meeting. Nothing digital exists.
- **Adrian**: backfill lead, runs Tamarack excavation, owns columns K–N in
  the schedule, comfortable with technology. Kyle owns the earlier columns.
  Zach oversees and occasionally enters.
- **Completion chain**: crew finishes → texts one of ~10 group chats → Kyle
  or Adrian types into the sheet → Jonnie verifies field paperwork against
  the sheet → bills. Jonnie is blocked when the sheet lags.
- **Builder scheduling emails** arrive weekly, one week ahead, as mass
  emails to all trades. Toll and Alturas send Monday; Avimor Friday or
  Monday. Kyle hand-copies lot/block/address; transcription errors here are
  the #1 reason Jonnie calls him.
- **Scope varies per job.** Tresidio: Hartley does excavation only, another
  contractor does foundation, Hartley sometimes returns for flatwork. Toll
  at Valor: Hartley excavation, Riverstone foundation. The builder email
  states what Hartley is doing.
- **Crews clock in/out at the shop** (find out if digital). Per-job hours
  are self-reported on paper; Kyle called the splits unrealistic. Day total
  is measured; per-lot is allocation.
- **Dig capacity**: 3 operators, 2–3 houses each per day.
- **Partial flatwork pours in winter**; return weeks later. Column Q is
  Y/N/P.
- **Kyle also maintains**: permitting sheet (daily), job count for Taylor
  (weekly), six-month sales forecast. Future modules, not now.
- **The shop wants a TV showing the schedule.**
