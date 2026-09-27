# English examples (synthetic material)

The setting, design and every number below are invented. They illustrate judgment and selection and come from no paper or market data. Do not carry the objects, numbers or conclusions into a user's text. Each example gives the material, the judgments made before writing, and the delivered text. In real use only the text and any necessary notes are delivered; the judgments are not shown.

## Material

The research question has two parts. Did a reduction in the minimum tick size lower trading costs for the affected stocks, and did liquidity supply at the best quotes change?

An exchange reduced the minimum tick from 1 cent to 0.5 cent for a pilot group of 120 mid-cap stocks on one announced date. The exchange chose the pilot stocks; assignment was not randomized. Each pilot stock is matched to one control on pre-period market capitalization, price level and average quoted spread. The main sample covers six months before and six months after the change at the stock-day level. The specification is a difference-in-differences regression with stock and day fixed effects and standard errors clustered by stock. The event study uses month −1 as the reference and bins months beyond ±4 into end-point indicators. The placebo test uses an extended pre-period of twelve months and a pseudo change date six months before the actual one. Tick-constrained stocks are those whose pre-period quoted spread averaged at most 1.5 ticks (54 of the 120 pilot stocks).

Table 1. Difference-in-differences estimates

| Outcome | Pre-period mean (pilot) | Estimate | SE |
|---|---|---|---|
| Quoted spread (bps) | 14.2 | −3.1 | 0.6 |
| Effective spread (bps) | 9.8 | −1.2 | 0.5 |
| Log depth at best quotes | — | −0.48 | 0.07 |
| Log cumulative depth within 10 bps of midquote | — | −0.05 | 0.06 |
| Log daily share volume | — | 0.03 | 0.04 |

Table 2. Event-study coefficients, quoted spread (bps)

| Month | −4 | −3 | −2 | −1 | +1 | +2 | +3 | +4 |
|---|---|---|---|---|---|---|---|---|
| Estimate | 0.2 | −0.3 | −0.9 | ref. | −2.6 | −3.0 | −3.3 | −3.2 |
| SE | 0.6 | 0.6 | 0.5 | — | 0.6 | 0.6 | 0.7 | 0.7 |

Table 3. Additional estimates, quoted spread (bps)

| Specification | Estimate | SE |
|---|---|---|
| Placebo change date | −0.4 | 0.7 |
| Tick-constrained pilot stocks and their matches | −5.6 | 0.9 |
| Unconstrained pilot stocks and their matches | −0.7 | 0.7 |
| Two-way clustering by stock and day | −3.1 | 0.8 |
| Excluding the 10 trading days around the change | −3.2 | 0.6 |

Other facts. No other exchange rule change took effect in the sample window. Two pilot stocks were added to a major index in month +2; their announcement dates are not supplied. No analysis has been run on order flow migrating between pilot and control stocks, and trade sizes were not analysed. The submitted abstract states that "the tick size reduction improved liquidity: quoted spreads fell by 22% and effective spreads by 12%." The depth results appear in a table and are described only as a change in the composition of liquidity supply. The quoted-spread estimates by tick constraint appear in an appendix. The authors hold the underlying data and code, but have not run further analyses.

## Example 1. From result tables to a Results section

The request is a Results section of about 450 words.

### Judgments before writing

The question names two outcomes, trading costs and liquidity supply at the best quotes, so both lead. Spreads fell and best-quote depth fell. The abstract's "improved liquidity" covers only the first. The text follows the estimates and the mismatch is flagged in a note.

Order of material. The cost estimates with their base values; depth and what it leaves open; subgroup estimates; the evidence on identification. The subgroup result moves ahead of the robustness checks because it shows where the quoted-spread point estimates differ. The month −2 coefficient is 1.8 standard errors from zero and about 30% of the main estimate, so it is reported with its consequence for magnitudes. The event study, placebo and split cover quoted spreads only, which limits what can be said about the other outcomes; that goes in the text.

