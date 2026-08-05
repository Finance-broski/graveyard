# THE GRAVEYARD

[![DOI](https://zenodo.org/badge/1322596014.svg)](https://doi.org/10.5281/zenodo.21803488)

*"The graveyard is the most informative dataset I own, and almost nobody keeps one."*

This is a public, forward-running ledger of my dead trading research. Every hypothesis I
kill gets a row: what I believed, what would have counted as success, what the data said,
and how many configurations died finding out.

**155 distinct strategies tested, across 112 ledger entries, over 2,123
configurations. 12 survived. Five public retractions. Provenance graded honestly, row by row.**

There are more strategies than entries because fourteen entries are families: one row can
hold eleven separate ideas. This ledger said 112 until those bundles were expanded by hand,
which meant an artifact about publishing your denominator was under-reporting its own by a
third. And 2,123 is still a floor, because before this ledger existed the discarded variants
were never counted at all. Both corrections are the thesis applied to itself.

## Why publish failures

Everyone publishes their wins. Nobody publishes their denominator. That asymmetry is
survivorship bias applied to research itself, and it is the reason most published backtests
cannot be trusted: you are looking at the best row of a table you were never shown.

This repo is the table.

I run a systematic book on Indian markets and a research process that kills most of what it
touches. The kills are not the waste product of that process. They are most of what the
process knows. A strategy that survived 155 funerals means something different from a
strategy that survived none.

## How to read it

[LEDGER.md](LEDGER.md) holds the rows, grouped by cause of death:

| cause of death | class | meaning |
|---|---|---|
| Nothing there | `no-signal` | nothing there once artifacts and controls were applied |
| Broken test | `infra-invalid` | the test itself was broken; refiled honestly, some became retractions |
| Costs ate it | `cost-wall` | real gross, dead net of honest Indian costs |
| One era only | `regime` | worked in one era, died outside it; a portrait, not a law |
| Edge given back | `handed-back` | the edge is real and the mechanism hands it back |
| Market said no | `structural-wall` | unshortable, illegal, or capacity-walled; the market says no |

Business and go-to-market kills are recorded in the internal master but are not shown here.
This ledger is about dead trading strategies, and "the GST-reconciliation wedge had a dozen
incumbents" is not something a reader of this can use.

A set of rows is withheld pending leak review (they sit too close to the live book). They
are counted, never hidden: the ledger states exactly how many rows you are not seeing.
Withheld rows publish in redacted form as review completes, and several already have.

## The retractions

The credibility core of this ledger is not the kills. It is the five times the test itself
was wrong and I said so in public:

1. **The dump-day short (G-052).** A +50bps/day intraday short printed t=5.1 and survived a
   first audit. It used full-day volume in a 09:45 entry signal: the volume was caused by
   the outcome it predicted. The point-in-time version loses 15bps/day. Retracted with its
   entire downstream: pro-forma Sharpes, a 25.5% CAGR three-way book, and a leverage plan,
   all invalid. It propagated four working sessions before I caught it. That is the honest
   speed of these errors.
2. **The pump-long twin (G-053).** Same look-ahead, opposite sign: claimed +64bps t=7.4,
   point-in-time reality -48bps t=-11.9.
3. **The Kelly-Jiang mechanism claim (G-014).** My published explanation for why a paper
   failed to replicate in India (circuit-band censoring) was itself wrong: censoring is ~4%
   and the effect was threshold geometry. Retracted the explanation, kept the kill.
4. **The cost-shifted t-stat (G-092).** I t-tested a return series that had a constant cost
   subtracted, which inflates \|t\| mechanically. Raw t was insignificant. Standing rule
   born: significance on raw, profitability on net, never t-test a deterministic constant.
5. **The double-counted lever (G-103).** I proposed a "new" structural improvement that was
   already live in the book's canonical config, and retracted the pro-forma. Lesson: read
   the live config before proposing structure.

If you have never retracted anything, you have not looked hard enough at your own work.

## Checked against the field

Every major kill-family was cross-checked against the academic literature: 16 families,
7 confirmed by independent published work (naked option buying loses: Coval-Shumway;
vol-managed portfolios disappoint out of sample: Cederburg et al; and so on), 5 scoped as
dead-at-my-venue but alive elsewhere, 4 flagged for bounded re-trials where the literature
uses a different construction, and zero cases of the literature contradicting a component
that survived. The kill-machine replicates the field. Details in the ledger rows.

## What survived

Twelve hypotheses, out of everything above, are alive in some form: deployed, paper-gated, or
parked as candidates. Their construction does not publish from this repo. The ledger is
about the dead; the survivors are the book.

## What the ledger says about research

Read as a distribution rather than a list, the causes of death are themselves the finding.

**60% died as no-signal.** 51 of 85 published hypotheses produced nothing once
artifacts and controls were applied. That is the base rate this work runs at, worth stating plainly
because most published research implies the opposite ratio.

**13% died because my own test was broken.** 11 rows are infra-invalid: look-ahead in the
plumbing, stale marks, a statistic computed on a cost-shifted series, a calendar artifact.
Roughly one investigation in eight failed because of me rather than because of the market. That
is the number I did not expect when I started counting, and it is the strongest argument for
keeping the ledger at all, because an error rate you cannot see is one you cannot reduce.

**13% were real and unharvestable.** 11 rows are cost-wall: genuine gross edge, dead net of
honest costs. The most expensive kind of dead end, because they pass every statistical check and
fail only where money changes hands.

The rest divide into premium the mechanism hands back (6), era-dependence (5), and one structural wall where the market simply says no.

Recurring failure modes, in the order they have cost me most: a field only knowable after the
decision timestamp; a universe screened today and run backwards; costs assumed rather than
measured; a statistic computed on a series that was already smoothed; and a result found by
search but reported as though it were found by hypothesis.

## Exploratory and confirmatory are not the same evidence

Of the 85 published rows, 29 carry a stated numeric bar that was fixed before
the test ran. Those are confirmatory: the result either cleared a threshold set in advance or it
did not. The other 56 were exploratory, run to see what was there, with the verdict recorded afterwards.

Exploratory work is legitimate and necessary, and it is how you learn which questions are worth
asking. It is not evidence at the same strength, and treating it as though it were is precisely
the error this ledger exists to document. The preregistered bar column is the marker: where it
holds a number, the test was confirmatory. Everything appended to [FORWARD.md](FORWARD.md) from
launch onward is confirmatory by construction, because the bar is committed before the result
exists.

## Known limitations

**Rows record what was tested and how it died, not why I believed it would work.** The rationale
is the most useful field for someone learning to do this, and it is the one the backlog lacks.
Autopsies carry it and are being added over time.

**The published set is not the complete set.** Rows sitting too close to live book construction
are withheld, counted and stated. More importantly, configurations discarded before this ledger
existed were never recorded at all, so the true denominator is higher than the number shown and
is not recoverable.

**Configuration counts are deliberately conservative.** The census takes the first number in each
row's configs field, which undercounts compound entries. The recorded total is a floor rather
than an estimate.

## Timestamps, stated precisely

"Preregistered before results" is only as good as its clock, so here is what the clock shows and
where it stops short.

Every preregistration file in the research repo was committed as its own commit, before any result
was appended to it. There is no case where a bar and its verdict landed together. The gaps,
though, are minutes to hours rather than days, for the plain reason that most of these tests take
minutes to run: the median is twelve minutes between the bar going in and the file next being
touched. Anyone treating a twelve-minute gap as strong evidence of good faith should not, and I
would rather state that than have it discovered.

What those short follow-up commits contain carries more weight than the gap. They are protocol
amendments that declare their own position relative to the output, in the file, at the time. One
reads *"declared after Phase-1 output, before any rescoring."* Another opens with *"epistemic
status declared before results: this is a same-data follow-up on a result already seen, so
directional confirmation here is not independent evidence."* Writing down in advance that your own
next test will not count as independent evidence is a harder discipline than preregistration, and
it is the one worth pointing at.

The limitation is real. That repository is private, because the same files contain live book
construction, so none of the above is directly checkable by you. What exists externally are
anchors for the flagship rows: an SSRN working paper, dated public posts, and a retraction trail
published the same day the errors were found.

From launch onward the situation inverts. New preregistrations append to [FORWARD.md](FORWARD.md)
before their results exist, and that git history is a clock anyone can audit without taking my
word for anything.

## Run your own

The method is free and does not need my tooling: [METHOD.md](METHOD.md). The short version:
write the bar before you run the test, count everything you run, publish the funerals, park
with re-open conditions instead of deleting, and retract in public when the test itself was
wrong.

## Citing this

If you cite a row, a class, or the census, cite the ledger:

> Jain, A. (2026). *The Graveyard: a public ledger of killed trading-research hypotheses*
> (version 1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.21803488

The DOI above always resolves to the latest version; each release also carries its own
version DOI (v1.0 is 10.5281/zenodo.21803489), so a citation can pin the exact state it
read. Every release is archived independently of GitHub.

`CITATION.cff` is in the repo, so GitHub's "Cite this repository" button produces BibTeX and APA
directly. Rows are versioned: the git history preserves every prior state, so a citation to a row
is a citation to a specific version of it.

## Corrections

Measured disagreements are the good kind. If you believe a row is wrong, open an issue with
your own numbers and method. Rows change when the evidence does, and the git history keeps
every prior version.

---

*Ayan Jain. I publish measured backtest biases at [The Bias Ledger](https://financebroski.substack.com)
and build [backtest-bias](https://github.com/Finance-broski/backtest-bias)
(`pip install backtest-bias`). If you want this class of scrutiny on your own backtest:
[Bias Check](https://forms.gle/sAvosfHnitCBm9FD7), fixed fee, written verdict.*
