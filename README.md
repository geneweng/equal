# 等号何以拥有不成比例的力量

**The Disproportionate Power of the Equal Sign**

这是一本关于数学符号 `=` 的书稿仓库 —— 追问一个最简洁的符号如何以其"枢纽"地位，承担起组织现代数学知识的核心接口功能。

本仓库同时包含：

- [`equal_sign_book.pdf`](equal_sign_book.pdf) —— 当前版本的书稿 PDF
- [`manuscript_pdf.md`](manuscript_pdf.md) —— 书稿的 Markdown 源文件（用于生成 PDF）

## 内容结构

全书围绕"**压缩与接口**"这一统一视角展开，分为三个层次（历史层、结构层、当代层），共十一章，另有导论与结语。

- 导论：等号何以拥有不成比例的力量
- 第一章　没有等号的数学——前现代"相等"观念的表达方式
- 第二章　1557——雷科德与等号的发明
- 第三章　从发明到通用——等号在近代欧洲的扩散
- 第四章　等号与代数革命——从修辞到操作
- 第五章　等号与解析几何——图形如何变成方程
- 第六章　等号与现代科学语言——从公式到定律
- 第七章　等号的多重语义——相等、恒等、定义、赋值
- 第八章　数学为什么能够被压缩
- 第九章　等号作为局部压缩器——数学表征的最小机器
- 第十章　机器如何理解"相等"
- 第十一章　等号之后——新的问题与哲学的回声
- 结语：在两条横线之间
- 术语表（Glossary）
- 参考文献（Bibliography）

## 阅读方式

最简单的方式是直接下载 [`equal_sign_book.pdf`](equal_sign_book.pdf) 阅读。

如需查看或编辑原始文本，请打开 [`manuscript_pdf.md`](manuscript_pdf.md)。Markdown 中包含 LaTeX 数学公式（形如 `$F = ma$`），在任何支持 MathJax/KaTeX 的渲染器中都可以正确显示。

## 从 Markdown 构建 PDF

本书的 PDF 由 Markdown 源文件经由 Pandoc + XeLaTeX 生成。假设已安装 [Pandoc](https://pandoc.org/) 与 TeX Live（含中文字体支持），可运行：

```bash
pandoc manuscript_pdf.md \
  -o equal_sign_book.pdf \
  --pdf-engine=xelatex \
  -V CJKmainfont="Songti SC" \
  -V geometry:margin=1in
```

具体命令可根据本地字体与排版偏好调整。

## 反馈与贡献

- **内容问题**（错字、事实性错误、引用不准确、论证瑕疵等）：欢迎在 [Issues](../../issues) 中提出，并尽量指明章节与段落位置。
- **修改建议**：可以通过 Pull Request 提交。请从 `main` 开一个新分支，提交修改后向 `main` 发起 PR。

## 引用

如需在学术写作中引用本书，暂请使用如下格式：

```
Weng, G. (2026). 等号何以拥有不成比例的力量 [The Disproportionate Power of the Equal Sign]. 
Manuscript. https://github.com/geneweng/equal
```

## 许可

书稿内容版权归作者所有。未经书面许可，请勿以任何形式复制、分发或用于商业用途。代码片段（如有）以 MIT 协议发布。
