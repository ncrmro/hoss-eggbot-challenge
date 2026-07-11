# Contributing / Submitting an Entry

All submissions happen via **fork + pull request**. No direct pushes, no emailing zip files, no handing over a USB stick taped to an egg.

## Submission workflow

1. **Fork** this repository to your own account.
2. **Create a branch** in your fork, e.g. `submission/<your-team-name>`.
3. **Create your submission directory:**

   ```
   submissions/<your-team-name>/
   ├── README.md          # copy of SUBMISSION_TEMPLATE.md, filled out
   ├── design.svg         # the final SVG you plotted
   ├── photos/            # finished egg, local-machine proof, calibration plot
   ├── skills/            # your agent skill(s) — see below
   └── notes/             # optional: process notes, timelapse links, war stories
   ```

4. **Fill out the template.** Copy [SUBMISSION_TEMPLATE.md](SUBMISSION_TEMPLATE.md) into your directory as `README.md` and complete every field.
5. **Open a pull request** against `main`. Title it `Submission: <your-team-name>`.
6. Judges review the PR. Discussion happens in PR comments. Merged = officially entered.

## Agent skills (judged!)

Part of your score comes from **agentic skill**: build an agent skill — for Claude, Gemini, Codex, pi, or any agent framework of your choosing — that automates some or all of the EggBot lifecycle. The more of the loop your agent can run, the better:

- **Setup** — install Inkscape + EggBot extensions, detect the EBB over USB, verify communication, run a calibration plot
- **Design generation** — generate new plottable egg designs (SVGs) on demand: generative art, themed prompts, polar/symmetric layouts that respect egg curvature
- **Plotting process** — drive the plot itself: pen changes, multi-color passes, resume-after-disaster
- **Teardown** — pen up, park the motors, disable steppers, leave the machine ready for the next victim

A skill that handles *any* of these earns points; a skill that handles *all* of them earns glory. Include your skill files in `submissions/<your-team-name>/skills/` with a short README explaining:

- Which agent(s) it targets (Claude/Gemini/Codex/pi/other)
- What parts of the lifecycle it covers
- How to install/invoke it
- Proof it worked (transcript, recording, or output artifacts)

Skills will be judged on how much of the process they genuinely automate, how reproducible they are on someone else's machine, and how well they handle the EggBot's real-world jank.

## Ground rules for PRs

- One PR per team entry. Push updates to the same branch before the deadline.
- Only touch files inside your own `submissions/<your-team-name>/` directory.
- Keep binary files reasonable: compress photos, link out to videos rather than committing them.
- Be kind in PR comments. We are all just people trying to make robots draw on eggs.

## Non-submission contributions

Fixes to the rules, docs, or repo tooling are welcome too — open a regular PR and explain the change.
