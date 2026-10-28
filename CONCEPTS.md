# Scouting concepts

This is the mentor's reference for every concept in the scouting tutorial. Students don't read this file. The agent explains each concept just-in-time, in plain words, and checks understanding with the **Check yourself** question. See `AGENTS.md` for how.

Each concept has:

- **Phase / Needs:** where it shows up in `TUTORIAL_PLAN.md`, and which concepts should come first.
- **The idea:** the plain-language explanation (aim for about 150 words when teaching).
- **Analogy:** one everyday comparison. If it doesn't land, invent a different one.
- **Why it matters on the field:** how it helps the drive team or the pick list.
- **Watch out for:** common mix-ups.
- **Check yourself:** the question the student must answer in their own words before the concept counts as understood.

Game-specific details (point values, ranking point rules, endgame rules) come from the **official 2026 game manual**, not from this file.

---

## Phase 0 · Why we scout

### C1 · Why we scout
**Phase:** 0 · **Needs:** none

**The idea:** Scouting means collecting information about every robot at an event so we can make better decisions. It has two jobs. **Job 1, match strategy:** before each qualification match, our drive team meets our 2 partners and makes a plan to beat 3 opponents. Good scouting tells them who's good at what. **Job 2, alliance selection:** if we're a top-8 team, we pick partners for the playoffs. Good scouting tells us who fits best with our robot. Job 1 happens every match, so it's our main focus.

**Analogy:** A sports team watching film of the other team before a game. You don't need to know everything, just what helps you win *this* game.

**Why it matters on the field:** Strategy can win matches you'd otherwise lose. A plan like "you score, we defend their best shooter" only works if you know who their best shooter is.

**Watch out for:** Thinking scouting is only about picking. Most teams never become a captain, but every team plays 10+ qual matches.

**Check yourself:** What are the two jobs of scouting, and which one will our team use more often? Why?

### C2 · How an event works
**Phase:** 0 · **Needs:** C1

**The idea:** An FRC event has two parts. **Qualification matches ("quals"):** you're randomly paired with 2 partners against 3 opponents, and partners change every match. You earn **ranking points (RP)** for winning and for hitting bonus goals. Teams are ranked by average RP. **Playoffs:** the top 8 teams become **alliance captains** and pick 2 or 3 partners each, in a "snake draft" (1→8, then 8→1). Then the 8 alliances play a double-elimination bracket.

**Analogy:** Quals are like a school group project where the teacher assigns new groups each week. Playoffs are like the end of the year, when you get to pick your own group.

**Why it matters on the field:** In quals, you can't choose your partners, so you plan *around* them. In playoffs, you choose partners, so you need a pick list.

**Watch out for:** Thinking rank equals robot quality. Rankings depend a lot on luck (who your partners were). This is why we scout instead of just reading the rankings.

**Check yourself:** Why might a really good robot be ranked 20th after quals?

### C3 · The 2026 game, as data
**Phase:** 0 · **Needs:** C2

**The idea:** Every game has things robots do that earn points or ranking points: scoring game pieces, doing tasks in autonomous, and an endgame task. To scout well, we break the game into **things we can count or check**. For each one, ask: "Does this win matches or earn RP?" and "Can a scout in the stands see it reliably?" The official game manual has the exact rules and point values. The columns in `data-2026/` show what our team actually scouted.

**Analogy:** A basketball stat sheet. Points, rebounds, and assists are listed because they decide games and you can count them.

**Why it matters on the field:** If we scout the wrong things, the brief is full of numbers that don't help the drive team.

**Watch out for:** Scouting everything. More boxes on a form means more mistakes. Pick the few things that matter most.

**Check yourself:** Name the three things in the 2026 game that matter most for winning or RP, and say how a scout would measure each one.

### C4 · Objective vs. subjective data
**Phase:** 0 · **Needs:** C3

**The idea:** **Objective** data is a fact anyone would agree on: "scored 12 fuel," "climbed: yes." **Subjective** data is an opinion: "good driver," "defense: 4 out of 5." Objective data is more reliable because two scouts watching the same robot get the same answer. Subjective data is still useful for things numbers miss, but it changes with who's scouting and how tired they are. Chief Delphi veterans advise: mostly objective, a few metrics you really care about, and short written notes for the rest.

**Analogy:** "It's 72°F outside" vs. "It's nice out." One is a measurement; the other depends on who you ask.

**Why it matters on the field:** The drive team needs to trust the numbers. A notes field like "gets pushed around easily" is helpful, but "driver skill: 3/5" from different scouts can't be compared fairly.

