<p align="center">
  <img src="assets/cover.png" alt="BioSeeki — 面向生命科学的个人科研工作台" width="1400" />
</p>

<p align="center"><a href="README.md">English</a> · <strong>简体中文</strong></p>
<p align="center">
  <a href="https://bioseeki.com/download"><strong>下载 Mac Beta</strong></a> ·
  <a href="https://bioseeki.com/">访问官网</a> ·
  <a href="https://bioseeki.com/changelog">更新日志</a> ·
  <a href="docs/getting-started.zh-CN.md">开始使用</a> ·
  <a href="https://github.com/zjuphD/BioSeeki/issues">问题反馈</a>
</p>

**BioSeeki 是安装在电脑上、围绕课题持续工作的个人科研 AI 工作台。** 面向生命科学研究，将文献翻译与对照阅读、深度研究、数据分析、实验记录、分子设计和论文汇报放在同一个课题空间。

课题文件、带来源的知识库、可管理的记忆与实际生成的成果连接多次工作。这里汇集产品介绍、架构图、使用指南、功能更新和用户反馈。

## 让工作接上已有的研究

- **以课题为单位。** 论文、数据、序列、实验记录与成果保存在本地课题目录，可以跨会话继续使用。
- **知识库与记忆各司其职。** 知识库回答“材料里写了什么”；记忆保留课题事实、个人偏好、纠正和重要决定。
- **从阅读到实际工作。** 围绕问题检索证据、运行分析、生成图表、记录实验，或在 GeneCode 中查看序列设计。
- **成果能够继续修改。** 结果文件、脚本、来源位置与可编辑序列留在课题中，方便核对、重绘和后续写作。
- **科研判断由你掌握。** 回读证据、检查分析条件，预览并确认序列修改。

## 整体架构

<a href="assets/architecture/Fig1_BioSeeki_architecture_en.png"><img src="assets/architecture/Fig1_BioSeeki_architecture_en.png" alt="BioSeeki 英文架构图：本地课题工作区、智能体上下文与任务循环、知识库和记忆、科研工具，以及在线模型与文献服务。" width="1400" /></a>

智能体结合当前问题与课题上下文，组织任务、调用工具、检查结果并继续工作。本地文件、知识库、记忆和科研工具支持执行；模型推理、文献检索及公共数据库通过网络提供服务。

**[查看三张英文架构与功能图、完整图注和 SVG 版本 →](docs/architecture.md)**

## 知识库保留证据，记忆延续课题

<a href="assets/architecture/Fig2_Knowledge_and_memory_en.png"><img src="assets/architecture/Fig2_Knowledge_and_memory_en.png" alt="英文知识库与记忆图：原始材料形成带来源的检索索引，全局记忆和课题记忆保存可查看、修改、确认与遗忘的上下文。" width="1400" /></a>

| | 知识库 | 记忆系统 |
| --- | --- | --- |
| **保存什么** | 原始资料与可检索的正文片段。 | 可复用的个人与课题背景。 |
| **解决什么问题** | “这篇论文或记录具体怎么说？” | “我们之前已经确认、纠正或决定了什么？” |
| **返回什么** | 相关正文及其文档、页码或段落位置。 | 与当前任务有关的偏好、事实、纠正和研究进展。 |
| **如何管理** | 选择课题资料，随时回看原文。 | 分开管理全局与课题记忆，查看、修改、确认或遗忘。 |

夜间整理按所选记忆策略运行，帮助归纳可复用背景；原始研究材料仍可回查。

## 各项科研功能与交付成果

<a href="assets/architecture/Fig3_Research_capabilities_en.png"><img src="assets/architecture/Fig3_Research_capabilities_en.png" alt="英文功能图：文献翻译对照阅读、深度研究与文献追踪、数据分析、实验记录、GeneCode 分子设计和写作引用核对。" width="1400" /></a>

