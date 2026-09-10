# Table C.4 模块有用性与易用性调查说明及问卷


## 1. 调查目的

调查分别测量参与者对四个模块的：

1. **Perceived usefulness**：参与者认为模块对完成相关任务是否有用；
2. **Perceived ease of use**：参与者认为模块是否容易理解和操作。

被评价的模块：

- Race Engineer；
- Coach；
- Commentary；
- Bot。

这是自定义的模块级7点评分问卷，不是 SUS 或 NASA-TLX。结果主要用于比较各模块及识别“功能有价值但难以使用”的模块。

## 2. 建议的参与者配置

| 项目 | 建议设置 |
|---|---|
| Participant count | 10人，与论文 Table C.4 的样本规模一致 |
| Participant ID | 使用 R01–R10 等匿名编号 |
| Experience group | Novice / Intermediate / Expert |
| Participation | 自愿参与，可随时退出 |
| Personal data | 只收集完成分析所必需的信息 |
| Data storage | 保存匿名问卷和计算表，限制访问并设定删除时间 |

经验分组必须使用事先定义的标准。例如可以依据模拟赛车使用经验、TORCS 使用经验和相关技术背景划分；实际阈值需由研究者提前确定并保存，不能在看到结果后修改。

## 3. 调查实施流程

### 3.1 调查前准备

1. 为所有参与者准备相同的软件版本、设备和初始状态；
2. 准备四个模块的标准任务；
3. 检查所有任务能够正常运行；
4. 准备匿名 Participant ID；
5. 向参与者说明评价对象是系统，不是参与者的能力；
6. 获得参与者同意后再开始记录。

### 3.2 建议任务

| Task ID | Module | Proposed task |
|---|---|---|
| T1 | Race Engineer | 启动或进入 Race Engineer，查看车辆状态信息，并找到系统提供的驾驶或车辆建议。 |
| T2 | Coach | 进入 `Drive now`，获取实时指导；随后进入 `Plan and review`，查看赛后或计划信息。 |
| T3 | Commentary | 查看 Commentary 设置，识别 mode、interval、event window、queue/playback 状态，并启动或观察 Commentary 输出。 |
| T4 | Bot | 识别 Bot 的 strategy switch、运行状态和 Stop 操作，并完成一次启动和停止。 |

以上是建议任务脚本。正式使用前，应根据实际可运行版本核对按钮名称、功能路径和前置条件。

### 3.3 填写顺序

建议每完成一个模块任务，立即填写该模块的两道题，以减少记忆误差：

```text
完成模块任务 → 填写 Usefulness → 填写 Ease of use → 进入下一个模块
```

如果所有参与者必须按同一顺序使用模块，应记录该顺序并在局限中说明潜在学习效应。若功能依赖允许，可以平衡模块顺序。

### 3.4 主持要求

- 主持人使用相同的任务说明；
- 不解释问卷中“有用”或“容易”的预期答案；
- 不使用“你为什么觉得导航困难”等引导性提问；
- 除非参与者完全无法继续，否则不提供额外操作指导；
- 如提供帮助，应记录 help request；
- 每名参与者结束后检查是否存在漏答，但不要求其改变答案。

## 4. 评分量尺

### 4.1 Usefulness

| Score | Anchor |
|---:|---|
| 1 | Not useful at all / 完全没有用 |
| 2 | Mostly not useful / 基本没有用 |
| 3 | Slightly not useful / 略微没有用 |
| 4 | Neither useful nor not useful / 中立 |
| 5 | Slightly useful / 略微有用 |
| 6 | Very useful / 很有用 |
| 7 | Extremely useful / 非常有用 |

### 4.2 Ease of use

| Score | Anchor |
|---:|---|
| 1 | Very difficult / 非常困难 |
| 2 | Difficult / 困难 |
| 3 | Slightly difficult / 略微困难 |
| 4 | Neither difficult nor easy / 中立 |
| 5 | Slightly easy / 略微容易 |
| 6 | Easy / 容易 |
| 7 | Very easy / 非常容易 |

所有模块必须使用相同的题目和锚点。

---

# Participant Questionnaire / 参与者问卷

## A. Participant information / 参与者信息

**Participant ID / 参与者编号：** `____________`

**Evaluation round / 评价轮次：**

- [ ] Round 1
- [ ] Round 2

**Experience group / 经验组：**

- [ ] Novice
- [ ] Intermediate
- [ ] Expert

**Module order / 模块体验顺序：** `____________________________`

## B. Race Engineer

**B1. How useful was the Race Engineer for understanding the vehicle state and supporting your driving-related task?**  
Race Engineer 对理解车辆状态和支持驾驶相关任务有多大帮助？

```text
1      2      3      4      5      6      7
Not useful at all                         Extremely useful
完全没有用                                      非常有用
```

Selected score / 选择分数：`____`

**B2. How easy was the Race Engineer to understand and operate?**  
Race Engineer 是否容易理解和操作？

```text
1      2      3      4      5      6      7
Very difficult                                 Very easy
非常困难                                        非常容易
```

Selected score / 选择分数：`____`

## C. Coach

**C1. How useful was the Coach for obtaining live guidance and reviewing or planning your driving?**  
Coach 对获取实时指导以及回顾或规划驾驶有多大帮助？