**Watch out for:** Treating a 1–5 rating like a measurement. A "4" from one scout isn't the same as a "4" from another.

**Check yourself:** Is "drives fast" objective or subjective? How could you turn it into something more objective?

---

## Phase 1 · Collecting good data

### C5 · Kinds of scouting
**Phase:** 1 · **Needs:** C4

**The idea:** There are three common kinds. **Match scouting:** one scout watches one robot for a whole match and records what it does. Six scouts cover all six robots. **Pit scouting:** visiting teams in their pit to ask about their robot (drivetrain, what it can do, where it likes to start). **Super scouting / qualitative scouting:** an experienced scout watches a whole alliance and writes notes on things like defense, driving, and how robots work together. We also have **outside data** from The Blue Alliance and Statbotics (Phase 4).

**Analogy:** Match scouting is the stat sheet, pit scouting is the player interview, and super scouting is the coach's notes.

**Why it matters on the field:** Each kind fills gaps in the others. Pit scouting says "we can climb," and match scouting tells you whether they *actually* do.

**Watch out for:** Believing pit claims without checking match data. Teams are honest, but robots are hopeful.

**Check yourself:** A team tells you in the pits they can score 20 fuel per match. How would you check that?

### C6 · A good scouting form
**Phase:** 1 · **Needs:** C5

**The idea:** A scouting form (paper or app) should be quick to fill out while watching a fast match. Good forms: count things with tap buttons, use yes/no checks, keep the number of fields small, follow the order of the match (auto → teleop → endgame), and leave one short notes box. Every field should help answer a strategy or pick-list question. Look at what our 2026 form collected (the columns in `data-2026/`) and judge it.

**Analogy:** A good checkout screen at a store: few buttons, in the order you need them, nothing extra.

**Why it matters on the field:** A form that's too long gets filled in wrong, and wrong data leads to wrong plans.

**Watch out for:** Adding a field "just in case." Every field costs scout attention.

**Check yourself:** Pick one field from our 2026 data. What question does it help answer? If none, should it stay on the form?

### C7 · Where data goes wrong
**Phase:** 1 · **Needs:** C6

**The idea:** Scouts are humans, so data has mistakes. Common ones: wrong team number, wrong match number, losing count during a busy moment, watching the wrong robot, and getting tired by the afternoon. There's also **bias**: scouts may rate a friendly team or a flashy robot higher. Ways to fight it: short scouting shifts, clear training, robot bumper numbers checked before each match, and sometimes having two scouts watch the same robot to compare.

**Analogy:** Playing telephone. Each person passing the message adds a little error, and you need ways to catch it.

**Why it matters on the field:** One wrong team number can put a great match on a weak robot's record, or the other way around.

**Watch out for:** Blaming scouts. Errors are normal. The goal is a system that catches them.

**Check yourself:** Name two mistakes a tired scout might make, and one way the team could catch each one.

---

## Phase 2 · Meet our data

### C8 · Tidy data: one row, one robot, one match
**Phase:** 2 · **Needs:** C7

**The idea:** Our scouting data is a big table. The cleanest shape is: **each row is one robot in one match**, and **each column is one thing we measured** (team, match number, fuel scored in auto, climbed, and so on). This shape is called "tidy." It makes questions like "what's team 1234's typical score?" easy, because you just grab that team's rows.

**Analogy:** A gradebook where each row is one student's one test. You can find any student's tests, or every student's test #3, without rearranging anything.

**Why it matters on the field:** Every analysis in this tutorial starts from this table. If the shape is wrong, everything after it is harder.

**Watch out for:** Mixing in rows that aren't "one robot, one match" (like a pit scouting row, or a whole-alliance total).

**Check yourself:** Look at the first row of our data. In your own words, what does that row describe?

### C9 · The data dictionary
**Phase:** 2 · **Needs:** C8

**The idea:** A data dictionary is a short document that says what every column means: its name, what it measures, its units or allowed values, and any gotchas ("`climb` is blank if the scout forgot, not if they didn't climb"). We'll write ours in `DATA_DICTIONARY.md`. Writing it forces us to actually understand the data before analyzing it.

**Analogy:** The legend on a map. Without it, you don't know if a blue line is a river or a road.

**Why it matters on the field:** If two people think a column means different things, their numbers won't match, and the drive team gets mixed messages.

**Watch out for:** Guessing what a column means. If you're not sure, ask a coach or the person who designed the form.

**Check yourself:** Pick one column. Explain what it means and one way it could be misread.

### C10 · Notebooks and DataFrames
**Phase:** 2 · **Needs:** C8

