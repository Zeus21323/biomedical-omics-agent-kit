# 生物医学组学 Agent 技能包

**224 个技能 + 51 个数据源工具**，不属于任何特定 agent 框架——纯 Markdown 技能目录 + 标准 MCP server，Claude Code / Cursor / Windsurf / DeepSeek Harness / 自研 agent 都能直接用。

## 里面有什么

| 部分 | 内容 | 依赖 |
|---|---|---|
| `skills/` | 224 个技能目录，每个含 `SKILL.md`（YAML frontmatter + 正文） | 无，纯文本 |
| `mcp/` | 51 个工具的 stdio MCP server，覆盖 22 个公开数据源 | Python 3.9+ 标准库，无第三方包、无 token |

技能负责**选方法、给参数、写流程**；MCP 负责**取真实数据**。两者互不依赖，可以只用其中一个。

## 技能格式

每个技能是一个目录：

```
skills/<name>/
├── SKILL.md              # 必需：YAML frontmatter + 正文
├── references/           # 可选：官方文档摘录、参数表、排错
│   ├── official-docs.md
│   ├── parameters.md
│   └── troubleshooting.md
├── scripts/              # 可选：可直接执行的脚本
└── assets/               # 可选：模板、配色、示例数据
```

`SKILL.md` 的头部：

```yaml
---
name: bulk-rnaseq
description: 端到端 bulk RNA-seq 编排：QC/修剪 → 比对定量 → counts 矩阵 → 差异表达 → 富集 → 出版级图。当用户有原始读段或 counts 矩阵并要做转录组差异分析时使用。
---

正文：方法选择、命令、参数、判读标准、常见错误。
```

**通用约定**：`name` 与目录名一致；`description` 写清"什么时候该用这个技能"，agent 靠它决定是否加载；正文只写可执行的东西（命令、参数、阈值），不写空泛建议。

## 接入方式

### 1. 任何能读文件的 agent（最通用）

把 `skills/` 放进 agent 的技能目录，或直接在提示里给出索引：

```
读 SKILLS.md 挑出与本任务相关的技能，再读对应的 SKILL.md 执行。
```

`SKILLS.md` 是 224 个技能的分类索引（技能名 + 一句话说明），适合一次性塞进上下文做路由；`SKILL.md` 只按需读取。

### 2. Claude Code / Claude Desktop

- **技能**：复制到 `~/.claude/skills/`（或项目的 `.claude/skills/`），Claude Code 会自动发现。
- **MCP**：把 `examples/claude-desktop.json` 的内容合并进 Claude Desktop 配置（macOS `~/Library/Application Support/Claude/claude_desktop_config.json`），把路径换成你的实际路径。

### 3. Cursor / Windsurf

- **技能**：放进项目的 `.cursor/rules/`，或作为 `AGENTS.md` 引用 `SKILLS.md`。
- **MCP**：把 `examples/cursor.json` 合并进 `~/.cursor/mcp.json`。

### 4. DeepSeek Harness

- **技能**：作为 skill provider 的 bundledSkillDir 指向 `skills/`，或用 `skill-filesystem` 的自定义根。
- **MCP**：用 `mcp-client` 行，命令 `python`、参数指向 `mcp/biomedical_mcp.py`。

配置细节见 `examples/generic-stdio.md`（stdio 通用说明 + 自检命令）。

## 技能分类（224）

| 主题 | 技能数 | 覆盖 |
|---|---|---|
| 转录组上游与定量 | 32 | 从 FASTQ 到表达矩阵：比对、定量、质控与批次处理 |
| 差异表达与功能富集 | 11 | 差异检验、多重校正、GSEA/ORA 与结果解释 |
| 单细胞基础分析 | 20 | QC、去双细胞、聚类、注释、轨迹 |
| 单细胞高级与虚拟细胞 | 20 | 多模态整合、扰动预测、细胞状态建模 |
| 空间组学分析 | 15 | 空间转录组、区域注释、邻域与共定位 |
| 表观遗传与 DNA 甲基化 | 31 | ATAC/ChIP 峰值、WGBS、甲基化差异 |
| 调控网络与序列模型 | 18 | GRN 推断、增强子-启动子、序列到功能模型 |
| 蛋白质组学 | 21 | 质谱定量、缺失值、修饰与 DIA |
| 代谢组与脂质糖组 | 18 | 峰识别、注释、归一化与通路映射 |
| 微生物组与宏基因组 | 38 | 分类/功能谱、多样性、差异丰度、菌群建模 |

完整清单（技能名 + 说明）见 [`SKILLS.md`](SKILLS.md)。

## MCP 工具（51 / 22 个域）

| 域 | 工具数 | 示例 |
|---|---|---|
| 基因组序列与注释 | 3 | `genomes_sequence`、`genes_lookup` |
| 变异 | 3 | `variants_gnomad`、`variants_clinvar` |
| 表达与调控 | 4 | `expression_gtex`、`regulation_roadmap` |
| 蛋白与结构 | 6 | `protein_uniprot`、`structures_pdb` |
| 化学与药物 | 6 | `chembl_compound`、`drug_opentargets` |
| 文献 | 5 | `pubmed_search_articles`、`biorxiv_recent` |
| 临床 | 4 | `clinicaltrials_search`、`cancer_depmap` |
| 单细胞图谱 | 2 | `cellguide_cell_types` |

完整清单见 [`mcp/README.md`](mcp/README.md)。

## 目录结构

```
.
├── README.md              本文件
├── SKILLS.md              224 个技能的分类索引
├── skills/                224 个技能目录
├── mcp/
│   ├── biomedical_mcp.py  51 个工具的 stdio server（纯标准库）
│   └── README.md          工具清单与说明
├── examples/
│   ├── claude-desktop.json
│   ├── cursor.json
│   └── generic-stdio.md   stdio 通用接入 + 自检
└── LICENSE                MIT
```

## 使用约定

- **技能不是软件**：`SKILL.md` 里写的工具（STAR、salmon、Scanpy、PyDESeq2…）需要你自行安装。技能负责告诉你装哪个、怎么配、参数怎么取、结果怎么判读。
- **参数默认值以官方文档为准**：技能里给的是常用起点，不是绝对标准；命令与参数冲突时以软件官方文档为准。
- **MCP 走公开 API**：受各站点未授权访问速率限制，批量调用请加间隔；部分工具在源站失败时会自动降级到等价来源。
- **不承诺数据合规**：临床、法医、人群遗传相关技能只提供方法，样本与数据的使用需自行确认伦理与法规要求。

## 许可

MIT。技能正文部分整理自各软件官方文档与社区实践，引用处已标注来源。
