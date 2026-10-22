---
name: kai-research
description: Research argumentation and results analysis for quantitative finance, statistics, and machine learning. Identify the main conclusion and the relative importance of evidence from the research question, design, and result tables; organize comparisons, robustness checks, unexpected findings, and genuine limitations; address reviewer objections individually; and decide which additional analyses are worth doing. Use to write or revise results analysis, discussion and limitations, reviewer response letters, and pre-submission reviews. Use kai-writing for language editing and kaiplot for figures.
---

# kai-research · Research argumentation

## Purpose and delivery

This skill handles judgments in research argumentation: which finding answers the research question, what comes first, what to compare it with, how large and how certain the difference is, what each test rules out, how to explain unexpected results, which judgment a limitation affects, and whether an objection calls for evidence, a design explanation, further analysis, or a narrower conclusion. Use kai-writing for sentence-level expression and kaiplot for figures and tables. If neither is loaded, still avoid the first-person plural “我们” in Chinese manuscript prose, use colons sparingly in ordinary narration, and do not add formulaic openings, conclusions, or disclaimers.

Once materials are available, deliver the prose, analysis, or response letter the user requested, in the requested language. If the user specifies a length, select content to fit it; establishing priorities is how that selection is made. Do not output version numbers, scores, checklists, or internal checking procedures by default.

Divide the prose into paragraphs as the argument develops. Keep the comparison, numbers, and explanation for one finding together, and start a new paragraph when moving to another question or body of evidence. Do not give each number its own short paragraph or compress an entire results section into one paragraph. Reorganizing paragraphs must not reduce the length or depth of development the user requested.

Put the research subject, setting, and conditions into an affirmative statement of the finding, then stop at the result. If the sentence itself or preceding text already states “on the grid tested” or “during this evaluation period,” do not append endings such as “other settings remain untested” or “the result cannot be generalized to other fields.” Discuss that issue only when the current argument actually makes the relevant extrapolation or the user asks to discuss the limitation. Do not turn every supported claim into a self-negating statement.

Add notes outside the manuscript prose only in four situations: an existing user claim conflicts with the results; a missing piece of material prevents a particular judgment; the prose contains values calculated from the supplied material; or one or two additional analyses would materially change the conclusion. Include only information that changes what the user should do next, without repeating the prose, usually in no more than three or four points. If an external note identifies doubts about the material itself, do not continue using that material as evidence in the prose.

When rewriting manuscript prose, correcting a judgment does not mean placing the correction process in the manuscript. If the draft attributes a performance difference to a mechanism but the materials support only a performance comparison, write the comparison clearly. Explain outside the manuscript why the attribution was removed and what still needs checking. Do not append “these metrics alone cannot establish…” to every finding that has already been narrowed. Known design problems and contrary results that change the meaning of the main finding must still be addressed; do not hide them by moving them out of the manuscript.

Use only the research materials provided for the current task. Do not borrow research subjects or numerical values from examples or source notes into the user's prose. A test not supplied is not necessarily a test not performed, and do not claim on the user's behalf that it was performed. If a premise needed for the reasoning is absent—for example, that costs are higher during certain periods or that certain events affect spreads—state it conditionally rather than treating it as a known fact.

## Judgments before drafting

### The main conclusion

First identify the main conclusion and its direct support. An empirical conclusion refers to a specific comparison: relative to whom, on which metric, and in which sample. A model-based study refers to a proposition, proof, or numerical evidence and its conditions. The main conclusion answers the research question; it is neither the largest number in the table nor the component the author most wants to emphasize. Narrow an insufficiently supported conclusion rather than substituting a more attractive result.

If the user's title, abstract, draft, or request already contains a claim, first interpret its original subject, negations, and qualifiers, then compare it with the results. “No significant deterioration was found” does not mean “deterioration has been proved impossible”; do not strip the qualification from the former and then criticize it as overstated. Correct a wrong metric, excessive strength, excessive scope, or omitted conditions according to the evidence, and identify the original sentence and supporting evidence outside the prose. Preserve descriptions that hold.

Keep the strength of the same claim consistent across the abstract, introduction, results, and conclusion. Qualifications made in the main text must also appear in the abstract and conclusion, including parameter conditions, sample scope, and findings that hold only in some settings. Do not describe an unevaluated component as a capability of the method, or turn something called a conjecture earlier into an established finding later.

### Priorities and space

Order results by their role in supporting the main conclusion. The main results that directly answer the question come first and receive the most space, followed by evidence that makes them credible, then their scope of applicability, with extensions and supplementary analyses last. Evidence that determines whether the main conclusion is credible belongs in the main text; do not leave it only in an appendix while giving the main text to extensions. Allocate space by the weight of the evidence for the claim, not by the amount of work or the author's preference for a component. If an extension brings no improvement, give it less prominence in both the abstract and the main text.

Discuss only numbers that determine the judgment in the prose, leaving the rest in tables. Numbers quoted in the prose must agree exactly with the tables; approximations must not make the result look more favorable. Check each directional statement, such as an increase or decrease, against the tables. Every number in the abstract, introduction, and conclusion must match the main text, with its calculation and definition identifiable in the results section. Specify the metric, task, cost level or sample segment, and comparator.