**The idea:** We'll use **Python** in **Jupyter notebooks**. A notebook is a page with "cells" of code you run one at a time, and the result shows right under the cell. We'll use **pandas**, a Python library for tables. In pandas, a table is called a **DataFrame**. You can load a file into one, look at the first few rows (`.head()`), count rows (`len()`), and pick columns (`df["team"]`).

**Analogy:** A notebook is like a calculator that remembers every step and shows its work. A DataFrame is a spreadsheet you control with code instead of clicks.

**Why it matters on the field:** Code can redo the whole analysis in seconds when new matches come in. A hand-edited spreadsheet can't.

**Watch out for:** Running cells out of order. If something looks weird, "Restart and run all" is a good first fix.

**Check yourself:** What's the difference between a cell's code and its output? Why does running cells out of order cause problems?

### C11 · Cleaning data
**Phase:** 2 · **Needs:** C9, C10

**The idea:** Before analyzing, we fix problems in the data: misspelled or mistyped team numbers, duplicate rows (two scouts submitted the same robot and match), missing matches, and impossible values (like −3 fuel). We **never edit the raw files**. Instead, cleaning code reads the raw data and produces a clean version. Every fix is written down in code, so anyone can see what changed.

**Analogy:** Washing vegetables before cooking. You don't throw out the grocery receipt; you just clean what goes into the pot.

**Why it matters on the field:** A typo that turns team 8048 into 8084 hides one of our matches and invents a fake team.

**Watch out for:** Silently deleting rows. Always count how many rows you dropped and why.

**Check yourself:** Why do we fix data with code instead of editing the raw file by hand?

### C12 · Checking our data against official scores
**Phase:** 2 · **Needs:** C11

**The idea:** The official match results (from The Blue Alliance) tell us each alliance's real total score and some breakdowns. If we add up our three scouts' numbers for an alliance, we should get close to the official number. If we're way off, something went wrong: a scout lost count, scouted the wrong robot, or the form is missing a way to score. This is called **validation**. Chief Delphi teams in 2026 have used this to check their fuel counts.

**Analogy:** Checking your receipt against your bank statement. If they don't match, something's wrong, even if you don't know what yet.

**Why it matters on the field:** It tells us how much to trust our numbers, and which matches or scouts need a second look.

**Watch out for:** Expecting a perfect match. Penalties and things scouts can't see make small gaps normal. Big gaps are the ones to investigate.

**Check yourself:** Our scouts add up to 40 points for red alliance, but the official score breakdown says 65. Name two things that could explain the gap.

---

## Phase 3 · Describing one robot

### C13 · Grouping by team
**Phase:** 3 · **Needs:** C10

**The idea:** To learn about one robot, we gather all of its rows and summarize them. In pandas, `df.groupby("team")` does this for every team at once: it sorts the rows into piles (one pile per team), and then we compute something for each pile, like the average fuel scored.

**Analogy:** Sorting a bag of mixed candy into piles by color, then counting each pile.

**Why it matters on the field:** "Team X scores about 15 fuel per match" is the kind of sentence the drive team needs. Grouping is how we get it.

**Watch out for:** Grouping before cleaning. Duplicates and typos end up in the wrong piles.

**Check yourself:** In plain words, what does `df.groupby("team")["fuel"].mean()` give you?

### C14 · Average vs. median
**Phase:** 3 · **Needs:** C13

**The idea:** The **average (mean)** adds everything and divides by how many there are. The **median** lines the numbers up from smallest to largest and takes the middle one. One very weird match (a breakdown that scored 0, or one lucky 40) pulls the average a lot but barely moves the median. So the median often describes a robot's "normal" match better.

**Analogy:** Five friends' allowances are $10, $10, $12, $15, and $500. The average is over $100, which describes nobody. The median is $12, which is pretty typical.

**Why it matters on the field:** If a strong robot broke down once, its average makes it look weaker than it usually is. The drive team should plan for the robot that usually shows up.

**Watch out for:** Thinking the median is always better. When we predict an alliance's *total* score, averages add up nicely (C27). Use both and know why.

**Check yourself:** A robot scored 0, 18, 20, 21, 22 fuel. Without a calculator, which is higher, the mean or the median? Which better describes what they'll probably do next match?

### C15 · Floor and ceiling (percentiles)
**Phase:** 3 · **Needs:** C14

**The idea:** A **percentile** tells you where a number falls in a lineup. The 25th percentile is a robot's "bad day" (only a quarter of its matches were worse). The 75th percentile is a "good day." We call these the **floor** and **ceiling**. Our team's old tool used the 75th percentile to show what robots can do when things go well.

