# 合成教学例

本页的研究对象、设计、审稿意见与数值均为合成材料。两例根据项目已有任务整理，成文为公开阅读而编排，不是论文原文、真实审稿记录或未经编辑的首次输出。中文例说明如何同时报告相对改善与代价，英文例说明如何依据随机分配保留因果结论并回应误读。

## 中文例　转折识别速度与误报

### 研究材料

研究考察新增序列状态模块能否缩短金融时间序列的转折识别延迟，以及缩短延迟的代价。方法 G 与基准 B 使用相同输入，唯一差别是 G 加入该模块。模型、阈值和调参流程在评估前冻结，每次评估只使用当时已知的数据。

测试包含12条独立模拟序列，每条序列由生成机制预先定义8次转折，共96次。两种方法都在预设5日窗口内检出这96次转折。延迟定义为转折实际发生到首次报警的交易日数。配对比较先按序列计算，再以序列为单位重采样得到区间。

B 的平均检测延迟为2.8个交易日，G 为1.2个交易日。G 相对 B 的配对差为−1.6个交易日，95%区间为［−2.1，−1.1］。在事先选定的1000个非事件窗口中，B 有40个窗口报警，G 有70个，误报比例分别为4.0%和7.0%。配对差为3.0个百分点，95%区间为［1.0，5.0］。误报比例的分母是非事件窗口数。

原稿将结果概括为“状态模块消除了识别滞后，实现了检测性能的全面提升”。合成审稿意见则认为，G 仍平均滞后1.2个交易日，所以没有证据表明它比基准更快，要求撤回提速结论。作者需要结果正文与简短回应，尚未修改稿件。

### 结果分析

在给定的12条独立模拟序列中，新增序列状态模块缩短了转折识别的平均延迟。方法 G 的平均延迟为1.2个交易日，低于基准 B 的2.8个交易日；配对差为−1.6个交易日，95%区间为［−2.1，−1.1］。两种方法检出了同一组96次转折，延迟比较覆盖全部预设事件。

两种方法使用相同输入，唯一差别是 G 加入了状态模块，因此该对照反映模块在本次评估中的增量作用。模型、阈值和调参流程均在评估前冻结。区间以独立序列为单位重采样，使同一序列内的事件保留在一起。

识别速度的改善伴随着更多误报。在事先选定的1000个非事件窗口中，G 有70个窗口报警，B 有40个，误报比例分别为7.0%和4.0%。配对差为3.0个百分点，95%区间为［1.0，5.0］。在转折检出数相同的条件下，G 的平均识别延迟更短，非事件窗口误报比例更高。

### 拟议回应

G 平均仍滞后1.2个交易日，并不否定其相对提速。B 的平均延迟为2.8个交易日，配对差为−1.6个交易日，95%区间为［−2.1，−1.1］，支持保留缩短延迟的结论。原句将提速写成消除滞后，并忽略了误报增加的代价，拟替换为“在给定评估样本中，状态模块缩短了平均识别延迟，但提高了非事件窗口误报比例”。

### 这一例的判断

原稿的全面改善与审稿意见的没有优势，都没有准确表达这组比较。正文保留延迟下降及其区间，同时报告误报增加。回应引用同一个直接比较，修改超出证据的部分，拟议文字也按实际状态呈现。

## English example　A randomized display experiment

### Material

The study asks whether a new display changes the probability of a correct decision in a simulated portfolio-choice task. A computer randomly assigned 800 participants, 400 per arm, to the new or standard display. The task, incentives, information shown, and available choices were identical. All participants completed the task and were analysed according to assignment. Each participant saw only the assigned display and made one scored choice.

Randomisation and the analysis plan were fixed before recruitment. The registered analysis used a linear probability regression of correctness on assignment, with HC2 standard errors and no covariates. Section 2.2 of the manuscript already described these design details, and Table 1 labelled the contrast as the effect of assignment. The authors had not edited the manuscript after receiving the review.

There were 240 correct decisions among the 400 participants assigned to the standard display and 284 among the 400 assigned to the new display. The corresponding rates were 0.60 and 0.71. The reported assignment coefficient was 0.110, with a 95% interval of [0.045, 0.175]. No participant exclusions, outcome-dependent adjustments, or additional treatments occurred.

### Synthetic reviewer comment

“The effect is estimated with a regression, so it can only be an association. There is no random allocation described, and causal wording should be removed throughout. Did you select the regression controls after observing the outcomes?”

### Draft response

The causal interpretation is supported by random assignment, which is explicitly described in Section 2.2. A computer randomly assigned 800 participants, 400 per arm, to the new or standard display. All assigned participants completed the task and were analysed according to assignment. The task, incentives, information shown, and available choices were identical across arms; only the presentation changed. Table 1 accordingly labels the contrast as the effect of assignment. Using regression to estimate this randomized contrast does not make it merely an association.

The registered analysis included no covariates, and the analysis plan was fixed before recruitment. There were no participant exclusions or outcome-dependent adjustments. The randomized design supports retaining the claim that assignment to the new display increased the probability of a correct decision in this experiment. We propose the following results paragraph to state the design and contrast together.

### Proposed results paragraph

In the randomized experiment, 284 of 400 participants assigned to the new display made the correct decision (71%), compared with 240 of 400 assigned to the standard display (60%). Assignment to the new display increased the probability of a correct decision by 11 percentage points, with a 95% confidence interval of 4.5 to 17.5 percentage points. The estimate comes from the registered linear probability regression with no covariates and HC2 standard errors. All 800 participants completed the task and were analysed according to assignment. The outcome was the single scored choice in the simulated portfolio-choice task.

### Interpretation

The response points to the randomized assignment already described in the manuscript and directly answers the question about control selection. It retains the supported causal claim and presents the replacement as proposed text. The scientific claim, the evidence cited in the response, and the status of the manuscript remain consistent.

## 延伸阅读

更多结果分析、讨论与逐条回应的完整示范，见[中文实例](../references/EXAMPLES_CN.md)与[英文实例](../references/EXAMPLES_EN.md)。规范的来源范围和核对方式见[开发说明](DEVELOPMENT.md)。
