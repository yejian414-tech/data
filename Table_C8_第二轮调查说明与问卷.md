# Table C.8 第二轮调查说明与问卷


## 1. 调查目的

在完成界面修改后，再次评价四个模块：

- Race Engineer；
- Coach；
- Commentary；
- AI Driver Bot。

每个模块使用与第一轮相同的两个7点评分：

1. Usefulness：1 = Not useful at all，7 = Extremely useful；
2. Ease of use：1 = Very difficult，7 = Very easy。

Table C.8 的计算关系为：

```text
Change = Second-round mean ease − First-round mean ease
```

论文的 `Usefulness` 只有一列。本文件暂按“第二轮 usefulness”处理；其确切轮次仍需用原始问卷或论文源文件确认。

## 2. 参与者与配对

建议使用第一轮相同的10名参与者和匿名编号：

| IDs | Experience | N |
|---|---|---:|
| R01–R03 | Expert | 3 |
| R04–R07 | Intermediate | 4 |
| R08–R10 | Novice | 3 |

同一 Participant ID 应连接第一轮 ease 和第二轮 ease。只有真实身份映射存在时，才能称为 paired data。

## 3. 调查流程

1. 使用修改后的统一软件版本和相同设备配置；
2. 向参与者说明本轮仍然评价系统，不评价个人能力；
3. 使用与第一轮相同的四项模块任务；
4. 每完成一个模块，立即填写该模块的 Usefulness 和 Ease；
5. 使用相同题目、相同1–7量尺和相同方向；
6. 保存 Participant ID、软件版本、模块顺序、日期、帮助次数和漏答；
7. 将第二轮 ease 与第一轮同一模块的 ease 连接后计算变化。

如果第一轮和第二轮并非同一批参与者，只能比较组均值，不能把参与者级变化或 Wilcoxon signed-rank test 写成配对分析。

## 4. 第二轮模块任务

| Task | Module | Task instruction |
|---|---|---|
| T1 | Engineer | 进入 Race Engineer，查看车辆状态，并找到系统提供的驾驶或车辆建议。 |
| T2 | Coach | 使用 `Drive now` 获取实时指导，然后进入 `Plan and review` 查看回顾或计划信息。 |
| T3 | Commentary | 查看 mode、interval、event window 和 queue/playback 状态，并观察一次 Commentary 输出。 |
| T4 | AI Driver Bot | 识别 strategy switch、运行状态和 Stop 操作，并完成一次启动和停止。 |

任务必须根据第二轮实际界面确认，且除待评价的界面修改外，应尽可能保持两轮条件一致。

---

# Participant Questionnaire / 参与者问卷

## A. Participant information

```text
Participant ID: ____________________
Evaluation round: 2
Experience group: Novice / Intermediate / Expert
Software version: __________________
Module order: ______________________
```

## B. Race Engineer

**B1. How useful was the Race Engineer for understanding the vehicle state and supporting your driving-related task?**  
Race Engineer 对理解车辆状态和支持驾驶相关任务有多大帮助？

```text
1     2     3     4     5     6     7
Not useful at all              Extremely useful
```

Selected score: `____`

**B2. How easy was the Race Engineer to understand and operate?**  
Race Engineer 是否容易理解和操作？

```text
1     2     3     4     5     6     7
Very difficult                       Very easy
```

Selected score: `____`

## C. Coach

**C1. How useful was the Coach for obtaining live guidance and reviewing or planning your driving?**  
Coach 对获取实时指导以及回顾或规划驾驶有多大帮助？

```text
1     2     3     4     5     6     7
Not useful at all              Extremely useful
```

Selected score: `____`

**C2. How easy was the Coach to understand and operate?**  
Coach 是否容易理解和操作？

```text
1     2     3     4     5     6     7
Very difficult                       Very easy
```

Selected score: `____`

## D. Commentary

**D1. How useful was Commentary for following events during the simulation?**  
Commentary 对了解模拟过程中的事件有多大帮助？

```text
1     2     3     4     5     6     7
Not useful at all              Extremely useful
```

Selected score: `____`

**D2. How easy was Commentary to understand and operate?**  
Commentary 是否容易理解和操作？

```text
1     2     3     4     5     6     7
Very difficult                       Very easy
```

Selected score: `____`

## E. AI Driver Bot

**E1. How useful was the AI Driver Bot for controlling or automating the simulated driver?**  
AI Driver Bot 对控制或自动驾驶模拟车辆有多大帮助？

```text
1     2     3     4     5     6     7
Not useful at all              Extremely useful
```

Selected score: `____`

**E2. How easy was the AI Driver Bot to understand and operate?**  
AI Driver Bot 是否容易理解和操作？

```text
1     2     3     4     5     6     7
Very difficult                       Very easy
```

Selected score: `____`

## F. Optional comments

```text
Which interface change was most helpful, and why?
哪项界面修改最有帮助？为什么？

Response: ______________________________________________

Which part is still difficult to understand or operate?
哪一部分仍然难以理解或操作？

Response: ______________________________________________
```

## 5. 数据计算

对每个模块计算：

```text
Second usefulness = 第二轮10个 Usefulness 分数的平均值
First ease = 第一轮10个 Ease 分数的平均值
Second ease = 第二轮10个 Ease 分数的平均值
Change = Second ease − First ease
```

最终输出：

| Module | Usefulness | First ease | Second ease | Change |
|---|---:|---:|---:|---:|
| Engineer |  |  |  |  |
| Coach |  |  |  |  |
| Commentary |  |  |  |  |
| AI Driver Bot |  |  |  |  |

## 6. 数据边界

- 不得把漏答填为0；
- 两轮题目和量尺方向必须相同；
- Change 使用未四舍五入的均值计算，再显示一位小数；
- 只有真实配对记录才能进行参与者级变化分析；
- 重构数据只能用于核算和图表复现；
- 开放题不得生成模拟引语；
- 该量表应称为 `a custom seven-point module-level usefulness and ease-of-use questionnaire`，不能称为经过验证的标准量表。

