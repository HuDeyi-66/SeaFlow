# SeaFlow

**证据优先 · 来源可追溯 · 小核心 · 可扩展 Skills**

SeaFlow 由私有应用 Core 与六个独立归属的 Skill 组成。本仓库仅提供公共架构与项目入口。

| Skill | 职责 | 可用范围 |
|---|---|---|
| [海珊 ShanHai](https://github.com/HuDeyi-66/Shan_Hai_Code_Skill) | 法律文本结构、精确片段与引用候选 | 公开 |
| [海珞 LuoHai](https://github.com/HuDeyi-66/Luo_Hai_Tables_Skill) | 工作簿/单元格重建与损失记账 | 公开 |
| 海玟 WenHai | 文书登记、转录、证据分段与署名建议 | 仅本地 |
| 海琛 ChenHai | 证据充分性与研究过程评估 | 已接受实现保持私有 |
| [海珏 JueHai](https://github.com/HuDeyi-66/Jue_Hai_Graph_Skill) | 有界溯源图、主张权限与有限样本公式 | 公开 |
| [海现 XianHai](https://github.com/HuDeyi-66/Xian_Hai_Time_Skill) | 时间知识、状态、准入与复核计划 | 公开 |

四个公开 Skill 可独立使用，无需私有 Core。Core 负责应用适配、来源身份边界与跨 Skill 编排。
已接受的私有 ChenHai 充分性实现与历史公开探索原型是不同项目；WenHai 没有公开远程仓库。

当前资格是有界的内部 V3.5 合成工程验收。Pre-3.6 精选回归包含 150 个唯一用例、156 次执行；
其口径不同于历史 1,064 个用例（1,048 通过、16 个可选跳过）。这些结果不是独立外部评审、
真实语料精度、法律专家验证、生产就绪或 V3.6 基准验收。V3.6 外部基准仍待开展。

各公开 Skill 的 README 与 `docs/PRE36_QUALIFICATION.md` 提供安装、展示及安全回归命令。
来源字节、派生表示与研究判断保持区分；缺失、歧义、未知和不支持状态不会被自动补全。

## 本地 V3.6 英文引用修复

本地任务 `SF36-ENG-P0-ENGLISH-CITATION-001` 已验证 ShanHai 显式文书片段模式，
并通过实际 SeaFlow QueryService 引用原先准入的 **10 个 CUAD 原生上下文**。
原生引用绑定来源哈希、表示身份及可重建的码点／字节偏移；英文法条解析和法律效力仍未取得资格。

探索性 **90 问／415 分块**三方法检索候选比较已完成，沿用 Top-1／Top-5 与 6,000 码点预算。
历史 BM25 和 MiniLM 基线保持封存。第三方法为 **SeaFlow 应用精确词项排序 + ShanHai 文书片段引用治理**，
未将 BM25／MiniLM 排序重命名为独立 SeaFlow 算法。检索排序归应用编排；忠实来源的证据与引用契约归独立 ShanHai。

90 问均返回可重建引用候选；QueryService 回答 34 问、拒绝 56 问。
检索候选指标包括拒绝包中返回的候选，不衡量回答正确性。两个独立的固定 CPU 进程复现排序及预算内引用。
本选定试点中的字符 F1 低于两条封存基线；引用工程资格不表示检索性能提升。

工程决定：`V3_6_ENGLISH_SOURCE_CITATION_REPAIR_PASS`。
实验决定：`SF36_CUAD_THREE_WAY_COMPARISON_PASS`，仅限上述描述性检索候选比较。
原试点 `SF36_FAST_PILOT_002_PARTIAL` 及历史结果不变。本地证据位于私有工作区的
`Exam_Field/Active/V3_6/English_Citation_Repair/` 与
`Test_Records/Test_Outputs/V3_6_English_Citation_Repair/Run_001/`；本仓库不公开 CUAD 上下文或标签。

本次范围与历史 V3.5 合成集成验收分开；不是官方 LegalBench-RAG、独立法律专家验证、
冻结的确证性 P0 证据、统计显著性或六 Skill 全能力验收。P1G 操作保留项及来源用途边界保持有效。
这些仅为本地 README 修改；公开同步需要所有者另行批准。

[六 Skill 公共展示](https://hudeyi-66.github.io/seaflow-library-project-control/) ·
[完整英文架构入口](README.md) · [当前 GitHub 个人主页](https://github.com/HuDeyi-66)

本仓库文档采用 MIT 许可证，参见 `LICENSE` 与 `NOTICE.md`。公开 Skill 以各自许可证为准。
此处不授予私有 Core、私有 ChenHai 或任何私有材料的许可。
