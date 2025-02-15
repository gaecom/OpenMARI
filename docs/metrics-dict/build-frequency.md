---
sidebar_label: '构建次数'
---

# 构建次数

| 属性   |                                                             |
| ---- | ----------------------------------------------------------- |
| 指标定义 | 单位时间内软件进行编译构建的次数。持续构建有助于及早发现缺陷和修复缺陷。                        |
| 指标价值 | 从项目的维度展示各个周期的构建次数、构建成功次数以及构建成功率。快速定位构建出现的问题，同时直观的了解项目的构建情况。 |
| 指标来源 | CI/CD系统                                                     |
| 实践域  | 开发、测试、发布                                                    |
| 认知域  | 交付能力                                                        |
| 度量范围 | 项目                                                          |

## MARI 方法

### 度量

* 统计项目维度构建总次数、构建成功次数、构建失败次数。
* 统计周期内构建总次数、构建成功次数、构建失败次数。

![](img/gou-jian-ci-shu-1.png)

* 分别统计开发、测试、发布阶段构建总次数、构建成功次数、构建失败次数。

### 分析

* 按项目维度，横向分析、对比不同项目的构建次数，对最大值、最小值或者低于平均值的项目进行下钻分析。
* 按阶段下钻分析开发、测试、发布阶段的构建次数，分析各阶段构建次数的合理性，找到瓶颈点。
* 分析各个周期内构建次数的变化趋势，进行纵向对比，对最大值、最小值、连续上升、连续下降的周期进行调研。

### 回顾

针对构建次数出现异常的项目和迭代周期，进行根本原因的分析、调研和回顾。

以构建次数偏少/降低为例，进行如下根因分析：

* 上游的需求、开发任务是否饱满、均匀？
* 开发人员是否每日小步多次提交？
* 构建过程是否自动化？
* 构建自动化的调度机制是否高效？

### 改进

基于回顾结果，聚焦关键根因，从规范、流程、工具、行为等方面给出针对性改进措施，明确提升目标、改进措施、验证周期及责任人。

以构建次数偏少/降低为例，以下为可参考的改进思路：

* 合理进行需求排期和任务分配，避免人等活的情况。
* 需求/任务颗粒度尽量小，提倡每日小步多次提交。
* 自动化构建过程，要求构建自动化率达到100%。
* 调整自动化构建的调度机制，提高构建吞吐量。

改进成果也应当是可量化的，便于持续度量，追踪改进效果。