**Analogy:** Your test scores: your 25th percentile is what you get on a rough day, and your 75th is what you get when you studied.

**Why it matters on the field:** In a must-win match, you might want a partner with a high floor (reliable). In a bonus-RP chase, you might need a high ceiling.

**Watch out for:** Percentiles from only 3 or 4 matches are shaky (C17).

**Check yourself:** Robot A: floor 10, ceiling 14. Robot B: floor 2, ceiling 25. Which would you want if we just need a safe win? Which if we need a huge score?

### C16 · Consistency (spread)
**Phase:** 3 · **Needs:** C15

**The idea:** **Spread** is how much a robot's results jump around. A small spread means it does about the same thing every match. A big spread means it's unpredictable. A simple measure is the gap between ceiling and floor. Another is **standard deviation**: roughly, "how far from its average is a typical match."

**Analogy:** Two pitchers both average 85 mph. One always throws 84–86. The other throws anywhere from 70 to 100. You know what you're getting with the first one.

**Why it matters on the field:** A plan built on an unpredictable partner needs a backup plan.

**Watch out for:** Treating high spread as "bad." It might mean the robot is improving fast (C20).

**Check yourself:** Two robots both have a median of 15. How could you tell which one is more reliable?

### C17 · Sample size
**Phase:** 3 · **Needs:** C14

**The idea:** **Sample size** is how many matches we've seen. With few matches, one lucky or unlucky match changes everything. At a typical event, each team plays about 10–12 quals, which is not a lot. Early in the event, with only 2–3 matches per team, our numbers are rough guesses.

**Analogy:** Judging a restaurant from one meal vs. from ten. One bad night could just be bad luck.

**Why it matters on the field:** Early briefs should say "based on 2 matches," so the drive team knows how much to trust them. Outside data (Phase 4) helps fill in early.

**Watch out for:** Ranking teams with 3 matches against teams with 10 as if the numbers mean the same thing.

**Check yourself:** It's match 8 of quals. Team X has played 1 match and scored a ton. How confident should we be that they're the best scorer at the event?

### C18 · Outliers and context
**Phase:** 3 · **Needs:** C16

**The idea:** An **outlier** is a match that's way off from the rest. Before ignoring or keeping it, find out *why*. Did the robot break down or lose communication? Was it heavily defended? Did it play defense on purpose? Did the scout make a mistake? Notes and match video help. Some outliers should be kept (a robot that breaks down often is unreliable), and some should be explained (they played defense that match, so scoring 0 isn't a weakness).

**Analogy:** A student who's usually an A student gets a D on one test. Were they sick that day, or did they not understand the topic? The answer changes what you do next.

**Why it matters on the field:** "Scored 0" means very different things for the drive team if the cause was "disabled" vs. "played defense."

**Watch out for:** Deleting outliers just because they're inconvenient.

**Check yourself:** A robot scored 0 fuel in one match. Name three possible reasons, and say which ones you'd want to keep in the data.

### C19 · Rates: how often, not just how many
**Phase:** 3 · **Needs:** C13

**The idea:** Some things are yes/no each match, like "climbed" or "left the starting zone in auto." For these, we count **how often** it happens: climbed in 6 of 8 matches = 75%. Always show the counts with the percentage, because "100%" from 1 match is very different from "100%" from 10.

**Analogy:** A basketball player's free-throw percentage. Making 1 of 1 is 100%, but you'd trust 90 of 100 more.

**Why it matters on the field:** Endgame and RP plans depend on yes/no tasks. "They climb 9 out of 10 times" lets the drive team count on it.

**Watch out for:** Treating a blank (scout forgot) as a "no."

**Check yourself:** Why should the brief say "6/8" instead of just "75%"?

### C20 · Trends: recent form
**Phase:** 3 · **Needs:** C17

**The idea:** Robots change during an event. Teams fix bugs, tune autos, or break something. Looking at results **in match order** shows whether a robot is getting better or worse. Sometimes the last 3–4 matches tell you more than the whole event average.

**Analogy:** A student whose grades went C, C, B, A, A. Their average is a B, but you'd bet on an A next time.

**Why it matters on the field:** A partner who fixed their climber yesterday can probably climb today, even if their overall rate is low. And a pick-list decision on day 2 should care about who a robot is *now*.

**Watch out for:** Reading a trend into 2 or 3 noisy matches (C17).

**Check yourself:** A robot's fuel by match: 5, 6, 4, 15, 17, 16. What happened, and what would you put in the brief?

---

## Phase 4 · Outside data

### C21 · The Blue Alliance and Statbotics
**Phase:** 4 · **Needs:** C12

