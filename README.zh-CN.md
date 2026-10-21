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

[六 Skill 公共展示](https://hudeyi-66.github.io/seaflow-library-project-control/) ·
[完整英文架构入口](README.md) · [当前 GitHub 个人主页](https://github.com/HuDeyi-66)

本仓库文档采用 MIT 许可证，参见 `LICENSE` 与 `NOTICE.md`。公开 Skill 以各自许可证为准。
此处不授予私有 Core、私有 ChenHai 或任何私有材料的许可。
