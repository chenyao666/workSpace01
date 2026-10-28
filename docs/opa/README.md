# 组织过程资产（OPA）索引

| 属性 | 内容 |
|------|------|
| 版本 | 1.0 |
| 适用 | 陈尧个人/小型软件组织 |
| 对齐 | CMMI 成熟度等级 3（已定义级）过程域要点；ISO/IEC 12207:2017 主要生命周期与支持过程 |
| 声明 | **本包为过程资产与工作模板，不构成 CMMI/ISO 认证或符合性声明，亦无伪造证书。** |

## 使用说明

1. 先读 `00-governance/` 政策、架构与裁剪。
2. 项目按类型（A/B/C/D）裁剪后，复制 `04-templates/` 到项目目录填写。
3. 评审与 PPQA 使用 `03-quality/` 检查单。
4. 度量按 `05-metrics/` 最小集采集；改进与培训见 `06-improvement/`。

**假设**：小型 Java/Web 团队（可一人多角）；迭代增量交付；工具以 Git + 看板 + 文档库为主。

---

## 文件清单与映射

### 00 治理与过程架构

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [00-governance/01-org-policy.md](00-governance/01-org-policy.md) | 组织软件工程政策与强制要求 | OPF/OPD GP2.1 | 6.2.1 Life cycle model management |
| [00-governance/02-process-architecture.md](00-governance/02-process-architecture.md) | 过程分层架构、默认生命周期与门禁 | OPD | 6.2.1, 6.2.2 |
| [00-governance/03-tailoring-guide.md](00-governance/03-tailoring-guide.md) | 项目分类与裁剪矩阵、裁剪记录表 | OPD SP1.3, IPM | 6.2.1（裁剪） |

### 01 项目生命周期过程

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [01-lifecycle/01-requirements.md](01-lifecycle/01-requirements.md) | 需求获取、规格、基线与追溯 | REQM, RD | 6.4.1, 6.4.2 |
| [01-lifecycle/02-design.md](01-lifecycle/02-design.md) | 架构与详细设计、设计评审 | TS | 6.4.3, 6.4.4 |
| [01-lifecycle/03-implementation.md](01-lifecycle/03-implementation.md) | 编码、评审、构建与集成 | TS, PI | 6.4.5, 6.4.7 |
| [01-lifecycle/04-verification-validation.md](01-lifecycle/04-verification-validation.md) | 验证与确认（测试/验收） | VER, VAL | 6.4.6, 6.4.9 |
| [01-lifecycle/05-release.md](01-lifecycle/05-release.md) | 发布、部署与移交 | PI, VAL, CM | 6.4.8, 6.4.9 |
| [01-lifecycle/06-maintenance.md](01-lifecycle/06-maintenance.md) | 维护分诊、实施与退役要点 | 工程 PA + CM | 6.4.10, 6.4.11 |

### 02 项目管理过程

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [02-project-mgmt/01-initiation.md](02-project-mgmt/01-initiation.md) | 立项简表与启动批准 | PP（前置） | 6.3.1 |
| [02-project-mgmt/02-planning.md](02-project-mgmt/02-planning.md) | 项目计划编制与基线 | PP, IPM | 6.3.1 |
| [02-project-mgmt/03-monitoring.md](02-project-mgmt/03-monitoring.md) | 监控、纠正措施与状态报告 | PMC | 6.3.2 |
| [02-project-mgmt/04-risk-management.md](02-project-mgmt/04-risk-management.md) | 风险识别、应对与登记表 | RSKM | 6.3.4 |
| [02-project-mgmt/05-configuration-management.md](02-project-mgmt/05-configuration-management.md) | 配置项、基线、分支标签与审计 | CM | 6.3.5 |
| [02-project-mgmt/06-measurement.md](02-project-mgmt/06-measurement.md) | 项目度量采集与上报 | MA | 6.3.6 |
| [02-project-mgmt/07-ppqa.md](02-project-mgmt/07-ppqa.md) | 过程/产品质量保证与 NCR | PPQA | 6.3.7 |
| [02-project-mgmt/08-dar.md](02-project-mgmt/08-dar.md) | 重大决策分析与记录 | DAR | 6.3.3 |

