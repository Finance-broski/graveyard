# RETRACTIONS

Five entries in this ledger are not kills. They are places where the test itself was wrong,
I had already published or acted on the result, and the record had to be corrected in public.
They get their own file because they are the credibility core of everything else here: a
ledger that only ever says "the market said no" is easy. This file is the expensive part.

A retraction here means: the claim was published or relied upon, the flaw was in my test
rather than in the market, and the correction names the mechanism. Each of these also has
its row in [LEDGER.md](LEDGER.md); this file is the fuller writeup.

---

## R1. The dump-day short (G-052)

**The claim.** An intraday short on dump-day names printing **+50bps/day at t=5.1**. It
survived a first audit. Downstream work was built on it the same week: pro-forma
projections and sizing plans, none of which survived it.

**The bug.** The signal used **full-day volume inside a 09:45 entry**. The volume was caused
by the outcome it predicted: the dump IS the volume. At 09:45 the signal knew the size of a
day that had not happened yet.

**The correction.** Rebuilt point-in-time, the strategy **loses ~15bps/day**. Not weaker.
Inverted.

**The impact.** Everything downstream was retracted the same day the bug was found. The
error had propagated through **four working sessions** of research before being caught,
which is the honest speed of this class of mistake. A first audit had already passed it. The full mechanics are in
[autopsies/G-052.md](autopsies/G-052.md).

## R2. The pump-long twin (G-053)

**The claim.** The mirror-image long: **+64bps/day at t=7.4**.

**The bug.** The same full-day-volume look-ahead, opposite sign.

**The correction.** Point-in-time: **-48bps/day at t=-11.9**. The pair is a matched
demonstration that one plumbing bug can manufacture two "independent" strategies with
five-plus-sigma t-stats in opposite directions.

**The impact.** Retracted alongside R1. The pair now serves as the ledger's standing example
of why a big t-stat is not evidence when the field itself is leaky.

## R3. The Kelly-Jiang mechanism claim (G-014)

**The claim.** A published explanation for why a paper's result fails to replicate in India:
circuit-band censoring of the return distribution.

**The bug.** The explanation was wrong. Measured properly, band censoring accounts for only
~4% of the effect; the actual driver was threshold geometry in the construction.

**The correction.** The kill verdict stands (the strategy is still dead); the *mechanism*
was retracted and replaced. Being right that something fails does not license being wrong
about why.

**The impact.** Corrected in public. The row now records both the dead strategy and the
dead explanation.

## R4. The cost-shifted t-stat (G-092)

**The claim.** A return series held as statistically significant at the scoping stage.

**The bug.** The t-test was run on a series that already had a constant cost subtracted.
Subtracting a deterministic constant shifts the mean while leaving the variance untouched,
which inflates |t| mechanically. The raw series was insignificant.

**The correction.** Standing rule, now applied ledger-wide: **significance is tested on raw
returns, profitability on net returns, and a deterministic constant is never t-tested.**

**The impact.** The row was refiled with the raw-series verdict, and the rule it minted is
applied ledger-wide.

## R5. The double-counted lever (G-103)

**The claim.** A proposed structural improvement to the book, presented with a pro-forma
uplift.

**The bug.** The "new" lever was already live in the book's canonical configuration. The
pro-forma double-counted an effect that was already in the baseline.

**The correction.** Proposal withdrawn, pro-forma retracted.

**The impact.** Minted the cheapest rule in this file: **read the live config before
proposing structure.** The most embarrassing entry here, and the fastest to fix.

---

If you have never retracted anything, you have not looked hard enough at your own work.