**The idea:** **The Blue Alliance (TBA)** is a website with official results for every FRC match: schedules, scores, and score breakdowns. **Statbotics** uses those results to estimate how good each team is. Both have an **API**, a way for our code to ask for data directly. TBA requires an **API key**, a password-like code. Keys are secret: they go in a `.env` file that git ignores, never in a notebook.

**Analogy:** An API is a restaurant's takeout window: you order in a specific way and get back exactly what you asked for. The key is your membership card.

**Why it matters on the field:** TBA gives us the match schedule (who's with us and against us) and official scores to check our scouting against. Statbotics gives us a head start before we've scouted anything.

**Watch out for:** Committing an API key. If it happens, tell a coach so the key can be replaced.

**Check yourself:** Why don't we paste the API key directly into the notebook?

### C22 · OPR: guessing each robot's share
**Phase:** 4 · **Needs:** C21

**The idea:** Official results only give **alliance** scores, not each robot's share. **OPR (Offensive Power Rating)** estimates each robot's share by solving a big puzzle: across all matches, what per-robot numbers best explain every alliance score? If team A's alliances always score high no matter who their partners are, A's OPR is high. "Component OPR" does the same thing for one part of the score (like auto or endgame).

**Analogy:** You know the total bill for many group dinners, and who was at each one, but not who ordered what. After enough dinners, you can figure out who usually orders the steak.

**Why it matters on the field:** OPR doesn't need any scouts, so it's a great check on our data and a backup when we have gaps. Chief Delphi guides say: if you have to go in blind, use OPR.

**Watch out for:** OPR is noisy with few matches, doesn't see defense, and can't separate two robots that are always on the same alliance. It also gives credit for points that came from fouls.

**Check yourself:** Explain OPR to a friend who's never heard of it, using the dinner bill idea or your own example.

### C23 · EPA (Statbotics)
**Phase:** 4 · **Needs:** C22

**The idea:** **EPA (Expected Points Added)** from Statbotics is like OPR's smarter cousin. It updates after every match, a bit like how a chess rating goes up when you win, and it carries over a team's results from earlier events. That means it's useful even before a team plays its first match at this event.

**Analogy:** A player's rating in an online game. It's a good guess at how strong they are before you play them, and it keeps updating.

**Why it matters on the field:** Early in an event, when we have few scouted matches (C17), EPA is our best guess. Later, our scouting should know more.

**Watch out for:** Carried-over EPA can be outdated if a team rebuilt their robot between events.

**Check yourself:** Early on day 1, why might EPA be more useful than our own scouting? When would our scouting be better?

### C24 · When scouting and outside data disagree
**Phase:** 4 · **Needs:** C20, C23

**The idea:** Sometimes our scouting says a robot is great, and OPR or EPA says it's average, or the other way around. That's not a problem; it's a clue. Possible reasons: our scouts miscounted, the robot plays defense (which OPR can't see), the robot changed recently, or its partners carried it. Comparing the two sources and investigating big differences is how we catch mistakes and find hidden gems.

**Analogy:** Two witnesses describe a car differently. You don't pick one at random; you ask what each one could see.

**Why it matters on the field:** Hidden gems are robots that are better than their rank or OPR suggests. These make great second picks.

**Watch out for:** Always trusting the source you like better.

**Check yourself:** Our scouting says team X averages 2 fuel per match, but their OPR is high. Give two possible reasons.

---

## Phase 5 · Showing it clearly

### C25 · Choosing the right chart
**Phase:** 5 · **Needs:** C16

**The idea:** Match the chart to the question. **Bar chart:** compare one number across teams ("median fuel by team"). **Box plot or dot plot:** show each team's floor, ceiling, and outliers at once. **Scatter plot:** compare two things to find specialists ("auto points vs. endgame points"). **Line chart:** show change over matches (trends). A table is fine when people need exact numbers.

**Analogy:** Choosing the right tool from a toolbox. A hammer is great, but not for screws.

**Why it matters on the field:** The right chart lets the drive coach see the answer in two seconds.

**Watch out for:** Pie charts and 3D charts. They look cool but are hard to read.

**Check yourself:** You want to show which robots are great at auto but weak at endgame. Which chart would you use, and why?

### C26 · Designing for a busy reader
**Phase:** 5 · **Needs:** C25

**The idea:** The drive team reads our work in a noisy queue line, with a couple of minutes to spare. So: put the most important thing first, use big clear numbers, cut anything that doesn't change a decision, label units, and say how many matches a number is based on. Then test it: show it to a drive team member and watch what confuses them.