| 功能 | 可以怎样工作 | 留下什么 |
| --- | --- | --- |
| **文献翻译与对照阅读** | 原文与译文对照，解释图表，跳回支持结论的段落。 | 对照译文、阅读笔记与来源位置。 |
| **深度研究** | 明确研究问题，检索公共文献和课题资料，比较证据后整理综述。 | 证据台账、文献清单与研究报告。 |
| **文献雷达** | 持续跟进课题主题，在日报与周报中查看相关新增文献。 | 新文献、摘要与检索状态。 |
| **数据分析与科研绘图** | 检查数据结构和样本分组，使用 Python/R 分析，并调整图表与参数。 | 结果表、图表、脚本和执行记录。 |
| **实验记录** | 整理目的、样本、试剂、步骤、观察和附件，预览并导出记录。 | 可编辑记录、附件、Word 与 PDF 文件。 |
| **GeneCode 分子设计** | 查看序列、质粒图谱、注释、翻译、酶切和比对，协作设计克隆与引物。 | 可编辑序列、候选引物、质控结果和修改提案。 |
| **论文写作与引用核对** | 围绕课题材料写作，关联论断与证据，核对 DOI、发表版本和撤稿状态。 | 文稿、带来源的论断与引用核对报告。 |
| **汇报与 PPT** | 将论文、数据和图表整理成研究报告或组会汇报。 | 可编辑幻灯片、逐页讲稿与来源。 |

图中为架构与功能示意，不代表某次实验结果或性能测试。具体分析取决于所提供的材料、研究设计及可用工具。

## 一个课题，可以这样连着推进

以荧光蛋白相关课题为例：

1. 将论文和已有实验记录收录到课题知识库。
2. 对照阅读原文与译文，比较不同来源的证据。
3. 在 **GeneCode** 打开载体与插入序列，检查设计提案并确认需要的修改。
4. 分析实验数据，保存脚本与图表，整理实验记录。
5. 沿用课题背景完成论文或组会汇报，再由文献雷达跟进新进展。

也可以只从其中一个任务开始，无须按固定流程使用。

## 本地工作与在线服务

| 在你的电脑上 | 按需联网 |
| --- | --- |
| 课题文件与生成成果。 | BioSeeki 账号和模型服务。 |
| 知识库索引与可管理的记忆。 | 为模型推理提供所选的任务相关上下文。 |
| 本地文件工具、分析运行环境与 GeneCode 工作台。 | 文献检索和公共科研数据库。 |

BioSeeki 是桌面软件，模型任务与在线检索需要网络连接。数据处理说明见[隐私政策](https://bioseeki.com/privacy)。

## 下载与安装

**[从官网下载 BioSeeki →](https://bioseeki.com/download)**

| 平台 | 公开下载情况 |
| --- | --- |
| **macOS** | **Beta 0.1.7**，Apple 芯片 M 系列，macOS 14 及以上。 |
| Windows / Intel Mac | 暂未开放公开下载。 |

1. 下载并打开 DMG，双击 **BioSeeki Beta**。
2. 按提示点击**安装到应用程序**，完成后自动打开。也可以拖入 **Applications** 文件夹安装。
3. 登录或注册 BioSeeki 账号，选择课题目录，添加材料并描述希望得到的成果。

Mac Beta 已签名并通过 Apple 公证。[下载页](https://bioseeki.com/download)提供当前安装说明与 SHA-256 校验值。更新前请保存工作并退出旧版。

**[开始使用与常用场景](docs/getting-started.zh-CN.md)** · **[功能更新日志](https://bioseeki.com/changelog)**

## 可以直接这样开始

> **读文献：** 打开这篇 PDF 做原文与译文对照阅读，解释图 2，并标出支持结论的原文位置。

> **分析数据：** 先检查列名、缺失值和样本分组，说明分析方法，再输出结果表、图表与脚本。

> **记实验：** 把这些笔记和附件整理成带日期的实验记录，预览后导出 PDF。

> **看序列：** 检查载体与插入序列的连接位置和阅读框，在 GeneCode 中展示提案。

> **做汇报：** 将这些结果做成 10 分钟组会汇报，提供可编辑 PPT、逐页讲稿和引用来源。

## 反馈与交流

- [提交问题反馈](https://github.com/zjuphD/BioSeeki/issues/new?template=bug_report.yml)或[提出功能建议](https://github.com/zjuphD/BioSeeki/issues/new?template=feature_request.yml)。
- 在 [Discussions](https://github.com/zjuphD/BioSeeki/discussions) 分享使用方法和科研场景。
- 账号、费用及需要私下处理的问题：[support@bioseeki.com](mailto:support@bioseeki.com)。

公开 Issue 请使用脱敏示例。安全漏洞请通过[私下联系渠道](SECURITY.md)报告。

点一个 **Star**，让更多科研人员发现 BioSeeki；也欢迎向课题组分享[官网](https://bioseeki.com/)和这个仓库。

---

[官网](https://bioseeki.com/) · [下载](https://bioseeki.com/download) · [更新日志](https://bioseeki.com/changelog) · [隐私政策](https://bioseeki.com/privacy) · [服务条款](https://bioseeki.com/terms) · [仓库说明](NOTICE.md)
