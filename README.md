<p align="center">
  <img src="assets/cover.png" alt="BioSeeki — a personal research workspace for life sciences" width="1400" />
</p>

<p align="center"><strong>English</strong> · <a href="README.zh-CN.md">简体中文</a></p>
<p align="center">
  <a href="https://bioseeki.com/download"><strong>Download Mac Beta</strong></a> ·
  <a href="https://bioseeki.com/en">Website</a> ·
  <a href="CHANGELOG.md">Changelog</a> ·
  <a href="docs/getting-started.md">Getting started</a> ·
  <a href="https://github.com/zjuphD/BioSeeki/issues">Feedback</a>
</p>

**BioSeeki is a personal AI research workspace for life sciences, installed on your computer and organized around your projects.** Read and translate papers, investigate a question, analyze data, keep experimental records, work with sequences, and develop manuscripts and presentations in the same workspace.

The work continues through project files, source-linked knowledge, manageable memory and saved outputs. This repository brings together the product introduction, architecture figures, practical guides, updates and community feedback.

## A workspace that stays with your research

- **Your project is the unit of work.** Keep papers, tables, sequences, experimental records and generated files in a local project folder, and return to them across conversations.
- **Knowledge and memory have different jobs.** The knowledge base retrieves evidence from documents; memory preserves reusable context such as project facts, preferences, corrections and decisions.
- **Reading connects to doing.** Move from a paper or research question to literature synthesis, analysis scripts, figures, records or a sequence design.
- **Outputs remain usable.** Continue editing the actual files, inspect source locations and analysis conditions, or reopen a design in GeneCode.
- **You retain scientific judgment.** Review evidence and proposed sequence edits before using the result in your research.

## How BioSeeki works

<a href="assets/architecture/Fig1_BioSeeki_architecture_en.png"><img src="assets/architecture/Fig1_BioSeeki_architecture_en.png" alt="BioSeeki architecture: a local project workspace, an agent context–plan–act–inspect loop, knowledge and memory, scientific tools, and connected online services; evidence and outputs persist across sessions." width="1400" /></a>

The desktop agent combines the current question with project context, chooses tools, inspects their results and continues the task. Local files, knowledge, memory and scientific tools support the work; model reasoning, literature retrieval and public databases use online services.

**[View all three architecture figures, full captions and SVG versions →](docs/architecture.md)**

## Knowledge for evidence. Memory for continuity.

<a href="assets/architecture/Fig2_Knowledge_and_memory_en.png"><img src="assets/architecture/Fig2_Knowledge_and_memory_en.png" alt="Source documents form a local retrieval index, while global and project memory preserve context that users can view, edit, confirm or forget. Both contribute to the current task." width="1400" /></a>

| | Knowledge base | Memory |
| --- | --- | --- |
| **Keeps** | Source documents and searchable passages. | Reusable personal and project context. |
| **Helps answer** | “What does this paper or record actually say?” | “What have we already established or decided?” |
| **Returns** | Relevant text with document and source locations. | Relevant preferences, facts, corrections and project progress. |
| **Your control** | Choose which materials belong to a project and inspect the originals. | View, edit, confirm or forget records; manage global and project memory separately. |

Memory consolidation follows the selected memory policy. It supports continuity while keeping the original research material available for review.

## Research capabilities and what they produce

<a href="assets/architecture/Fig3_Research_capabilities_en.png"><img src="assets/architecture/Fig3_Research_capabilities_en.png" alt="Six connected research workflows: bilingual literature reading, deep research and literature tracking, data analysis, experimental records, GeneCode molecular design, and manuscript citation checks." width="1400" /></a>