**Analogy:** A road sign. Drivers have seconds to read it, so it says one thing in big letters.

**Why it matters on the field:** A perfect analysis that no one reads in time doesn't help.

**Watch out for:** Showing every stat "because we have it."

**Check yourself:** Look at a draft summary. What's one thing you could remove, and how do you know nobody will miss it?

---

## Phase 6 · Pre-match briefs (our main goal)

### C27 · Predicting an alliance's score
**Phase:** 6 · **Needs:** C14, C22

**The idea:** A simple way to predict a match: add up each robot's expected contribution for each alliance. Use our scouting (averages add up nicely) and back it up with EPA or OPR when our data is thin. Compare red vs. blue. 2026's top strategy teams (like 1678 on Chief Delphi) found that simple predicted-score methods work well enough, so we don't need anything fancy.

**Analogy:** Guessing the final score of a relay race by adding up each runner's usual lap time.

**Why it matters on the field:** It tells the drive team if we're the favorite or the underdog, which changes the plan: favorites play it safe, underdogs take risks.

**Watch out for:** Double-counting. If two robots both rely on the same scoring spot or game pieces, they can't both hit their usual numbers.

**Check yourself:** Our alliance's predicted score is 90 and theirs is 110. What does that suggest our strategy should be?

### C28 · Uncertainty: how sure are we?
**Phase:** 6 · **Needs:** C16, C27

**The idea:** A prediction is a guess, not a promise. If robots are inconsistent (big spread) or we have few matches (small sample size), the real score could be very different. A rough way to show this: predict a "bad day" total (using floors) and a "good day" total (using ceilings). If the ranges overlap a lot, the match is a toss-up.

**Analogy:** A weather forecast: "70% chance of rain" is more honest than "it will rain."

**Why it matters on the field:** "We're favored, but it's close" leads to a different plan than "we should win easily."

**Watch out for:** Sounding more confident than the data allows.

**Check yourself:** Red's predicted range is 80–120, and Blue's is 95–105. Who's favored? How confident are you?

### C29 · Roles on our alliance
**Phase:** 6 · **Needs:** C27

**The idea:** The best plan gives each of our 3 robots a **role** that fits what it's good at: main scorer, support scorer, defender, endgame/RP specialist, or "feeder" (moving game pieces to a better scorer). Also check **where** robots like to work, so they don't get in each other's way. Use our data and pit notes to suggest roles, then let the drive teams talk it through.

**Analogy:** A soccer team doesn't have 11 strikers. Each position covers something.

**Why it matters on the field:** Three robots fighting over the same game pieces score less than three robots with clear jobs.

**Watch out for:** Assigning roles our partners haven't agreed to. The brief makes *suggestions*; the drive teams decide together.

**Check yourself:** Our partners are a great scorer and a robot that rarely scores but drives well. What roles would you suggest for all three of us?

### C30 · Reading the opponents
**Phase:** 6 · **Needs:** C27

**The idea:** For each opponent, find their **biggest threat** (what they do that wins matches) and **weak spots** (what they struggle with: slow cycles, missing endgame, getting pushed around, frequent breakdowns). Also check how they usually play: where they score, whether they play defense, and their auto routine.

**Analogy:** A tennis player looking at an opponent's stats and seeing they have a weak backhand.

**Why it matters on the field:** It tells us whom to defend, what to protect against, and where we can gain points.

**Watch out for:** Judging a robot by one match that didn't go well (C17, C18).

**Check yourself:** Opponent A scores the most, but only from one spot. Opponent B scores less but from anywhere. Which is easier to slow down, and how?

### C31 · Defense
**Phase:** 6 · **Needs:** C29, C30

**The idea:** **Defense** means using a robot to slow down an opponent's scoring instead of scoring yourself. It's worth it when the points we take away from them are more than the points our robot would have scored. Good defense targets the opponent's best scorer and follows the game rules (there are limits on pushing, pinning, and protected zones; check the manual).

**Analogy:** In basketball, guarding the other team's best shooter can be worth more than taking your own shots.

**Why it matters on the field:** Defense can win "underdog" matches. Our data can estimate whether it's worth it.

**Watch out for:** Fouls. Defense that draws penalties gives points to the other side.

**Check yourself:** Our weakest scorer averages 5 points. Their best scorer averages 30 and slows down a lot when defended. Should our weak scorer play defense? Why?

### C32 · Playing for ranking points
**Phase:** 6 · **Needs:** C27

**The idea:** In quals, the goal isn't just to win; it's to earn **ranking points (RP)**. Besides winning, there are bonus RPs for reaching certain goals (check the 2026 manual for the exact ones). Sometimes the best plan is to go for a bonus RP even if it means a slightly lower score. If we're very likely to win, chasing bonus RPs matters more. If we're likely to lose, a bonus RP can still help our ranking.

