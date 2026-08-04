# RUN YOUR OWN GRAVEYARD

The method costs nothing and needs no tooling beyond a text file and a git repo. It changes
what your research process knows about itself.

## 1. Write the bar before the test

Before running anything, write one line: the hypothesis, and the preregistered bar that
would count as success. Numbers, not vibes: "net return positive with t >= 2 after measured
costs, in-sample AND out-of-sample" is a bar. "See if it works" is not. If you cannot write
the bar, you are not ready to run the test, because any result can be argued into a win
after the fact.

Commit the preregistration before the result exists. The git timestamp is your clock, and
it is the only part of this that cannot be faked later.

## 2. Count everything you run

The single most corrosive habit in retail quant work is running twenty variants and
remembering one. Every configuration you run goes in the count, including the ones you
eyeballed and deleted. The count is the denominator that makes your survivor meaningful.
A Sharpe 2 found among 5 preregistered configs and a Sharpe 2 found among 500 casual ones
are different objects: with enough draws, selection alone manufactures whatever statistic
you are screening for.

## 3. Kill with numbers, classify the death

A kill row states what actually happened, with the numbers: the t-stat that was not there,
the cost that ate the edge, the era where the sign flipped. Then classify the death (the
taxonomy in this repo's README is yours to steal). The classes matter because they teach
different lessons: no-signal teaches humility, cost-wall teaches venue realism, regime
teaches that most "laws" are portraits, infra-invalid teaches that your own test is a
suspect in every result.

## 4. Park, do not delete

Some kills are conditional: real but too small for your capital, real but walled by a
borrow constraint, real in a regime that may return. Park those with a NAMED re-open
condition ("comes back if X, checked on date Y"). This removes the fear of premature
shelving, because the door is not welded shut, and it stops zombie strategies wandering
back in just because time passed and you missed them.

## 5. Retract in public

Sooner or later a test you already announced will turn out to be broken: a look-ahead, a
stale mark, a mechanical artifact. Retracting it in public, with the mechanism named, is
the highest-yield credibility act available to a researcher. It is also the strongest
possible internal incentive to audit before you announce.

## 6. The ledger format

One markdown table, one row per hypothesis:

| id | killed | hypothesis (one line) | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|

The receipt column points at your own evidence (the script, the ledger entry, the commit).
You will be surprised how often you consult your own graveyard, and how often it stops you
from re-running a funeral you already paid for.

## 7. Why bother

Because the graveyard is the most informative dataset you own. It encodes your venue's cost
frontier, your market's regime map, and your own most repeated errors. And if you publish
it, it does one more thing: it makes your survivors believable, because the reader can
finally see the denominator.
