ClipAgent | COMP7608B Group 59 | Illustrated report

Import this ZIP into Overleaf. Set main.tex as the main document and pdfLaTeX as the compiler. main.pdf is a compiled preview generated locally with Tectonic.

Figure 1: supplied system architecture, inserted in System design.
Figure 2: supplied editing workflow, inserted in System design.
The original raster images remain unchanged in figures/. Embedded headings are cropped by graphicx so LaTeX controls figure numbering. Architecture terminology corrections are editable LaTeX picture overlays: the per-call guard is three attempts total (including retries), rather than three retries; the SQLite contents label was cleaned up.

Added: architecture overview, workflow explanation, figure captions, cross-references, and supplied-image disclosure.
Preserved: all experimental tables, reported results, original checklist, and official neurips_2026.sty.

Verified: successful compilation, no overfull boxes or unresolved references, complete PDF rendering for visual review, and byte-for-byte preservation of checklist and style files.


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
checklist.tex                            NeurIPS 检查清单
figures/                                 插图原文件

协作方式：每位组员修改自己负责的章节文件。无需在章节里添加 \documentclass、\begin{document} 或 \end{document}，也不要直接编译单个章节。统一编译 main.tex 即可预览完整报告。图像路径仍相对于项目根目录。添加标签时沿用 sec:、fig:、tab: 前缀并保持唯一。

保留现有全局样式和图表设置（包括 Figure 2 的 88% 宽度）。源文件拆分不改正文内容。

拆分验证：全文 13 页；逐页文字一致，1.5 倍渲染后的像素也完全一致。原 PDF 文件保持不变。