**Analogy:** In a video game, sometimes you replay a level not just to beat it, but to collect all the bonus stars.

**Why it matters on the field:** Rankings decide who becomes an alliance captain.

**Watch out for:** Chasing a bonus RP so hard that we lose a winnable match.

**Check yourself:** We're heavy favorites in our next match. How would that change the plan compared to a close match?

### C33 · The brief: format and delivery
**Phase:** 6 · **Needs:** C26, C28, C29, C30, C31, C32

**The idea:** The **pre-match brief** puts it all together on one screen: predicted scores and how sure we are, our partners' strengths and suggested roles, opponents' threats and weak spots, an RP target, and a few short notes. It should be ready before our team goes to the queue (check the schedule for timing). When the drive team meets partners, the brief helps them start the conversation; it doesn't replace it. Be respectful: our partners know their own robots best.

**Analogy:** A coach's game-day card. It has just the plays they need, not the whole playbook.

**Why it matters on the field:** This is the main thing our scouting produces. Everything in Phases 0–5 feeds into it.

**Watch out for:** Making it too long, or being rude about partners' or opponents' robots in writing.

**Check yourself:** Show a brief to a drive team member. What did they look at first? What did they skip? What would you change?

### C34 · Closing the loop: post-match review
**Phase:** 6 · **Needs:** C33

**The idea:** After a match, compare what happened to what we predicted. Was our predicted score close? Did the roles work? Did a robot surprise us? Write a quick note. Over an event, this tells us where our predictions are good and where they're off, so we can fix our methods.

**Analogy:** Checking your answers after a practice test, so you know what to study.

**Why it matters on the field:** Without checking, we'd never know if our briefs help or hurt.

**Watch out for:** Only reviewing losses. Wins can come from luck, too.

**Check yourself:** We predicted 100–80 and lost 70–95. List three questions you'd ask to figure out why.

---

## Phase 7 · Alliance selection

### C35 · How alliance selection works
**Phase:** 7 · **Needs:** C2

**The idea:** After quals, the top 8 teams are alliance captains. Captains pick in a snake draft: round 1 goes captain 1 → 8, round 2 goes 8 → 1. Captains can pick other captains (who then leave their own spot, and everyone below moves up). A team can decline an invitation, but then it can't be picked by anyone else (check this year's rules for details). Some events also have a backup robot round. So when it's our turn, many robots are already gone.

**Analogy:** Picking teams in gym class, but you pick twice, and the order flips the second time.

**Why it matters on the field:** Our pick list must be long enough that we still have good options when our turn comes, especially in round 2.

**Watch out for:** Only planning for our top 3 choices.

**Check yourself:** We're captain #6. About how many robots will be gone before our second pick?

### C36 · Needs vs. wants
**Phase:** 7 · **Needs:** C35

**The idea:** Before ranking anyone, decide what *our* alliance needs to win playoffs. **Needs** are must-haves (for example, "someone who can reliably do the endgame task" or "a strong second scorer"). **Wants** are nice extras (for example, "a strong auto"). Chief Delphi guides recommend settling this first, then ranking teams by how well they fill our needs.

**Analogy:** Packing for a trip: first you pack what you can't go without (passport, medicine), then the nice-to-haves.

**Why it matters on the field:** It stops us from picking the "best" robot on paper when it doesn't fit our plan.

**Watch out for:** Forgetting our own robot's weaknesses. The needs come from those.

**Check yourself:** List our robot's two biggest weaknesses. What need does each one create?

### C37 · Complementary robots
**Phase:** 7 · **Needs:** C29, C36

**The idea:** **Complementary** means a partner is strong where we're weak, and doesn't compete with us for the same space or game pieces. Picking a copy of our own robot usually isn't best: two robots that score from the same spot get in each other's way. Look for partners whose strengths fill our gaps and who can work in a different area or role.

**Analogy:** Puzzle pieces. Two identical pieces don't fit together; two different ones do.

**Why it matters on the field:** An alliance with a good mix of roles usually beats one with three similar robots, even if the similar robots have slightly better stats.

**Watch out for:** Picking a weak robot just because it's different. It still needs to be good at its role.

**Check yourself:** We're a strong scorer with no endgame. Robot A is a slightly better scorer than us with no endgame. Robot B scores a bit less but climbs every time. Which complements us better, and why?

### C38 · Reliability and red flags
**Phase:** 7 · **Needs:** C18, C19