The constrained and unconstrained point estimates differ by 4.9 bps, but the uncertainty of that difference is not given. A pooled interaction would test it. The text reports the two estimates without claiming a statistically established difference.

### Delivered text

Following the tick size reduction, quoted spreads of pilot stocks fell by an estimated 3.1 bps relative to matched controls (SE 0.6), about 22% of the pilot pre-period mean of 14.2 bps (Table 1). Effective spreads fell by 1.2 bps (SE 0.5), about 12% of their pre-period mean of 9.8 bps. The effective-spread decline is smaller in both absolute and proportional terms. It is also less precisely estimated relative to its magnitude, with a 95% interval of roughly −2.2 to −0.2 bps.

Liquidity supply at the best quotes declined. Depth at the best quotes fell by 0.48 log points (SE 0.07), about 38%. Cumulative depth within 10 bps of the midquote shows no detectable change (−0.05, SE 0.06), with an interval running from a decline of about 15% to an increase of about 7%, and volume did not change detectably (0.03, SE 0.04). The estimates show narrower spreads together with thinner best quotes. They do not show whether costs fell for orders larger than the depth displayed at the best quotes, because trade sizes were not analysed.

The quoted-spread point estimate is larger for stocks classified as tick-constrained. For the 54 constrained pilot stocks and their matches it is −5.6 bps (SE 0.9). For the remaining 66 pilot stocks and their matches it is −0.7 bps (SE 0.7), which is not distinguishable from zero and still admits a reduction of about 2 bps (Table 3). No test of the between-group difference is supplied; this split was not reported for effective spreads or depth.

Event-study coefficients for months −4 and −3 are 0.2 and −0.3 bps. The month −2 coefficient is −0.9 bps (SE 0.5), about 1.8 standard errors from zero. Month −1 is normalized to zero, so its displayed value does not establish a reversal of a pre-trend. Rebasing the post-change contrasts to month −2 would reduce their absolute magnitudes by 0.9 bps; their uncertainty would require the coefficient covariances. The reported post-change coefficients range from −2.6 to −3.3 bps (Table 2). The placebo estimate is −0.4 bps (SE 0.7), two-way clustering raises the main standard error to 0.8, and excluding the 10 trading days around the change gives −3.2 bps (SE 0.6). These checks concern quoted spreads only and do not establish parallel trends. Effective spreads and depth have only the baseline estimates.

### Notes outside the text

The abstract states that the change "improved liquidity." Depth at the best quotes fell by about 38%, so the estimates support lower spreads and thinner best quotes, not an unqualified improvement. The abstract needs the same two-sided statement as the text.

Derived numbers. The percentages are the estimates divided by the pilot pre-period means. The 38% is 1 − exp(−0.48). Intervals are the estimate ± 1.96 SE, with log estimates converted by exp.

Effective spreads by trade size would test whether the cost reduction extends to larger executed trades. To assess orders exceeding displayed depth, trade size must also be compared with the depth available at execution; trade records alone may not recover parent-order costs. An event study for effective spreads would assess its own pre-period behavior, which the quoted-spread event study cannot establish.

## Example 2. Discussion and limitations

The request is a Discussion of about 400 words covering interpretation and limitations.

### Judgments before writing

Two interpretations need a stated evidence status. Redistribution across the finer price grid is consistent with the depth estimates and untested. The quoted-spread pattern by tick constraint is consistent with relief from a binding grid, but selection or other shocks could also differ across these groups. It is not a mechanism test for effective spreads or depth.

The relevant limitations concern non-random selection, interference between pilot and control stocks, the index additions and the absence of trade-size analysis. Each affects a different inference. Bias directions require assumptions about how the event changes the particular outcome in each group; a direction for spreads does not carry over to depth.

### Delivered text