### 03 质量保证与检查单

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [03-quality/01-peer-review-procedure.md](03-quality/01-peer-review-procedure.md) | 同行评审流程与记录字段 | VER, PPQA | 6.4.6 |
| [03-quality/02-checklist-requirements.md](03-quality/02-checklist-requirements.md) | 需求评审检查单 | REQM/RD, VER | 6.4.1, 6.4.2, 6.4.6 |
| [03-quality/03-checklist-design.md](03-quality/03-checklist-design.md) | 设计评审检查单 | TS, VER | 6.4.3, 6.4.4, 6.4.6 |
| [03-quality/04-checklist-code.md](03-quality/04-checklist-code.md) | 代码评审检查单 | TS, VER | 6.4.5, 6.4.6 |
| [03-quality/05-checklist-test.md](03-quality/05-checklist-test.md) | 测试资产评审检查单 | VER, VAL | 6.4.6, 6.4.9 |
| [03-quality/06-ppqa-checklist.md](03-quality/06-ppqa-checklist.md) | PPQA 过程/产品抽查单 | PPQA | 6.3.7 |

### 04 模板

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [04-templates/project-plan.md](04-templates/project-plan.md) | 项目计划填写模板 | PP | 6.3.1 |
| [04-templates/requirements-spec.md](04-templates/requirements-spec.md) | 需求规格（SRS）模板 | REQM, RD | 6.4.1, 6.4.2 |
| [04-templates/design-spec.md](04-templates/design-spec.md) | 设计说明模板 | TS | 6.4.3, 6.4.4 |
| [04-templates/test-plan.md](04-templates/test-plan.md) | 测试计划模板 | VER, VAL | 6.4.6, 6.4.9 |
| [04-templates/test-case.md](04-templates/test-case.md) | 测试用例模板 | VER, VAL | 6.4.6, 6.4.9 |
| [04-templates/change-request.md](04-templates/change-request.md) | 变更请求（CR）模板 | REQM, CM, PMC | 6.3.5, 6.4.2 |
| [04-templates/issue-report.md](04-templates/issue-report.md) | 问题/缺陷报告模板 | VER, VAL, PMC | 6.4.6, 6.4.10 |
| [04-templates/meeting-minutes.md](04-templates/meeting-minutes.md) | 会议纪要模板 | PMC | 6.3.2 |
| [04-templates/training-record.md](04-templates/training-record.md) | 培训记录模板 | OT | 6.2.4 |

### 05 度量

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [05-metrics/metrics-and-baselines.md](05-metrics/metrics-and-baselines.md) | 强制/可选指标与基线用法 | MA, OPF | 6.3.6 |

### 06 过程改进与培训

| 文件 | 一句话用途 | CMMI | ISO/IEC 12207 |
|------|------------|------|---------------|
| [06-improvement/process-improvement.md](06-improvement/process-improvement.md) | 过程改进循环与改进项登记 | OPF, OPD | 6.2.1, 6.2.2 |
| [06-improvement/organizational-training.md](06-improvement/organizational-training.md) | 组织培训规程与必读清单 | OT | 6.2.4 |

---

## 统计

| 类别 | 文件数 |
|------|--------|
| 治理 | 3 |
| 生命周期 | 6 |
| 项目管理 | 8 |
| 质量 | 6 |
| 模板 | 9 |
| 度量 | 1 |
| 改进与培训 | 2 |
| 本索引 | 1 |
| **合计** | **36** |

## 修订历史

| 版本 | 日期 | 说明 |
|------|------|------|
| 1.0 | 2026-10-27 | 首版 OPA 包发布（过程资产，非认证） |
