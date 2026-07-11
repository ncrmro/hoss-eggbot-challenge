# 🥚 The HOSS EggBot Challenge

A challenge by the [Houston Open Source Society](https://houstonopensourcesociety.com/) (HOSS) — building a vibrant open source community in Houston, Texas. Join us on [Discord](https://discord.gg/FgGS5quF7P) or at our Wednesday 6 PM meetups.

> *"Revive the EggBot by any means necessary. Then make it draw something glorious on an egg."*

![The EggBot in all its glory](https://shop.emscdn.com/sites/eggbot/ebdlx_1600-2.jpg)

Somewhere out there is an [EggBot](https://egg-bot.com/) — a small, noble machine whose only purpose in life is to draw on eggs. Your mission is to get it up and running from **your own computer**, using **whatever means possible**, and plot the best egg design you can.

No preconfigured machines. No borrowing someone's already-working laptop. You, the EggBot, a USB cable of questionable vintage, and your wits.

## The Challenge

1. **Bring it up.** Install the EggBot software locally, connect over USB, and prove the machine obeys you.
2. **Calibrate.** Pen height, egg alignment, plot bounds. A wobbly egg is a humbling teacher.
3. **Design.** Create an original egg artwork (SVG). Hand-drawn, coded, generative, AI-assisted (disclose it!) — all fair game.
4. **Plot.** Make the EggBot draw it on an egg (or egg-shaped object — see Tracks below).
5. **Automate.** Build an **agent skill** (Claude, Gemini, Codex, pi — dealer's choice) that can handle any or all of the lifecycle: full setup, teardown, and generating new designs. The dream: an agent that can take a fresh machine to a finished egg.
6. **Submit.** Egg photo + SVG + agent skill + proof it ran from *your* machine.

"Whatever means possible" is the spirit of this challenge. The hardware is provided (see below) — the chaos is in the software. Running Inkscape in a VM because your OS hates you? Respect. Agent wrote your udev rules? Iconic.

## Know Your Enemy (Hardware Facts)

| Thing | Spec |
|---|---|
| Power supply | **9 V DC, center-positive, ≥1 A** (OEM is 9 V / 1.5 A, 2.1 × 5.5 mm barrel plug) |
| USB (original / EBB ≤ v2.0) | USB-A to **mini-B** |
| USB (EBB v2.5+) | USB-A to **micro-B** |
| Controller | EiBotBoard (EBB) — open-source USB motor control board |
| Software | Inkscape + EggBot extensions, installed via the [AxiDraw installer](https://wiki.evilmadscientist.com/Installing_software) (v3.9.4 recommended for EggBot) |

⚠️ USB is data only — the EggBot still needs its own 9 V supply. Don't update the EBB firmware unless you truly must, and never while USB connection problems are unresolved.

## What's Provided

HOSS supplies the shared hardware — you bring your laptop and your wits:

- 🤖 The **EggBot** itself (with its 9 V PSU)
- 🔌 **USB cable**
- 🖊️ **Markers**
- 🥚 **Eggs**

Everything else — software setup, design, and agentic tooling — is on you.

## Tracks

- **Classic Egg + Best Design:** plot on a real egg; judged on the best design. Maximum charm, maximum fragility.
- **Open Source Model + Agentic Tooling:** get there using open source models and agentic tooling — judged on how much of the setup → design → plot loop your agent handles.
- **Wildcard:** absurd, funny, experimental. If it was plotted by the EggBot, it counts.

## Proof of Local Bring-Up (required)

To keep everyone honest, each submission must include:

- 📷 Photo/video of your computer connected to the EggBot
- 🖥️ Screenshot of the EggBot extension/controls in Inkscape
- ✏️ A successful test/calibration plot
- 📄 The final SVG used
- 🥚 Photo of the finished egg

Bonus points for a timelapse, notes on failed attempts, and tales of hardship.

## Rules

**Design**
- Final design must be plotted *by the EggBot*.
- Original or properly-licensed artwork only. AI-assisted is fine — disclose it.
- Multiple colors allowed; every color pass must be plotted by the machine.
- No hand-finishing the plotted artwork. Wiping smudges is fine.

**Setup**
- The EggBot must be controlled from your local machine — not someone else's preconfigured rig.
- Debugging help, official docs, and community notes are all allowed.
- Windows, macOS, or Linux. Teams of 1–3.

**Fairness**
- Everyone gets the same plotting window.
- Broken eggs may be replaced, but the clock keeps running (unless shared equipment broke it).

## Scoring (100 points)

| Category | Points |
|---|---|
| Local setup success (machine obeys your laptop, clean test plot, docs) | 15 |
| Design quality (impact, originality, use of egg curvature, humor/elegance) | 25 |
| Technical execution (clean lines, registration, curve handling) | 20 |
| **Agent skills** (a Claude/Gemini/Codex/pi/etc. skill that automates setup, design generation, plotting, and/or teardown — see [CONTRIBUTING.md](CONTRIBUTING.md)) | 20 |
| Craft & presentation (polished egg, colors, photo) | 10 |
| Reproducibility (usable SVG, process notes, re-plottable by others) | 10 |

**Bonus awards:** Best First Successful Plot · Most Beautiful Failure · Best Use of One Line · Funniest Egg · Best Recovery From Disaster · People's Choice.

## Judging Philosophy

Reward entries that *understand the machine*: continuous linework, restraint with filled areas (smear city), intentional use of symmetry and rotation, designs that feel like they belong **on an egg** — not a flat page bent around one.

> A simple, elegant, perfectly plotted egg beats a complex design that turns into a smudged mess.

## How to Submit

Submissions are **fork + pull request only** — see [CONTRIBUTING.md](CONTRIBUTING.md) for the full workflow. Short version:

1. Fork this repo and branch.
2. Copy [SUBMISSION_TEMPLATE.md](SUBMISSION_TEMPLATE.md) into `submissions/<your-team-name>/`.
3. Add your SVG, photos, agent skill(s), and notes.
4. Open a PR titled `Submission: <your-team-name>`. The gallery judges you now.

Good luck. May your pen stay down and your eggs stay whole. 🐣