The estimates combine narrower spreads with thinner best quotes. Quoted spreads fell by about 22% and effective spreads by about 12%, while depth at the best quotes fell by about 38%. The smaller effective-spread decline could reflect pre-existing execution inside the quotes or greater price impact when trades exceed the reduced depth. Both explanations require trade-level analysis. A trade-size gradient alone would not distinguish them, since price improvement inside the quotes could also vary with trade size.

The depth estimates are consistent with liquidity being spread over the additional price levels. Cumulative depth within 10 bps shows no detectable change, although its interval admits a decline of up to about 15%, and depth further from the midquote was not examined.

The larger quoted-spread point estimate among tick-constrained stocks is consistent with relief from a binding price grid. The subgroup difference has not been tested, and selection or other shocks correlated with the constraint could generate this pattern. Matching on pre-period levels does not establish parallel trends. The month −2 coefficient of −0.9 bps is material relative to the −3.1 bps main estimate; neither the normalized reference month nor the imprecise placebo result resolves the concern. These diagnostics do not cover effective spreads or depth.

Order-flow migration could affect the control outcomes. If withdrawal of liquidity providers widened control spreads, the estimated spread reduction would be too large in absolute value for a direct effect holding controls unaffected. Order-flow migration need not have that consequence, and depth could be biased differently. The volume interval describes the net relative change in daily volume, not the amount of trading that migrated. Index additions could also exaggerate the spread decline if they narrowed the two stocks' spreads independently of the tick change. Month +1 precedes their inclusion, but announcement or anticipation effects remain possible. Finally, the effective-spread result cannot establish costs for large trades without the size analysis.

Over the six months after the change, the full pilot sample shows estimated declines in quoted spreads, effective spreads and best-quote depth relative to controls. Only the quoted-spread estimate is reported by tick constraint.

### Notes outside the text

Re-estimating without the two index-added stocks and their matches would show how much the estimates depend on those observations. Confirming the announcement dates would clarify whether month +1 can serve as a pre-index comparison.

## Example 3. Point-by-point response to reviewer comments

The reviewer comments are synthetic and are not a record of any real review. The authors hold only the results above. No further analysis has been run. The current request produces a response draft and proposed manuscript wording; it does not edit the manuscript.

The comments are as follows. (1) Pilot stocks were not randomly assigned, so why should parallel trends be believed, and the month −2 coefficient does not look trivial. (2) The fall in depth at the best quotes suggests liquidity got worse, so the claim that the tick reduction improved liquidity is not supported. (3) If order flow migrated from control to pilot stocks, the control group is contaminated. (4) The index additions in month +2 may confound the results. (5) Results should be reported for large trades, whose effective spreads may have increased.

### Judgments before writing

| Comment | Classification | Status |
|---|---|---|
| 1 | Existing estimates inform but do not resolve the concern | Text changes proposed; analysis planned |
| 2 | Answered by existing estimates, against the original claim | Narrower wording proposed |
| 3 | Needs new analysis; bias direction depends on spillover behavior | Text changes proposed; analysis planned |
| 4 | Partly answered by the month +1 coefficient; re-estimation needed | Planned |
| 5 | Needs new analysis; the claim must be restricted meanwhile | Narrower wording proposed; analysis planned |

Pre-period behavior and possible control-group spillovers bear on the causal interpretation of the main result. Trade-size analysis determines how far the cost claim extends. The index-addition exclusion is a focused check that can proceed alongside them. A pre-trend test can reveal violations or imprecision; failure to reject does not establish parallel trends.

### Delivered response draft

Summary of changes

Proposed manuscript changes, using estimates already available. The abstract's statement that the change "improved liquidity" would be replaced by a statement of narrower spreads and thinner best quotes. The quoted-spread estimates by tick constraint would move from the appendix to the main results, and the month −2 coefficient would be discussed. These edits have not yet been applied to the manuscript.

Planned and not yet run. Effective spreads by trade size. A joint test of the pre-period coefficients and event studies for effective spreads and depth. A comparison of control stocks with mid-cap stocks outside the matched sample. Re-estimation without the two index-added stocks.