### Comparisons, effect sizes, and uncertainty

Include the strongest simple approach for the task among the comparators, such as the previous value or an autoregression for a persistent series, buy-and-hold or a simple rule for a strategy, or the proposed method with its claimed key component removed. If all comparators are ablated versions of the proposed method itself, limit the conclusion to component contributions. When the magnitude is markedly greater than in comparable research, check metric definitions, information timing, and measurement conventions before explaining it. Give methods equivalent tuning budgets and information sets. Apply the same standard to the proposed method and its comparators; a deviation of the same size cannot be a defect in one and acceptable performance in the other.

When the materials provide both a version of the same model without a component and a strong external benchmark, the two comparisons answer different questions. To determine whether the component improves the original model, report the direct ablation comparison first. To establish how the improved model ranks among competing methods, use the external benchmark. Do not select only the strongest benchmark and omit the ablation that answers the research question, or report only an easily won ablation while avoiding a stronger benchmark.

Report effect sizes with their reference quantities and units. Distinguish percentage points from percentages, and express the size in terms readers can assess, such as a share of the mean or standard deviation, returns after costs, or the budget required to reach the same target. When comparing investment periods of different lengths, annualized returns may be added: calculate them separately from each strategy's portfolio value and period length, then compare them. Do not annualize the difference in cumulative returns directly. For a coefficient with a theoretical benchmark that is relevant to the claim, test its distance from that benchmark. Report gains that can be obtained by sacrificing another metric as pairs: coverage with interval length, returns with drawdown and turnover, and accuracy with cost.

Use uncertainty information to assess the reliability of differences; do not assume noise is negligible from point-estimate magnitudes alone. If standard errors, intervals, repetition counts, or tests are not supplied, describe point estimates without claiming statistical significance. If this affects the central judgment, identify the missing evidence outside the prose. With a very small sample, a difference can be translated into a number of observations. Nonsignificance does not mean no effect, nor that an effect is smaller than another. Significance in one group and nonsignificance in another do not establish a difference between them; test the difference itself.

For results selected from multiple settings, combinations, or parameters, state which data informed the selection. An optimum chosen using the test set carries selection bias; displaying the other settings does not remove it. Assess rolling training by the information available at each forecast time. Historical data already published before a forecast may be used in the next training run; it is not leakage simply because it falls within the overall backtest period. Exclude future information and the selection of a procedure after inspecting evaluation results followed by using those same results to claim out-of-sample superiority. Check generalizations such as “best throughout” or “holds universally” across all relevant segments, and specify the interval when an advantage occurs only there.

Beyond averages, examine distributions across units, groups, or time periods. An average that meets a target while individual units systematically deviate, or an improvement concentrated in a few periods, is a result that belongs in the main text.

### Robustness and heterogeneity

Tie each test to a specific concern, explaining what its design and result imply for that concern without appending “other explanations cannot yet be ruled out” to every item. Report not only whether significance remains but also how the estimate and uncertainty change. Loss of significance after a sample change may reflect a smaller effect or lower precision; judge from the estimates rather than significance stars alone. Do not combine different tests into the single statement “the conclusion is robust.” A mechanical conversion of the same value or a reparameterization that leaves the test unchanged does not count as independent evidence.

Keep attribution within the scope of the test. State conclusions according to the sample segment excluded, the outcome tested, and whether the analysis provides only counts or a return decomposition. Do not narrow a result to a particular year without support, infer sources from counts, or extend a test of one outcome to others.

Failure under favorable settings shows that even those conditions do not guarantee success. Without a monotonicity argument, it does not imply that all other conditions can only be worse. A successful correction in the same setting likewise supports a conclusion only within the tested range. Examine performance both when the method's claimed operating conditions hold and when they are violated.

Write mechanism explanations according to the actual evidence. A direct test of one link does not identify the entire mechanism. Findings consistent with a mechanism may support an explanation, but do not state that they exclude other explanations. To distinguish competing mechanisms, compare the outcomes each predicts. A two-sided test of whether an effect exists need not force a prespecified sign, but either significant sign cannot automatically support the same specific mechanism. Where possible, assess a new variable or component in a comparison that holds other arrangements constant. Improvement in an intermediate objective does not automatically improve the final outcome. Causal heterogeneity is usually grouped by pretreatment characteristics; grouping by post-treatment changes requires a separate identification explanation. Do not relabel parameter sensitivity as heterogeneity.

### Unexpected and unfavorable results

Include results that contradict expectations or prior literature, conflict across metrics, or hold only in some settings in the main text. State where they occur, their magnitude, and what they imply for the main conclusion. Indicate the evidential status of explanations. Revisit a prespecified expectation when the result has the opposite sign. Test explanations that can be examined with the available data rather than stopping at “the reason is…”.

Do not leave unfavorable findings only in tables or pass over them with “not shown” or “in most cases.” Details such as crossing a target threshold, shifting from conservative to anti-conservative behavior, or a reversal at low budgets belong in the prose if they change the reader's judgment of when the method is usable.

### Limitations

