---
type: wcca
category: cross
status: draft
version: 0.1.0
wcca_relevant: true
tags:
  - wcca
  - index
created: 2026-11-01
updated: 2026-11-01
---

# WCCA关联索引

## WCCA 知识文档
方法类文档（按分析流程顺序阅读）：

- [[WCCA基础方法]] — 分析目的、边界、最坏情况组合的枚举规则
- [[参数上下限提取方法]] — 从 Datasheet 取极值的步骤与资料不足时的处理
- [[温度影响计算]] — 温度敏感参数与修正方法
- [[降额设计方法]] — 降额准则与降额和裕量的关系
- [[元器件WCCA参数映射表]] — 各器件类别参与计算的参数汇总载体
- [[WCCA参数映射模板]] — 新增映射行时使用的表格模板

## 器件类别与 WCCA 参数
规划表：Phase 0 只确定「哪些器件类别需要哪些主参」，具体参数名与取值待 Phase 6 依 Datasheet 补齐。

| 器件类别 | 入口文档 | 主参 WCCA 参数 | 状态 |
|---|---|---|---|
| 电阻 | [[电阻_索引]] | 待 Phase 6 填写 | planned |
| MLCC | [[MLCC_索引]] | 待 Phase 6 填写 | planned |
| 铝电解电容 | [[铝电解电容_索引]] | 待 Phase 6 填写 | planned |
| 功率电感 | [[功率电感_索引]] | 待 Phase 6 填写 | planned |
| 共模电感 | [[共模电感_索引]] | 待 Phase 6 填写 | planned |
| 磁珠 | [[磁珠_索引]] | 待 Phase 6 填写 | planned |
| 二极管 | [[二极管_索引]] | 待 Phase 6 填写 | planned |
| MOSFET | [[MOSFET_索引]] | 待 Phase 6 填写 | planned |
| 三极管 | [[三极管_索引]] | 待 Phase 6 填写 | planned |
| IGBT | [[IGBT_索引]] | 待 Phase 6 填写 | planned |
| 光耦 | [[光耦_索引]] | 待 Phase 6 填写 | planned |
| 无源晶体 | [[无源晶体_索引]] | 待 Phase 6 填写 | planned |
| 有源晶振 | [[有源晶振_索引]] | 待 Phase 6 填写 | planned |
| 逻辑门 | [[逻辑门_索引]] | 待 Phase 6 填写 | planned |
| 缓冲器与反相器 | [[缓冲器与反相器_索引]] | 待 Phase 6 填写 | planned |
| 电平转换器 | [[电平转换器_索引]] | 待 Phase 6 填写 | planned |
| 施密特触发器 | [[施密特触发器_索引]] | 待 Phase 6 填写 | planned |
| 运算放大器 | [[运算放大器_索引]] | 待 Phase 6 填写 | planned |
| 比较器 | [[比较器_索引]] | 待 Phase 6 填写 | planned |

## 待补全项
Phase 6 需要补齐的条目（本阶段只登记，不填写）：

1. 每个器件类别的主参 WCCA 参数清单，逐项给出符号与单位。
2. 每个参数的取 Min 或 Max 判据，说明电路行为为何要求该方向的极值。
3. 温度与偏压修正公式及其适用温区，标注不适用区间。
4. 每个参数在 Datasheet 中的页码与表号，必要时补曲线编号。
5. 不可直接用于计算的参数清单，以及替代方案或附加确认要求。
6. 与 [[参数上下限提取方法]] 的步骤编号对齐，确保映射表可反查方法条。
