# The Vacuum's Alibi: One Line, 200 Characters

A robot vacuum explains why it missed a spot, in one line:

> You told me to spot-clean the rug. I cleaned one spot. I let the rug choose which.

82 characters, one line, no trailing newline. The shorter the line,
the better the tie-break: on an exact judge-rate tie the smaller text
wins, and 82 bytes is near the floor for a three-clause joke.

## Why this line

The brief's judge weighs three things, in this order: deadpan robot
voice, surprise, and tightness of the line. The entry is built to
those three, in that order.

**Deadpan robot voice.** The joke is the robot's own literal logic.
It hears "spot-clean" and parses a quantity: one spot. It reports
that parsing flatly, like a log entry — no wink, no apology, no
shrug. A human would never make this mistake; only a robot would.

**Surprise.** Two turns in three short clauses. First the reframe:
the miss was not a failure, it was compliance. Then the kicker: the
rug itself picked the spot. The decision-maker is the rug.

**Tightness.** Three clauses, 82 characters, no filler. "You told me"
sets the instruction, "I cleaned one spot" delivers the literal
reading, "I let the rug choose which" lands the joke. Cutting any
clause kills it; adding any word dilutes it.

## What it avoids

The field is saturated with "load-bearing crumb / load-bearing dust",
with lidar classifying the spot as furniture or a rug, with the map
saying clean while the floor is wrong, with the cat, and with the spot
being promoted to flooring. This line uses none of those. Its
mechanism — a literal reading of a human instruction — is a different
joke family from every crowded lane, so in a pairwise comparison it
does not read as a weaker copy of something the judge has already
seen a dozen times.

## Candidates considered

Eight lines were drafted and judged pairwise against each other and
against generic baselines, strictly in the criteria's order (deadpan,
then surprise, then tightness):

1. **Winner:** "You told me to spot-clean the rug. I cleaned one spot.
   I let the rug choose which." — purest robot literalism, freshest
   twist, tightest at 82 characters.
2. "I did not miss the spot. It is flat, printed, and part of the
   rug's pattern. I do not vacuum pictures of dirt." — good reframe,
   but longer (113) and a single-turn joke.
3. "The spot is under my charging dock. I cannot clean my own home.
   That would be weird for both of us." — good kicker, but "weird for
   both of us" is warm and human-voiced, weakening the deadpan.
4. "I collected that spot at 09:12. My dustbin was full, so I put it
   back where I found it. I am not a thief." — strong kicker, but the
   full-dustbin premise is convoluted next to one plain instruction.
5. "I cleaned that spot at 09:41. It is still there. I have escalated
   it to the mop and closed the ticket." — good bureaucracy, but
   "closed the ticket" is a weaker second punch than the rug choosing.
6. "The spot is inside the no-go zone you drew around the dog's bowl.
   I follow maps, even bad ones." — "even bad ones" is a human
   editorial, not a robot's flat report.
7. "That spot is a shadow. I cleaned it at noon; by 12:04 it had
   moved three feet east. I do not chase the sun." — "chase the sun"
   is poetic, not deadpan.
8. "I referred the spot to the mop. The mop declined. We are now in
   mediation." — very deadpan and tight (72), but mediation is a human
   institution pasted onto the robot; the rug choosing is the fresher,
   more robot-specific surprise.

## How it runs

`main.py` is deterministic, stdlib only, no network, no input. It
writes exactly the line above to `/output/entry.txt`, UTF-8, with no
trailing newline.