**The idea:** Playoffs are about winning every match, so **reliability** matters a lot. Red flags: frequent breakdowns or lost communication, lots of fouls, tipping over, and inconsistency. Some teams keep a **do-not-pick list** for robots with serious reliability or safety issues. Reliability notes should be about the robot, written respectfully.

**Analogy:** A car that's fast but breaks down every third trip isn't the one you take on a road trip.

**Why it matters on the field:** One breakdown in a best-of-three can end our playoffs.

**Watch out for:** Holding one early breakdown against a robot that's been fixed (C20).

**Check yourself:** How would you tell the difference between a robot that "had a bad match" and one that's actually unreliable?

### C39 · Tiers, then order
**Phase:** 7 · **Needs:** C36, C37, C38

**The idea:** Ranking 40 teams one by one is slow and leads to long arguments. Instead, first sort teams into **tiers** quickly (for example, "top first-pick choices," "great second picks," "okay," "not a fit"), spending about 30 seconds per team. Then order the teams within each tier carefully. Chief Delphi guides suggest keeping the list long, roughly 23 teams at a regular event, so we never run out.

**Analogy:** Sorting laundry into piles first (whites, colors, towels), then folding each pile.

**Why it matters on the field:** It makes the pick-list meeting faster and the list more complete.

**Watch out for:** Spending all the time arguing about #1 and #2 while #15–#23 never get looked at.

**Check yourself:** Why is a long pick list important if we only pick 2 or 3 robots?

### C40 · Simulating alliances
**Phase:** 7 · **Needs:** C27, C37

**The idea:** We can use the score-prediction code from C27 to test possible alliances: "us + A + B" vs. "us + A + C." Predict how each alliance would score, and check whether the roles fit together (C29). This turns "I think A fits better" into "here's the evidence."

**Analogy:** Trying on outfits before deciding, instead of guessing from the hanger.

**Why it matters on the field:** It helps us choose between close options and explain our reasoning to the team.

**Watch out for:** Trusting the simulation over common sense. If the numbers say a weird alliance is best, check why.

**Check yourself:** The simulation says us + A + B scores 5 more points than us + A + C, but B and A both play in the same spot. What would you do?

### C41 · First pick vs. second pick
**Phase:** 7 · **Needs:** C35, C39

**The idea:** The **first pick** is usually the best available robot that fits our needs, often a strong scorer. By the **second pick**, the top robots are gone, so we look for robots that fill a specific role well: a solid defender, a reliable endgame robot, or a "hidden gem" whose scouting data is better than their rank (C24). Second-pick choices are where good scouting gives the biggest advantage.

**Analogy:** In a fantasy sports draft, everyone knows the stars. Leagues are won by smart late-round picks.

**Why it matters on the field:** Good second picks often decide close playoff matches.

**Watch out for:** Using the same ranking for both rounds. The best second pick isn't just "the next best scorer."

**Check yourself:** Why might a robot ranked 30th be a great second pick?

### C42 · The pick-list meeting
**Phase:** 7 · **Needs:** C39, C40, C41

**The idea:** The pick list is usually finished at a team meeting the night before alliance selection. Plan for it: bring the data and charts ready to go, set a time limit, and let scouts share notes on what they saw. As a sanity check, compare our list to another ranking (like EPA). If a team is 5 or more spots apart between the two, look at it again. On selection day, update the list as more matches finish, and have someone track who's already picked.

**Analogy:** A team huddle before the big game: everyone brings what they know, and you leave with one plan.

**Why it matters on the field:** A good process turns everyone's scouting into one list the captain can trust.

**Watch out for:** The loudest voice winning. Ask, "What does the data say?"

**Check yourself:** Our list has team X at #4, but EPA ranks them #15. What do you do before the meeting ends?

---

## Phase 8 · Event day

### C43 · Event-day data pipeline
**Phase:** 8 · **Needs:** C11, C33

**The idea:** At an event, data flows: scouts collect → data gets combined → cleaning and analysis run → briefs come out. Internet at events is often bad, so the pipeline should work offline (cache TBA data early; the team's old tool did this). Make backups regularly. Know the match schedule so each brief is ready before our robot goes to the queue. Practice the whole flow before the event, not during it.

**Analogy:** A restaurant kitchen during dinner rush: orders come in, each station does its part, and food goes out on time. They practice before opening night.

**Why it matters on the field:** The best brief is useless if it's 10 minutes late.

**Watch out for:** Relying on Wi-Fi, or having only one person who knows how to run the code.

**Check yourself:** The internet goes down at lunch on day 2. What still works in our pipeline, and what doesn't?
