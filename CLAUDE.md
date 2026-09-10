# Hartley Field Capture — demo

Single-file HTML field capture demo for Hartley Concrete and Hartley
Dirtworks. Everything lives in `index.html`; it deploys to GitHub Pages by
pushing to `main`.

## Standing rules

- **The CONFIG block is the only place data lives.** ROSTER, CREWS, JOBS,
  FLAT_EL, FND_IT and friends stay in the CONFIG block at the top of
  `index.html` — never scatter data into the form code.
- **Crew-to-form assignments in ROSTER are unconfirmed pending Enrique.**
- **JOBS is sample data.** Real lots carry real addresses and never go into
  this public repo.
- **Commit and push after every completed change.**
