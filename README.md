# PKU 信科本科毕设模板 2025

## 仓库说明

本项目基于[该 Overleaf 模板](https://www.overleaf.com/latex/templates/pku-undergraduate-thesis-template-modified-from-pkuthss/pfrbvymbwbxk)进行修改，使其更符合信科教务在 2025 下发的本科毕设模板。本项目仅在 Overleaf 进行过测试，使用 XeLaTeX 编译器。

模板效果：[pkuthss_undergraduate_eecs_2025.pdf](./pkuthss_undergraduate_eecs_2025.pdf)

使用方式：在 [Overleaf 主页](https://www.overleaf.com/project)点击 New project -> Upload project，上传本项目的压缩包，在设置中切换为 XeLaTeX 编译器。

## 修改内容

- 整体：
    - 阻止文档自动添加空白页。
    - 取消 `newtxtext` 包的使用。该包会导致英文无法正常使用 `textbf` `textit` `textit` 等字体风格。
    - 删除对本科生无用的内容。
- 封面：
    - 将 `img/pku-fig-logo.png` 和 `img/pku-text-logo.png` 替换为同名 PDF 文件，以加速编译。
    - 无论中英文标题占据几行，其后都只有一条横线。
    - 英文标题加粗，使用三号字体。
    - date 字段去除空格，后三个字使用黑体。
- 导师评阅表：
    - 修改表项顺序和布局。
    - 表项内容居中对齐。
    - 给出完整使用示例。
- 中文摘要：
    - 去除页眉文本和页脚，保留页眉线。
- 英文摘要：
    - 去除作者名和导师名。
    - 标题字体大小使用三号。
    - 去除页眉文本、页眉线、页脚。
- 目录：
    - 去除页眉文本、页眉线、页脚。
    - 三级标题都使用五号字体（10.5pt）。
- 主要符号对照表：
    - 删除此页。
- 正文：
    - `chapter` 标题使用阿拉伯数字，三号字体，不居中；`section` 标题使用三号字体；`subsection` 标题使用四号字体。`subsection` 的标题缩进。
    - 仅正文第一页有页眉文本和页眉线，文本为中文论文名。这依赖于 [chap/chap0.tex](./chap/chap0.tex) 的第一行，修改/替换时注意保留。
    - 每页都有页脚，文本为“第 X 页”。
- 参考文献：
    - 标题取消居中。
    - 使用 `numeric-comp` 样式，参考文献按引用顺序排序，不显示 ISBN、DOI、URL 信息。
    - 去除页眉文本、页眉线、页脚。
- 其它成果：
    - 删除此页。
- 致谢：
    - 去除页眉文本、页眉线、页脚。
- 原创性声明和使用授权说明:
    - 调整格式和内容。
    - 给出完整使用示例。

## 许可证

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
