# 汽车电子基本元器件知识库

面向汽车电子与 BMS 控制器硬件开发的元器件知识框架。当前以 Obsidian Markdown 为主要维护载体，逐步建立可追溯的 Datasheet 参数记录和 WCCA 参数映射。

## 当前范围

- **Phase 0 — 框架与模板**：目录、知识规范、模板、导航和质量检查。
- **Phase 1 — 器件试点**：计划从电阻开始，验证模板、参数 ID、Datasheet 版本和数据追溯流程。
- **Phase 2 — 结构化数据模型**：根据试点结果确定字段和关联关系，再评估 YAML/JSON 等形式。
- **Phase 3 — AI/WCCA 接入**：在数据模型稳定后，设计面向 WorkBuddy/工程 Skill 的读取与计算流程。

当前仓库只维护知识框架与模板，不承载企业内部项目数据或未经授权的厂商资料。

## 目录导航

| 目录 | 用途 |
|---|---|
| `00_Home` | 首页、分类索引、WCCA 关联索引 |
| `01_Fundamentals` | Datasheet 阅读、参数定义、统一 ID、数据来源规则 |
| `02_Passive_Components` | 电阻、电容、电感、磁珠等无源器件 |
| `03_Semiconductor_Components` | 二极管、MOSFET、BJT、IGBT、光耦等 |
| `04_Timing_Components` | 晶体与有源晶振 |
| `05_Logic_Components` | 逻辑门、缓冲器、电平转换等 |
| `06_Analog_Components` | 运放、比较器等 |
| `07_Datasheet_Cases` | 具体型号与 Datasheet 版本案例 |
| `08_WCCA_Knowledge` | WCCA 方法、参数映射与修正方法 |
| `09_Templates` | 通用知识、Datasheet 案例、WCCA 映射模板 |
| `99_Management` | 建设计划、变更记录、待确认项与质量检查 |

## 使用流程

1. 从 `00_Home/首页.md` 或分类索引进入器件类别。
2. 复制 `09_Templates/元器件通用知识模板.md` 建立类别知识入口。
3. 为具体型号复制 `09_Templates/Datasheet案例模板.md`，记录原厂来源、文档版本、条件和数据记录。
4. 经评审后，使用 `09_Templates/WCCA参数映射模板.md` 将参数映射到分析目标和公式。
5. 框架变更同步更新首页、目录树、更新记录和质量检查。

## 数据与工程纪律

- 参数必须能够追溯到原厂 Datasheet 的具体版本、页码/表格/曲线和测试条件。
- 典型值、读图值、保证值、计算值、工程假设值和待确认值必须分开标识。
- Absolute Maximum Ratings 不作为正常工作条件。
- WCCA 极值方向由具体分析目标和电路传递关系确定，不能固定套用。
- Markdown 是当前阶段的主要维护入口；结构化数据形式待试点验证后再确定。避免同一事实在多份文件中长期手工重复维护。
- 不上传公司内部 BOM、原理图、DFMEA、内部 Datasheet 或项目数据到公开仓库。公开资料也应遵守原厂版权与许可。

## 模板

- [元器件通用知识模板](09_Templates/元器件通用知识模板.md)
- [Datasheet 案例模板](09_Templates/Datasheet案例模板.md)
- [WCCA 参数映射模板](09_Templates/WCCA参数映射模板.md)

## 状态

当前为框架和模板修订阶段。真实器件数据录入尚未开始；框架质量检查不等同于真实器件工程验证。