| Capability | Work in BioSeeki | Outputs you can return to |
| --- | --- | --- |
| **Literature translation and reading** | Read the original PDF alongside translated passages, explain a figure and navigate back to the supporting source. | Translated text, reading notes and source locations. |
| **Deep research** | Define a question, retrieve relevant public literature and project material, compare evidence and organize a synthesis. | Evidence tables, literature lists and research reports. |
| **Literature radar** | Follow a project topic and review relevant new publications through daily and weekly digests. | Paper updates, digests and retrieval status. |
| **Data analysis and figures** | Inspect sample groups and data structure, run analysis with Python/R tools, and revise plots and parameters. | Results tables, figures, scripts and execution records. |
| **Experimental records** | Organize aims, samples, reagents, procedures, observations and attachments; preview records and export documents. | Editable records, attachments, Word and PDF exports. |
| **GeneCode molecular design** | Inspect sequences, plasmid maps, features, translation, restriction sites and alignments; develop cloning and primer designs. | Editable sequences, candidate primers, quality-control results and edit proposals. |
| **Manuscripts and citations** | Develop a manuscript from project material and check how claims connect to sources, DOI records, versions and retraction status. | Drafts, source-linked claims and citation-check reports. |
| **Presentations and reports** | Turn papers, results and figures into a structured research report or lab-meeting presentation. | Editable slides, speaker notes and references. |

The figures are architecture and workflow schematics, not experimental results or performance benchmarks. The exact analysis depends on the supplied material, research design and available tools.

## One project, several connected steps

For example, a fluorescent-protein project can stay in the same workspace as you:

1. Add the relevant papers and existing experimental records to the project knowledge base.
2. Read a paper in the original language and translation, then compare its evidence with other sources.
3. Open the vector and insert in **GeneCode**, inspect the proposed design and confirm intended edits.
4. Analyze the resulting data, retain scripts and figures, and write up the experimental record.
5. Reuse the project context for a manuscript or presentation, and follow new literature with the radar.

You can also start with just one task. BioSeeki does not require following a fixed workflow.

## Local workspace, connected services

| On your computer | Connected when needed |
| --- | --- |
| Project files and generated outputs. | BioSeeki account and model services. |
| Knowledge index and managed memory. | Selected task-relevant context sent for model reasoning. |
| Local file tools, analysis runtimes and the GeneCode workspace. | Literature search and scientific databases. |

BioSeeki is a desktop application; model-assisted tasks and online search require a network connection. See the [privacy policy](https://bioseeki.com/privacy) for data-handling details.

## Download and get started

**[Download BioSeeki from the official website →](https://bioseeki.com/download)**

| Platform | Public availability |
| --- | --- |
| **macOS** | **Beta 0.1.7**, Apple silicon (M series), macOS 14 or later. |
| Windows / Intel Mac | Public downloads are not available yet. |

1. Download and open the DMG, then double-click **BioSeeki Beta**.
2. Choose **Install to Applications**. The installed app opens automatically. Dragging it into **Applications** also works.
3. Sign in or create a BioSeeki account. Select a project folder, add your material and describe the result you need.

The Mac Beta is signed and Apple-notarized. Current installation details and SHA-256 checksums are on the [download page](https://bioseeki.com/download). Before updating, save your work and quit the previous version.

**[Getting started](docs/getting-started.md)** · **[中文使用指南](docs/getting-started.zh-CN.md)** · **[Functional updates](CHANGELOG.md)**

## Try a concrete question

> **Literature:** Open this PDF for side-by-side reading. Explain Figure 2 and locate the passages supporting its conclusion.

> **Analysis:** Inspect these columns, missing values and sample groups first. Explain the analysis, then return the results, figures and scripts.

> **Experimental record:** Organize these notes and attachments into a dated experimental record, then preview it and export a PDF.

> **Molecular design:** Review this vector and insert. Check the junctions and reading frame, and show the proposal in GeneCode.

> **Writing:** Use these results for a 10-minute lab meeting, with editable slides, speaker notes and source references.

## Feedback and community

- [Report a bug](https://github.com/zjuphD/BioSeeki/issues/new?template=bug_report.yml) or [suggest a feature](https://github.com/zjuphD/BioSeeki/issues/new?template=feature_request.yml).
- [Join Discussions](https://github.com/zjuphD/BioSeeki/discussions) to share questions and research workflows.
- For account, billing or private support: [support@bioseeki.com](mailto:support@bioseeki.com).

Use anonymized examples in public issues. For vulnerabilities, see the [security contact](SECURITY.md).

**Star this repository** to help other researchers discover BioSeeki, or share the [website](https://bioseeki.com/) with your lab.

---

[Website](https://bioseeki.com/) · [Download](https://bioseeki.com/download) · [Changelog](https://bioseeki.com/changelog) · [Privacy](https://bioseeki.com/privacy) · [Terms](https://bioseeki.com/terms) · [Repository notice](NOTICE.md)