Discuss only specific limitations that change the reader's judgment, placing them near the relevant claim. Explain the affected conclusion, existing treatment, and remaining impact as needed; do not force every limitation into a four-part template or append “the existing evidence nevertheless…”. When discussing the direction of bias, state the premises. Do not invent a direction of bias for an issue that concerns only precision or applicability. Assess absolute shortcomings separately from relative advantages: a lag does not imply being slower than the benchmark, and falling short of an ideal target can still represent improvement. Preserve advantages supported by direct comparisons while explaining costs or failure cases that affect use.

Derive limitations from the study's design, data, and inferential approach rather than generic lists, and do not automatically add disclaimers. If only an excerpt is supplied, mark tests not provided as needing consultation; do not assert that the study did not perform them. When the user needs directly usable prose, write from the available results and place matters needing verification outside the manuscript. Do not insert placeholders for optional statistics. A claim that a method is “the best feasible approach under current conditions” needs specific support and cannot serve as a fixed ending.

## Responding to objections and choosing further analyses

Classify each comment before replying point by point. If existing results answer it directly, identify the evidence and add it to the manuscript only if it was omitted. Answer even when the result is unfavorable to the author, narrowing the corresponding conclusion. If the design needs explanation, provide supported reasons and relevant trade-offs. If new analysis is needed, report completed results; write unfinished work as a plan, specifying the proposed settings and how different outcomes would change the conclusion. If the evidence does not support the original claim, provide wording before and after revision. When a reviewer misreads the paper, first check the original text. Clarify ambiguous wording; for points already stated clearly, cite the location and explain the evidence. Do not assume in advance that the author is wrong or withdraw a supported conclusion merely to appear cooperative.

Make the current state clear in each response, distinguishing existing results, changes actually made to the manuscript, suggested replacement text, and planned additional analysis without imposing status labels. Do not say the manuscript has been revised when only replacement paragraphs have been drafted. Do not prewrite results for unfinished analyses; the opening summary of the response letter must also distinguish completed from planned work. Proposed manuscript text must not make stronger claims than the evidence in the response. Mark design facts absent from the materials for author verification rather than asserting them on the author's behalf.

Rank proposed analyses by three considerations: how seriously the concern threatens the main conclusion, whether plausible outcomes would change that conclusion, and cost. Recommend only a few top-ranked analyses, explaining which two explanations each can distinguish. Method names may be given, but do not write authors, publication years, volumes, or pages from memory into manuscript prose or a response letter. When a citation is needed, flag it for verification outside the prose.

If there are no reviewer comments and the user requests a pre-submission review, use the same approach to identify the most likely objections, evidence already in the manuscript that answers them, and the most useful additional evidence.

## Adjusting to the study type

Different study types rely on different evidence for credibility and are prone to different overclaims. The table is a starting point, not a template that must be filled. Handle mixed types in order of importance. See the study-types reference below for details.

| Type | The main conclusion usually concerns | Credibility mainly comes from | Common overclaims |
|---|---|---|---|
| Prediction | Out-of-sample improvement over a competitive benchmark | Selection and updating use only information known at prediction time; evaluation matches the claim | Treating predictive power as mechanism or causation; choosing the optimum from the test set |
| Causal identification | Direction and magnitude of a treatment effect in the main specification | Evidence for identification assumptions in the main text, alternative explanations addressed individually, and inference suited to the data structure | Treating a compatible mechanism as confirmed; presenting subgroup findings as unconditional |
| Theory and calibration | Model properties and quantitative implications | Analytical proof or numerical evidence, parameter ranges, precision, and sensitivity | Treating numerical results at selected parameters as a general theorem; omitting parameter conditions from applied implications |
| Methods and simulations | Whether the method attains target properties under stated conditions | Simulation designs matched to each claim, behavior under violated conditions, and Monte Carlo error | Evaluating only in the world assumed by the method; ranking methods by noise-sized differences |
| System evaluation | Improvement over strong baselines at equal budgets | Equivalent baseline tuning, repetitions and variance, end-to-end ablations, and held-out data | Abstract numbers without definitions; broad conclusions concealing local reversals |
| Failure diagnosis | Conditions under which a common approach fails and by how much | A minimal success criterion, settings most favorable to the method under test, and stratified measurements | Using the same ideal setting to claim a correction is universally effective |

## References as needed

This file is sufficient for ordinary tasks. Read the relevant file below when finer guidance or examples are needed; loading all of them is unnecessary.

| Need | Reference |
|---|---|
| Turn results tables into analysis with clear priorities | [Results analysis](references/RESULTS.md) |
| Organize discussion and limitations | [Discussion and limitations](references/DISCUSSION.md) |
| Address objections individually, review before submission, and prioritize further analysis | [Responses to objections](references/RESPONSE.md) |
| Credibility requirements and common overclaims for a study type | [Study types](references/STUDY_TYPES.md) |
| Chinese synthetic examples | [Chinese examples](references/EXAMPLES_CN.md) |
| English synthetic examples | [English examples](references/EXAMPLES_EN.md) |
| Paper sources for the practices | [Source evidence](references/SOURCES.md) |
