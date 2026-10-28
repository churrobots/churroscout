# Scouting tutorial plan

The student learns FRC scouting and data analysis by building ChurroScout, our scouting analysis tool, step by step. Concepts (`C1`, `C2`, …) are explained in `CONCEPTS.md`. The agent teaches each one just-in-time, following `AGENTS.md`.

**Main goal:** a one-screen **pre-match brief** the drive team uses before every qualification match (Phase 6).
**Second goal:** a **pick list** for alliance selection, in case we're a captain (Phase 7).

Each step lists the concepts it introduces, what the student builds, and how we know it's done. 🧑‍🏫 means a coach must be present for that step.

Our data lives in `data-2026/`. It is **read-only** (see `AGENTS.md`). If it's missing when a step needs it, stop and get a coach.

---

## Phase 0 · Why we scout (no code)

Goal: the student can explain what scouting is for and how the 2026 game turns into numbers.

1. **What scouting is for.** Talk through the two jobs of scouting. Ask the student what they think the drive team needs to know before a match. *Concepts: C1.*
   Done when: the student can name both jobs and says why match strategy comes first.
2. **How an event works.** Walk through quals, ranking points, alliance selection, and playoffs. If possible, look at a real 2026 event on The Blue Alliance together. *Concepts: C2.*
   Done when: the student can explain why rank doesn't always equal robot quality.
3. **The game as data.** With the 2026 game manual open, list how robots earn points and RP in auto, teleop, and endgame. Pick the 3 that matter most. *Concepts: C3.*
   Done when: the student has a short written list, saved as `notes/game-breakdown.md`.
4. **Facts vs. opinions.** Sort a list of example scouting fields into objective and subjective. *Concepts: C4.*
   Done when: the student can turn one subjective field into a more objective one.
5. 🧑‍🏫 **Set up the tools.** Install Python, Jupyter, and pandas (a coach confirms the setup steps for the team laptops). Create the folders `churroscout/`, `notebooks/`, and `output/`. Open a first notebook and print "hello."
   Done when: a notebook cell runs, and the student has made their first commit.

## Phase 1 · Collecting good data (light code)

Goal: the student understands where our data comes from and how it can go wrong.

1. **Kinds of scouting.** Compare match, pit, and super scouting. If a coach has pit notes or a paper form from 2026, look at them. *Concepts: C5.*
2. **Judge our form.** Look at the column names in `data-2026/` (the agent may list them). For each one, ask: what question does it answer? Would you keep it? *Concepts: C6.*
   Done when: the student has written a short "keep / change / cut" list for our form in `notes/form-review.md`.
3. **Where data goes wrong.** Brainstorm what could go wrong for a scout at an event. Predict what kinds of mistakes we'll find in our data in Phase 2. *Concepts: C7.*
   Done when: the student has a list of predicted mistakes to check later.

## Phase 2 · Meet our data

Goal: a clean table of our 2026 scouting data that we trust, and a document that explains it.

1. **Load it.** Write `churroscout/load.py` with a function that reads the raw data into a DataFrame. In `notebooks/01_explore.ipynb`, load it and look at `.head()`, the number of rows, and the column names. *Concepts: C8, C10.*
   Predict first: how many rows do you expect? (Teams × matches each.)
2. **Write the data dictionary.** Create `DATA_DICTIONARY.md` with one line per column: name, meaning, units or allowed values, gotchas. Ask a coach about anything unclear. *Concepts: C9.*
   Done when: every column is described, and nothing is guessed.
3. **Find the problems.** Look for the mistakes predicted in Phase 1: unknown team numbers, duplicate rows, missing matches, impossible values. Count each kind. *Concepts: C11.*
4. **Clean it.** Write `churroscout/clean.py`: a function that takes the raw DataFrame and returns a clean one, plus a small corrections table for known fixes. Print how many rows were changed or dropped, and why. *Concepts: C11.*
   Done when: re-running the notebook from scratch gives the same clean table every time.
5. 🧑‍🏫 **Connect to The Blue Alliance.** A coach provides the API key. Put it in `.env` (already in `.gitignore`). Write `churroscout/tba.py` to fetch an event's match results and save them to `output/` so they work offline. *Concepts: C21.*
6. **Check against official scores.** For each alliance in each match, add up our scouted numbers and compare them to the official score breakdown. Make a list of the matches with the biggest gaps. *Concepts: C12.*
   Done when: the student can say roughly how accurate our scouting is and name one likely cause of the big gaps.

## Phase 3 · Describing one robot

Goal: a "team card" that sums up any robot in a few honest numbers.

1. **Group by team.** In `churroscout/metrics.py`, summarize each team's main scoring stat. *Concepts: C13.*
   Predict first: which team will come out on top?