Comment 1

We agree that the month −2 coefficient is material. It is −0.9 bps (SE 0.5), 1.8 standard errors from zero and about 30% of the main estimate. The proposed text reports it and states that matching on pre-period levels does not establish parallel trends. Month −1 is normalized to zero, so it cannot supply independent evidence that a pre-trend reversed. The placebo estimate of −0.4 bps (SE 0.7) remains compatible with nontrivial pre-period changes. The quoted-spread point estimates are −5.6 bps for constrained stocks and −0.7 bps for unconstrained stocks, but their difference has not been tested and could reflect selection correlated with the constraint. We will add a joint test of the pre-period coefficients, report its precision, and estimate event studies for effective spreads, depth and the tick-constrained subsample. We will examine whether plausible departures from parallel trends could account for the estimated declines. If they could, the causal interpretation will be restricted accordingly; a nonsignificant pre-trend test alone will not resolve that concern.

Comment 2

The depth result warrants a more specific claim. Depth at the best quotes fell by 0.48 log points (SE 0.07), about 38%, and the original description understated it. Cumulative depth within 10 bps shows no detectable change (−0.05, SE 0.06), with an interval from about −15% to +7%. The abstract currently reads "the tick size reduction improved liquidity: quoted spreads fell by 22% and effective spreads by 12%." The proposed replacement is: "Following the tick reduction, pilot stocks show estimated declines relative to matched controls of 3.1 bps in quoted spreads (22% of the pre-period mean) and 1.2 bps in effective spreads (12%). The quoted-spread point estimate is larger among stocks classified as tick-constrained. Depth at the best quotes fell by about 38%, while cumulative depth within 10 bps shows no detectable change."

Comment 3

Migration has not been tested. If the pilot drew liquidity providers away from controls and thereby widened control spreads, the spread estimate would overstate the direct reduction relative to a counterfactual with unaffected controls. A shift in trade flow alone does not establish that response; the effect on depth must be assessed separately. The volume estimate (0.03, SE 0.04) has an approximate 95% interval from −5% to +11% after conversion from logs. This concerns the net relative volume change, which can combine migration with offsetting changes in other trading, and is not an upper bound on migration. We will examine control outcomes against a further group of comparable mid-cap stocks outside the matched sample, checking their pre-period behavior and possible exposure to the pilot. If that group is a credible unaffected comparison, we will report estimates using it as a sensitivity analysis. Wider control spreads alone would not establish that migration caused the difference.

Comment 4

Two of the 120 pilot stocks were added to an index in month +2. If index inclusion independently narrowed their spreads, it would make the estimated spread decline more negative. The month +1 coefficient of −2.6 bps precedes inclusion, but the announcement dates are not supplied and anticipation could affect that month. We will verify those dates and re-estimate the main comparisons without the two stocks and their matches. If the decline becomes materially smaller, we will report this dependence and narrow attribution of the full-sample decline. Stable estimates would address dependence on these observations without resolving other selection concerns.

Comment 5

Trade sizes have not been analysed, and thinner best quotes make the concern plausible without establishing that large-trade costs rose. The proposed text restricts the effective-spread finding to the reported full-sample estimate and leaves effects by size open. We will estimate effective spreads by trade-size category, with cutoffs fixed using each stock's pre-period distribution, and report changes in trade composition and the weighting used. A claim about trades exceeding available depth will also require comparing their sizes with contemporaneous depth. If the largest category shows a reliable cost increase, that result will enter the abstract alongside the overall decline; smaller-trade benefits will be stated only if their own estimates support them. These trade-level results would not establish costs for parent orders split across executions.

### Notes outside the letter

The draft distinguishes proposed edits from analyses still to be run. Update these statuses and add manuscript locations after the edits and analyses are actually completed.

The letter describes the exchange's choice of pilot stocks only as non-random. If the exchange published its selection criteria, state them in the response to Comment 1, since they decide which selection stories are plausible.