```text
1      2      3      4      5      6      7
Not useful at all                         Extremely useful
完全没有用                                      非常有用
```

Selected score / 选择分数：`____`

**C2. How easy was the Coach to understand and operate?**  
Coach 是否容易理解和操作？

```text
1      2      3      4      5      6      7
Very difficult                                 Very easy
非常困难                                        非常容易
```

Selected score / 选择分数：`____`

## D. Commentary

**D1. How useful was the Commentary module for following events during the simulation?**  
Commentary 模块对了解模拟过程中的事件有多大帮助？

```text
1      2      3      4      5      6      7
Not useful at all                         Extremely useful
完全没有用                                      非常有用
```

Selected score / 选择分数：`____`

**D2. How easy was the Commentary module to understand and operate?**  
Commentary 模块是否容易理解和操作？

```text
1      2      3      4      5      6      7
Very difficult                                 Very easy
非常困难                                        非常容易
```

Selected score / 选择分数：`____`

## E. Bot

**E1. How useful was the Bot module for controlling or automating the simulated driver?**  
Bot 模块对控制或自动驾驶模拟车辆有多大帮助？

```text
1      2      3      4      5      6      7
Not useful at all                         Extremely useful
完全没有用                                      非常有用
```

Selected score / 选择分数：`____`

**E2. How easy was the Bot module to understand and operate?**  
Bot 模块是否容易理解和操作？

```text
1      2      3      4      5      6      7
Very difficult                                 Very easy
非常困难                                        非常容易
```

Selected score / 选择分数：`____`

## F. Optional comments / 可选意见

**F1. Which module was most useful, and why? / 哪个模块最有用？为什么？**

```text


```

**F2. Which module was most difficult to use, and what caused the difficulty? / 哪个模块最难使用？困难是什么？**

```text


```

**F3. What is the single most important change you would make? / 你认为最重要的一项改进是什么？**

```text


```

---

## 5. 原始数据记录格式

| Participant | Group | Round | Engineer-U | Engineer-E | Coach-U | Coach-E | Commentary-U | Commentary-E | Bot-U | Bot-E |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| R01 |  | 1 |  |  |  |  |  |  |  |  |
| R02 |  | 1 |  |  |  |  |  |  |  |  |
| R03 |  | 1 |  |  |  |  |  |  |  |  |
| R04 |  | 1 |  |  |  |  |  |  |  |  |
| R05 |  | 1 |  |  |  |  |  |  |  |  |
| R06 |  | 1 |  |  |  |  |  |  |  |  |
| R07 |  | 1 |  |  |  |  |  |  |  |  |
| R08 |  | 1 |  |  |  |  |  |  |  |  |
| R09 |  | 1 |  |  |  |  |  |  |  |  |
| R10 |  | 1 |  |  |  |  |  |  |  |  |

`U = Usefulness`；`E = Ease of use`。

## 6. 计算方法

对每个模块分别计算平均有用性和平均易用性：

```text
Mean Usefulness = 所有有效 Usefulness 分数之和 ÷ 有效回答人数
Mean Ease = 所有有效 Ease 分数之和 ÷ 有效回答人数
Gap = Mean Usefulness − Mean Ease
```

以 Race Engineer 为例：

```text
Mean Usefulness = 58 ÷ 10 = 5.8
Mean Ease = 32 ÷ 10 = 3.2
Gap = 5.8 − 3.2 = 2.6
```

最终输出格式：

| Module | Usefulness | Ease | Gap |
|---|---:|---:|---:|
| Race Engineer |  |  |  |
| Coach |  |  |  |
| Commentary |  |  |  |
| Bot |  |  |  |

## 7. 缺失值处理

- 不得凭空填写漏答；
- 不建议用其他参与者的均值替代；
- 每个模块同时报告有效回答人数 `n`；
- 如果某位参与者没有实际完成一个模块的任务，该模块评分应标记为空，不应要求其猜测；
- 开放题仅进行真实回答的主题归类，不生成模拟引语。

## 8. 两轮比较

如果同一参与者参加两轮评价：

- 两轮使用相同匿名 ID；
- 使用相同任务和量尺；
- 记录软件版本、日期和模块顺序；
- 分别计算每个模块两轮的均值；
- 只有获得真实配对回答后，才可以考虑进行 Wilcoxon signed-rank test；
- 重构数据不能用于报告 p-value、effect size 或 statistical significance。

## 9. 报告中的准确名称

建议称为：

```text
a custom seven-point module-level usefulness and ease-of-use questionnaire
```

不要称为：

```text
a validated usability scale
```

除非能够提供该量表的验证来源。

## 10. 课程依据

- `SE/lecture/8a HCI Evaluation Part Two 2025.pdf`，PDF第4页：避免引导性问题、控制问卷长度，并优先使用经过验证的问卷；
- 同一讲义第18–24页：标准化 SUS 的实施时间和计分方式，可作为系统级量表，与本模块级自定义问卷区分；
- 同一讲义第31–33页：within-subject 与 between-subject 设计及学习效应；
- `SE/lab/8b - Quantitative Evaluation.pdf`，PDF第2页：任务完成后填写问卷、计算聚合结果，并在真实配对数据存在时选择配对分析。