2. **Average vs. median.** Compute both. Find the team where they're farthest apart and look at its matches. *Concepts: C14.*
3. **Floor and ceiling.** Add 25th and 75th percentiles. Compare with how our old tool used the 75th percentile (`git show f71207d~1:churroscout.ipynb`). *Concepts: C15.*
4. **Consistency.** Add a spread measure. Find the most and least consistent robots. *Concepts: C16.*
5. **How many matches?** Add the match count to every summary, and flag teams with too few matches. *Concepts: C17.*
6. **Outliers.** Find each team's weirdest matches, then look at the scout notes (and video, if possible) to explain them. Decide together what to do with each kind of outlier, and write down the rule. *Concepts: C18.*
7. **Yes/no tasks.** Add success rates for things like climbing, shown as "6/8 (75%)." *Concepts: C19.*
8. **Recent form.** Add a "last N matches" view, and find a team that clearly improved or got worse. *Concepts: C20.*
9. **The team card.** Put it together: one function that takes a team number and returns a short summary. Show it for our team and two others.
   Done when: a teammate who watched the event agrees the cards "look right," or the student can explain why they don't.

## Phase 4 · Outside data

Goal: our scouting, OPR, and EPA side by side, and an understanding of when to trust which.

1. **OPR.** Compute OPR from the official results saved in Phase 2 (the old tool's `calculate_power_ratings` is a reference). Before writing code, explain OPR using the dinner-bill idea. *Concepts: C22.*
2. **EPA.** Pull Statbotics EPA for every team at the event. *Concepts: C23.*
3. **Compare.** Put our scouted numbers, OPR, and EPA in one table. Find the 3 biggest disagreements and investigate each one. *Concepts: C24.*
   Done when: the student has a short written explanation for each disagreement.

## Phase 5 · Showing it clearly

Goal: charts that answer a question in two seconds.

1. **Chart menu.** Make one bar chart, one box plot, and one scatter plot from our data. For each, say what question it answers. *Concepts: C25.*
2. **Busy-reader test.** Make a one-screen view of a team card. Show it to someone on the drive team for 15 seconds, then ask what they remember. Revise it. *Concepts: C26.*

## Phase 6 · Pre-match briefs (main goal)

Goal: given a match number, produce a one-screen brief the drive team actually uses.

1. **Predict a match.** In `churroscout/predict.py`, take 3 red and 3 blue teams and predict each alliance's score. Test it on past matches: how often did we pick the right winner? *Concepts: C27.*
2. **How sure are we?** Add a bad-day / good-day range for each alliance. *Concepts: C28.*
3. **Our alliance.** For our partners, show each robot's strengths and suggest roles. *Concepts: C29.*
4. **The opponents.** For each opponent, show its biggest threat and weak spots. *Concepts: C30.*
5. **Defense check.** Add a simple "is defense worth it?" calculation and a suggested target. *Concepts: C31.*
6. **RP goals.** Add the bonus-RP picture: which bonus RPs are realistic for us this match? *Concepts: C32.*
7. **Build the brief.** Create `notebooks/match_brief.ipynb` (or a script) that takes a match number, looks up the teams from the schedule, and produces the brief in `output/`. Keep it to one phone screen. *Concepts: C33.*
8. 🧑‍🏫 **Drive team review.** Show briefs for 3 past matches to the drive coach and drivers. Write down what they used, what they ignored, and what they wished they had. Revise.
9. **Post-match check.** Add a way to compare each brief's prediction to the real result, and a place for a one-line note. Run it on the past matches. *Concepts: C34.*
   Done when: the drive team says they'd use the brief at an event.

## Phase 7 · Alliance selection (second goal)

Goal: a pick list that picks partners who complement our robot.

1. **How the draft works.** Walk through alliance selection with a real 2026 event's results on The Blue Alliance. *Concepts: C35.*
2. **Our needs.** With the drive team, list our robot's strengths and weaknesses, and turn them into needs and wants. *Concepts: C36.*
   Done when: there's a written list in `notes/alliance-needs.md`.
3. **Fit score.** In `churroscout/picklist.py`, score each team on how well it fills our needs, not just its raw points. *Concepts: C37.*
4. **Red flags.** Add reliability info (breakdowns, fouls, no-shows) and a do-not-pick list. *Concepts: C38.*
5. **Tiers.** Sort teams into tiers quickly, then order each tier. Make the list about 23 teams long. *Concepts: C39.*
6. **Simulate.** Use the predictor from Phase 6 to compare possible alliances. *Concepts: C40.*
7. **Second-pick list.** Make a separate ranking for round 2 that values role fit, reliability, and hidden gems. *Concepts: C41.*
8. 🧑‍🏫 **Mock pick-list meeting.** Using a past 2026 event, run a practice meeting with the team. Compare the final list to EPA rankings and check the big differences. *Concepts: C42.*
   Done when: the team has run one mock meeting and written down what to do differently next time.

## Phase 8 · Event day

Goal: the whole flow works under event pressure.

1. **Offline-ready.** Make sure everything runs with no internet, using saved TBA and Statbotics data. *Concepts: C43.*
2. **Backups and handoff.** Set up regular backups, and write a short "how to run ChurroScout" guide so more than one person can run it.
3. 🧑‍🏫 **Dress rehearsal.** Replay a past event match by match: add the data, produce each brief on time, and update the pick list. Time each step.
   Done when: a brief is ready within the time between our matches, and a second student can run the pipeline alone.
