# THE LEDGER

One row per dead hypothesis. Grouped by how it died. Every row states what would have
counted as success (the preregistered bar, where the batch recorded one), what actually
happened with numbers, and how many configurations were run. Rows marked withheld are
counted here and will publish in redacted form after leak review; nothing is silently
missing.

Reading note: configs counts preregistered cells actually run. The true denominator is
higher and, before this ledger existed, uncountable. That admission is the artifact's own
thesis applied to itself.


## Nothing there (52)
*`no-signal` — the hypothesis produced nothing once artifacts and controls were applied*

| id | killed | hypothesis | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|
| G-001 | 2026-07-30 | Option-seller "adjustments" (roll untested in) improve VRP shape | no-signal | beat static on mean AND p5, net | mean 10.3 to 0.8 pts/wk, tail WORSE (-481 vs -428) | 2 runs x 256 cycles | HUNT_LEDGER K4 |
| G-003 | 2026-07-30 | Convert-to-fly on breach | no-signal | same | worst week of program (-680 vs -428 static) | 256 | K4 |
| G-004 | 2026-07-30 | Stop-at-2x-credit on weekly strangle | no-signal | same | tail identical to static, mean -1.8; stops fire post-extraction | 256 | K4 |
| G-005 | 2026-07-30 | Zero-hero: expiry-day ATM straddle, tiered exits (8x/5x/4x) | no-signal | mean net > 0, t≥2 | all 6 exitxentry cells negative; tiers hit 3-9% of expiries | 6 x ~256 | K5 |
| G-006 | 2026-07-30 | ATM CE/PE parity gate improves expiry-day entries | no-signal | gated beats ungated | gate deletes 84% of days, adds nothing (subsample noise) | 2 | K5 audit |
| G-007 | 2026-07-30 | Zero-hero OTM ladder (ATM+1/+2/+4, distance + premium-targeted) | no-signal | any cell mean>0 t≥2 | 18+6 cells all negative, t to -10.7; monotone worse further OTM | 24 | K6 |
| G-008 | 2026-07-30 | "Buy cheap gamma" conditioning on expiry afternoons | no-signal | cheap quintile ≥ 0 | INVERTED: cheapest quintile worst (-131 to -160% of outlay) | 20 | K6b |
| G-011 | 2026-07-29 | Week-1 expiry long strangles (far-week premium cheap) | no-signal | k1-2 ratio ≠ theoretical | ratio 0.6746 vs 0.6745 median-\|z\| - priced to 4 decimals | 4 | K2 |
| G-012 | 2026-07-29 | F&O-inclusion repricing (+10%/60d, shortability story) | no-signal | survive momentum-matched control | t=6.51 raw to control -0.5; 219 events = 39 waves; momentum in costume | 6 | K3 + fo_inclusion_test |
| G-015 | 2026-07-31 | 200-EMA touch = support (the folklore) | no-signal | touch beats near-miss control t≥2 | touch +0.23% vs control +0.39% fwd10, t -2.5; hold rate 36.7% | 5 | ema200_test |
| G-016 | 2026-07-31 | The 200 specifically is special vs unwatched lengths | no-signal | 200 beats placebo family beyond their spread | 150/175/225/250 hold 36.3/36.4/36.3/35.9 vs 36.7 - inside noise | 5 | ema200_test |
| G-017 | 2026-07-31 | Confirmation pairing rescues EMA touches (RSI/volume) | no-signal | any pairing beats plain control | all pairings ≤ +0.50 vs control +0.59 (PIT-500 harmonized: vol combo -0.01) | 8 | ema200_paired + harmonized |
| G-018 | 2026-07-30 | Retail TA battery long entries (RSI<30, MACD cross, BB touch, golden cross, 55d, vol-chase) | no-signal | any \|t\|≥3 positive | nothing positive clears; significant cells all NEGATIVE (BB -0.70%/21d t-5.1) | 14 | ta_battery |
| G-019 | 2026-07-30 | Indicator confluence (3-4 agreeing = high-probability setup) | no-signal | monotone improvement in k, top cell t≥2.3 | V-shaped: k=2 worst cell of program (-0.60%/21d t-5.2); k=3-4 positive but ~once/stock/decade, thin after costs | 16 | ta_confluence |
| G-021 | 2026-06-20 | Directional time-of-day edge on NIFTY | no-signal | P(close>open \| window) ≠ .5 | P = .508; nothing tradable | ~10 | pattern scan |
| G-026 | 2026-07-02 | Options-sentiment cross-sectional contrarian L/S | no-signal | survive senior-audit noise bar | Sh +0.59 gross, cut as noise at audit (corr-to-mom +0.10) | ~8 | options_sentiment memory |
| G-027 | 2026-07-0x | Participant-wise options positioning signal | no-signal | survive audit | initial WIN, cut as noise at senior audit | ~6 | in_hand_signal memory |
| G-028 | 2026-07-0x | Rollover % as signal | no-signal | IC t≥2 | killed | ~4 | in_hand memory |
| G-029 | 2026-07-0x | Promoter-stake change (SHP) as signal | no-signal | IC t≥2 | killed at F&O-shortable universe (t 1.22) | ~6 | in_hand memory |
| G-032 | 2026-07-26 | Delivery-conviction short signal | no-signal | survive on BORROWABLE universe (SLB re-open TESTED) | paper t3.75 to borrowable non-F&O short-excess +0.1%/yr t0.0 hit48. The t lived in the untradeable illiquid tail | ~10 | KILL_AUDIT prize test |
| G-034 | 2026-07-26 | Promoter-selling short cluster | no-signal | same | borrowable universe short-excess +0.1%/yr t0.0 - same illiquid-tail evaporation. Generalization: SLB unlocks EVENTS, never continuous cross-sectional selection | ~10 | same |
| G-040 | 2026-07-0x | Multi-asset CTA sleeve | no-signal | adds to frontier | killed (thin, redundant) | ~8 | diversifier notes |
| G-042 | 2026-07-0x | Book-level vol targeting | no-signal | improves after diversification | redundant once diversified; killed | ~4 | diversifier notes |
| G-044 | 2026-07-18 | FX F3/F4/F5 (breadth campaign) | no-signal | prereg bars | all three killed at preregistered bars; two adjacent candidates frozen or parked, identities withheld | ~15 | fx_prop memory |
| G-049 | 2026-07-25 | I1 intraday cross-sectional reversion (fade morning move into close) | no-signal | net ≥ +12bps, t≥3 gross | corr(morning,afternoon) +0.002; net -27bps/d | ~8 | INTRADAY_HUNT B1 |
| G-051 | 2026-07-25 | I3 opening-range breakout/reversion | no-signal | same bars | corr +0.008; dead | ~6 | same |
| G-054 | 2026-07-26 | PIT trailing-volume rescue of continuation/reversion | no-signal | PIT filters revive edge | continuation WORSE with every filter; reversion-long = IS+/OOS- falling-knife lottery (median -63bps, win 38-44%) | ~12 | rescue attempt |
| G-055 | 2026-07-26 | OFS-day intraday short (scheduled forced-flow) | no-signal | net > 0 tradeable | stock RISES on OFS day intraday (short -65bps t-3.1); anticipated flow is priced at the open | ~6 | final kills |
| G-056 | 2026-07-26 | F&O ban-list entry short | no-signal | tradeable 09:45 entry | -6bps t-0.7 (drift spent by 09:45, open artifact); stop HURTS | ~6 | same |
| G-062 | 2026-07-26 | Option scalping - BUYING ATM intraday (mom/rev/burst, 0DTE+weekly) | no-signal | any cell positive | every cell negative (t -3.6 to -9.5, win 35-42%); bigger burst = worse (buying tops of mean-reverting moves); theta + double-spread + reversion all against buyer | ~24 | scalp mine |
| G-063 | 2026-07-26 | Cross-sectional options-positioning micro panel (OI/PCR/IV/skew/buildup) | no-signal | OOS-replicate | NONE replicate (signs flip train/test) | ~27 | micro mine |
| G-064 | 2026-07-26 | Directional macro cues (SP500/VIX overnight to NIFTY intraday) | no-signal | PIT tradeable direction | predicts the GAP only (+53% t22 = priced at open, untradeable); open-to-close is noise. 3rd look-ahead caught pre-claim | ~10 | macro mine |
| G-066 | 2026-07-26 | Bulk-deal net-flow signal | no-signal | orthogonal to owned factors | decade-STABLE IC -4.62 t-5.7 (both halves!) BUT net-of-reversal t-0.7 = reversal in disguise. Decade-stable and still redundant | ~8 | bulk mine |
| G-068 | 2026-07-26 | Sell calls on insider-flagged "won't rise" names | no-signal | insider adds to call-selling EV | INVERTED: the insider signal adds ~0 to call-selling EV; the edge that exists is tail-shape, not direction | ~18 | sell_calls_insider |
| G-072 | ≤2026-07-26 | Wrong-signed factor family: quality, accel, lowvol-as-RETURN, breakouts, buy-the-middle, India-continuation-not-reversion | no-signal | - | each carried the OPPOSITE sign OOS or in controls | ~6 | KILL_AUDIT B1 |
| G-073 | ≤2026-07-26 | OOS-collapse family: Follow-FII, Follow-Pro, resmom, most C-series, value_ey | no-signal | - | positive IS, dead OOS - the classic | ~8 | B1 + prereg batches |
| G-082 | 2026-07-26 | "Refine the graveyard" itself (the meta-hypothesis) | no-signal | - | refinement rescued NOTHING; every fixable-how was already refined to its next wall at kill time. The audit (re-classify by death reason) found the one dividend, refinement found zero | n/a | KILL_AUDIT bottom line |
| G-084 | 2026-07-02 | H2: expiry-day pin drift via futures | no-signal | hit ≥55%, monotone in GEX | non-monotone noise, hit 48% | 5 | h2_pin |
| G-085 | 2026-07-02 | H3: VRP roll-timing upgrade | no-signal | ≥0.1%/cycle improvement | <=5bps/cycle, under the bar | 10 | h3_rolltime |
| G-086 | 2026-07-02 | H4: conditional overnight-gap continuation (gap x GEX) | no-signal | conditioning separates | negative everywhere that matters; gaps fade | 6 | h2_pin_h4_gap |
| G-087 | 2026-07-02 | H5: open-auction IV-overshoot fade | no-signal | net Sharpe ≥1.5 | "overshoot" is information, not dislocation: hit 33%, Sharpe -2.5 WRONG WAY | 4 | h3_h5 |
| G-093 | 2026-07-23 | Circuit-lock continuation long (E16) | no-signal | - | KILL with sign REVERSED: next-open buying loses, t_raw ≈ -16 (reversal real, the opposite trade is cost-walled) | ~6 | E16 |
| G-094 | 2026-07-23 | IPO lock-in expiry supply dip (E8) | no-signal | - | 1,189 proxy events: no dip at proxy precision | ~4 | E8 |
| G-097 | 2026-07-24 | Seasonal tilt inside live composite (C1-v2) | no-signal | - | fails inside the composite; C1 family closes fully | ~5 | C1-v2 |
| G-098 | 2026-07-24 | MCX EOD momentum TS+XS (C6) | no-signal | - | TS +0.3%/yr t0.08, XS -1.0% t-0.36; consistent with 6-name breadth floor | ~4 | C6 |
| G-101 | 2026-07-24 | Crash tail-typing flags (options/basis/compression) | no-signal | - | ALL THREE fail as flags; "far from flag-grade" | ~9 | tail-typing |
| G-104 | 2026-07-20 | Correlation-regime reversion + index lead-lag + flow persistence | no-signal | - | clean DOWN moves do NOT revert (sign wrong, era-flips -1.03/+0.43/+0.59); lead-lag killed; flow-persistence dead | ~15 | PREREG_CORR_REGIME |
| G-105 | 2026-07-20 | Long-only reversal suite (T1-T4) + "buy the middle" | no-signal | - | ALL FOUR killed, the sign is the finding (India continues, doesn't revert); buy-the-middle killed BY THE VOLATILITY CONTROL (was lowvol in costume) | ~12 | PREREG_LONGONLY |
| G-106 | 2026-07-22 | Stream batch 1: GILT-as-UST-substitute, vol term-structure/skew signals, OR15 debit verticals | no-signal | - | GILT kill (crisis-shape fails +0.48 down vs +0.76 up; hostile audit found daily-corr inflated by smoothing - kill stands); term/skew nothing at 0.8t; OR15 debit = strongest kill of the night | ~12 | PREREG_STREAM 1 + audit |
| G-110 | 2026-07-1x | Participant-positioning follows (FII/Pro/Client index futures) | no-signal | - | Follow-FII the textbook trap: IS +1.35 to OOS -0.15; Pro OOS -0.9 to -1.4; the one IS+OOS survivor (fade retail) later cut as noise at senior audit | ~15 | POSITIONING_HUNT |
| G-112 | 2026-05-xx | Early forex H-series (H-EVENT-01-DRIFT, H-HTF-LTF-01 + siblings on the forex M1/M15 DB) | no-signal/infra | - | pre-swing-ledger era: the 4h drift survivor DIED after the -3h timezone-bug fix; the HTF-LTF v1 kill no longer holds as originally stated (data was mis-timestamped both ways). Era's honest lesson: half the "findings" were the clock. Receipts = memory-era notes + retained backup tables; provenance thinner than later rows, marked as such | ~15 | forex_ohlcv memory notes |
| G-115 | 2026-08-28 | The pair screener's acceptance rule ranks the year ahead | no-signal | accepted pairs beat correlation-matched rejected ones out of sample | +5.5 points a year with acceptance taken from the stored run, which knows the future; -2.1 (+/-1.3) once acceptance is recomputed inside each test year, so nothing could know. The difference was hindsight. Accepted pairs do not beat correlation-matched rejected controls and no sortable column ranks the year ahead. Published on the product's own front page and in its launch post rather than buried | 2 | pairdesk self-test |

## Broken test (12)
*`infra-invalid` — the test itself was broken (look-ahead, stale marks, artifacts); refiled honestly, and several became public retractions*

| id | killed | hypothesis | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|
| G-009 | 2026-07-30 | Limit-fill generosity rescues zero-hero | infra-invalid to no-signal | any fill model positive | close-fill vs limit-fill BRACKET reality; all cells negative both | 16 | K6b |
| G-014 | 2026-07-28 | KJ failure via circuit-band censoring (my own mechanism claim) | infra-invalid | censored-Pareto moves the measure | RETRACTED publicly: censoring ~4% pooled, threshold geometry artifact | 8 | kj_audit2-4 |
| G-031 | 2026-06-xx | Balance-sheet leverage factor on free PIT window | infra-invalid | pre-2023 PIT exists | FY2023 XBRL cliff: free PIT B/S pre-2023 nonexistent to crash-trap factor | ~4 | balance_sheet_cliff |
| G-050 | 2026-07-25 | I2 overnight-gap fade intraday | infra-invalid | tradeable after 09:29 | +30bps t12.5 raw to lives ENTIRELY open to 09:29 (untradeable); 09:29 entry -11.5bps. Open-window artifact | ~6 | same |
| G-052 | 2026-07-26 | **Dump-day intraday short (the retraction)** - vol≥3x + drop to short 09:45 | infra-invalid | PIT-clean at entry | "+50bps/day t=5.1 confirmed" survived a first audit, then the hostility pass: the signal used FULL-DAY volume, unknowable at 09:45 and caused by the outcome it predicts. Point-in-time version loses 15bps/day (t=-3.0). RETRACTED with its entire downstream, all invalid; propagated 4 sessions before caught | ~30 | dump_* scripts; propagated 4 turns before caught |
| G-053 | 2026-07-26 | Pump-long intraday (symmetric) | infra-invalid | PIT | claimed +64bps t7.4 to PIT -48bps t-11.9 | ~8 | same audit |
| G-075 | ≤2026-07-26 | Micro-artifact family: phantom-open E4 fills, cost-shifted-t E2, settle-vs-LTP ITM marks | infra-invalid | - | test-construction artifacts caught by entry/mark decomposition | ~5 | B1 |
| G-089 | 2026-07-0x | Residual momentum (our construction) | infra-invalid | OOS survives | killed; literature (Blitz-Huij-Martens) robust with a DIFFERENT recipe to bounded re-trial filed | ~6 | GRAVEYARD_LIBRARY D1 |
| G-092 | 2026-07-24 | F&O ban-list entry/exit drift (E2) | infra-invalid | - | **RETRACTED**: scoping bar t-tested a COST-SHIFTED series (constant charge inflates \|t\| mechanically); raw t -1.5/-1.7 = ns. Spawned the standing rule: significance on RAW, profitability on NET, never t-test a deterministic constant | ~8 | BATCH5 E2 correction |
| G-096 | 2026-07-23 | Gold-ETF stale-NAV arbitrage (E4) | infra-invalid | - | killed AS artifact - the "dislocation" was the stale print itself | ~4 | E4 |
| G-100 | 2026-07-24 | SIP-window calendar effect | infra-invalid | - | t=2.93 was ENTIRELY overlapping sessions 1-3 of month (pooling artifact) | ~4 | batch5 |
| G-113 | 2026-08-11 | The book's kill switch is armed whenever GEX is low, as wired | infra-invalid | the arming leg fires on the intended fraction of days | GEX grows with open interest, so ranking today against the raw 2011-2026 history made `gex_low` true on 5.2% of days in 2024+ against 51.4% era-neutral (pr252). The switch was arming on the 200dMA leg alone: blind to a crash from the top. Found in my own live wiring, not in a backtest. Fix specified the same night (compare against a trailing 252 sessions instead of the full history) and deliberately queued behind the gate verdict; verified still unapplied in book_run.py on 2026-08-31, so the leg remains dead while this row publishes | 2 | SEAMS_AUDIT 2026-08-11, arm_recheck.py |

## Costs ate it (11)
*`cost-wall` — the edge is real gross and dead net of honest Indian costs*

| id | killed | hypothesis | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|
| G-010 | 2026-07-29 | Peer's MCX intraday trend+reversion (orthogonal overlay) | cost-wall | net > 0 after measured costs | orthogonality real (-0.46) but 2bp gross vs 8bp cost; -59%/yr | ~12 | K1 |
| G-022 | 2026-06-03 | Fixed-param ORB (opening range breakout) India | cost-wall | net positive any config | all configs net-negative (infra validated, both look-ahead gates PASS) | ~24 | quant.intraday |
| G-024 | 2026-06-02 | VRP harvest futures-hedged | cost-wall | net after STT > 0 | futures STT eats the edge entirely | 4 | VRP_FINDINGS |
| G-036 | 2026-07-2x | Insider-trades signal | cost-wall | Sharpe after costs ≥ book bar | t7.7 IC to Sharpe 0.31 tradable-universe | ~6 | KILL_AUDIT |
| G-037 | 2026-07-2x | Reversal composite | cost-wall | net > 0 | t13 gross, dead on measured costs | ~10 | KILL_AUDIT |
| G-057 | 2026-07-26 | Intraday pairs (minute z-reversion, HDFCBANK/ICICI etc.) | cost-wall | net > 0 | gross +77-162%/decade real; 0.3bps/trip edge vs 40bps cost = ~-1000%/yr of cost drag on traded notional (the bankroll dies in ~5 weeks). Two orders of magnitude under | ~8 | final kills |
| G-058 | 2026-07-26 | Systematic intraday reversal composite (15-feature PIT mine) | cost-wall | net > 0 at any real venue | IC OOS +4.83% t13 GENUINELY REAL; net -62(mid)/-15(large)/-4bps(top-cap optimistic). Market efficient exactly to the cost frontier | ~40 | systematic mine |
| G-059 | 2026-07-26 | Any sub-daily horizon harvest (5m to close full sweep) | cost-wall | net > 0 any horizon | nothing clears at sub-10-day holds; what does clear lives at horizons the book already trades, so the sweep bought redundancy, not alpha | ~60 | horizon sweep, subdaily_fwd |
| G-076 | ≤2026-07-26 | Cost-walled residue: ADR-gap, reversal_5, seasonal-mom (79% turnover), illiquid-tail P2 (dies @100bps), covered-call, long-vol/gamma (theta), OR15 debit verticals | cost-wall | - | real gross, dead at honest round-trips | ~10 | B2 |
| G-090 | 2026-07-0x | Short-term reversal 2-4wk | cost-wall | net > 0 | killed; literature's surviving version is DAILY residual (liquidity provision) - likely still cost-dead here | ~6 | GL D4 |
| G-109 | 2026-07-20 | PEAD/SUE illiquid-tail long | cost-wall | - | REPRODUCED-NOT-TRADEABLE: monotone, t=11.65, survives every confound (half is bid-ask bounce, residual real) - and dies on the cost realistic for that liquidity bucket | ~10 | PREREG_PEAD |

## One era only (5)
*`regime` — worked in one era, sign flips or dies outside it; an era portrait, not a law*

| id | killed | hypothesis | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|
| G-013 | 2026-07-28 | Kelly-Jiang tail-risk state transfers to India | regime | paper's autocorr/vol-corr replicate | autocorr ~0 vs 0.9, COVID not top-tail, null all horizons; power verified 0.85 to 0.78 | ~20 | kj_* 4-audit chain |
| G-030 | 2026-07-0x | Promoter-pledge as crisis signal | regime | fires in crisis windows | pledge data 2021+ crisis-blind; can't validate where it matters | ~4 | balance_sheet memory |
| G-074 | ≤2026-07-26 | Regime-mirage family: vol-term-structure timer, crash-cue-atlas cells, BAB-highvol | regime | - | looked like signals, were era-portraits | ~10 | B1 + PREREG_CRASH_CUE |
| G-095 | 2026-07-23 | Index-rebalance add/delete flow (B5-1) | regime | - | every cell FLIPS SIGN by era; post-2021 arbed away | ~6 | B5-1 + FORCED_FLOW |
| G-107 | 2026-07-21 | Crash-cue atlas (macro cues predict crashes) + regime-weighted overlay | regime | - | prediction fails on clean methodology (reactive, not predictive); overlay tilt FAILS vs incumbent; halves disagree | ~20 | PREREG_CRASH_CUE |

## Edge given back (7)
*`handed-back` — the premium or edge is real and the mechanism hands it back (direction risk, crash correlation, theta)*

| id | killed | hypothesis | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|
| G-002 | 2026-07-30 | Roll-tested-out adjustment as risk tool | handed-back | p5 +25% w/ mean cost ≤10% | tail -95 vs -203 but mean -32%; 2x costs to negative | 256 cycles | K4 |
| G-020 | 2026-06-20 | Buyable window for naked long ATM weeklies (intraday) | handed-back | any entryxhold cell positive IS&OOS | all 78 straddle cells negative; momentum 0 cells positive | 78 | nifty_pattern_scan |
| G-023 | 2026-06-02 | VRP harvest naked short strangle | handed-back | direction survivable | premium real (+1.59 vol pts t=4.75) but direction kills unhedged | 6 | VRP_FINDINGS |
| G-061 | 2026-07-26 | NIFTY weekly/0DTE short straddle (incl intraday sell 09:45 to 15:15) | handed-back | net > 0 or a timer rescues | breakeven t1.2 win60% worst -2.1%; best conditioner t1.8 fails 6-way multiple testing. VRP fully priced net of cost at ATM | ~20 | weekly options mine |
| G-069 | 2026-07-26 | Single-stock OTM wing-selling as standalone sleeve | handed-back | survives a real crash | calm alpha REAL both sides (puts +8.2, calls +5.8%/yr, beta 0.13-0.19), then the COVID test: -24% notional in ONE month (-96% on margin) wipes ~3yr; predicted-by-strike-math -25%, hit -24.0. Spreads eat the edge; crash-correlated with the rest of the book, so it fails the diversification bar; in-book it was Sharpe-neutral with a worse tail | ~64 | grid + cov_crash_test + stop tests + combined_book_puts |
| G-077 | ≤2026-07-26 | Premium-handed-back family: iron-condor (proven 4 ways), ratio spreads, calendarized-VRP, tail-hedge-via-carry, index-hedge variants | handed-back | - | defined-risk hands the edge back; crash-correlated | ~15 | B5 |
| G-114 | 2026-08-11 | A per-side 3x settle stop on the VRP sleeve improves the BOOK | handed-back | beat the book A/B on CAGR without worsening drawdown percentiles | Standalone it works, and plateau-stably (k 2.5-4.0): sleeve geo 21.9 to 25.9%, worst-8 -48.8 to -27.7%, Sharpe 0.79 to 1.03. At book level REJECTED: +0.7pp CAGR but DD percentiles worsen (-10/-14/-16 to -12/-17/-20 at L1.15) and the solver strips L* 1.35 to 1.20. The stop insures a solo-cell risk the book already diversifies away, then pays the premium in the joint chop-crash cell (Covid -1.5 to -8.9%). Kept as a drawer item for standalone or high-weight VRP worlds | ~5 | SEAMS_AUDIT 2026-08-11, honest_update A/B |

## Market said no (1)
*`structural-wall` — unshortable, illegal, lot-size or capacity walls; the market says no*

| id | killed | hypothesis | class | preregistered bar | verdict, with numbers | configs | receipt |
|---|---|---|---|---|---|---|---|
| G-038 | 2026-07-02 | USDINR carry/trend sleeve (retail) | structural-wall | legally tradable | RBI: retail USDINR non-hedging ILLEGAL; offshore-only | ~6 | pareto memory |

---
*88 rows published in full or redacted form; 24 rows withheld pending leak review (counted, never hidden); 3 business and go-to-market kills counted but not shown, because this ledger is about dead trading strategies; 115 total. Maintained by hand against the source audits named in each row's receipt.*
