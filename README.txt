ClipAgent | COMP7608B Group 59 | Final report

Import this ZIP into Overleaf. Set main.tex as the main document and pdfLaTeX as the compiler. main.pdf is a compiled preview generated locally with Tectonic.

Figure 1: supplied system architecture, inserted in System design.
Figure 2: supplied editing workflow, inserted in System design.
The original raster images remain unchanged in figures/. Embedded headings are cropped by graphicx so LaTeX controls figure numbering. Architecture terminology corrections are editable LaTeX picture overlays: the per-call guard is three attempts total (including retries), rather than three retries; the SQLite contents label was cleaned up.

Added: architecture overview, workflow explanation, figure captions, cross-references, and supplied-image disclosure.
The report uses the official neurips_2026.sty.

The PDF was compiled and rendered for visual review.


Collaborative editing / 按章节协作
================================
main.tex is the only compilation entry point. Keep it selected as Main document in Overleaf. Global packages, title/author metadata, section order and appendix/page-break commands remain centralized there. Chapters are inserted with \input (not \include), so splitting files does not force new pages. Figures, tables, citations and cross-references remain globally numbered.

章节分工：
sections/00_abstract.tex                  摘要
sections/01_introduction.tex              引言
sections/02_system_design.tex             系统设计（含架构图和流程图）
sections/03_evaluation_protocol.tex       评估方法
sections/04_results.tex                   实验结果
sections/05_limitations_and_impacts.tex   局限与影响
sections/06_contributions_and_ai.tex      贡献与 AI 使用说明
sections/07_appendix_reproducibility.tex  附录与复现说明
sections/references.tex                   参考文献
figures/                                 插图原文件

协作方式：每位组员修改自己负责的章节文件。无需在章节里添加 \documentclass、\begin{document} 或 \end{document}，也不要直接编译单个章节。统一编译 main.tex 即可预览完整报告。图像路径仍相对于项目根目录。添加标签时沿用 sec:、fig:、tab: 前缀并保持唯一。

保留现有全局样式和图表设置（包括 Figure 2 的 88% 宽度）。源文件拆分不改正文内容。

最终报告加入五分钟合成电子表格补充案例。章节 3 说明实验设置，章节 4 列出五次尝试及其结果。原 24 次实验独立保留。提交代码包中的 evaluation/spreadsheet/ 目录提供素材、成片、任务记录和离线复核脚本。
