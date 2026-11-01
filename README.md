# 物理竞赛一轮讲义

高中物理竞赛一轮讲义，当前主套包含12个专题、61讲、2400页、1152道题，配有3132幅可编辑TikZ图。仓库提供正式PDF、LaTeX源码、配图源码及相关整理资料。

## 阅读与下载

- [61讲逐讲目录与PDF](output/全套讲义目录.md)
- [下载整套PDF与TikZ源码](https://github.com/sabercldong/physics-olympiad-lectures/releases/latest/download/physics-olympiad-61-lectures-pdf-tikz.zip)
- [查看发布版本](https://github.com/sabercldong/physics-olympiad-lectures/releases)
- [全套核对记录](output/全套讲义核对.md)

| 专题 | 讲数 | PDF | 可编辑源码 |
| --- | ---: | --- | --- |
| 微积分 | 4 | [阅读](output/微积分/pdf) | [LaTeX与TikZ](output/微积分/latex) |
| 运动学 | 6 | [阅读](output/运动学/pdf) | [LaTeX与TikZ](output/运动学/latex) |
| 牛顿运动定律 | 4 | [阅读](output/牛顿运动定律/pdf) | [LaTeX与TikZ](output/牛顿运动定律/latex) |
| 静力学 | 5 | [阅读](output/静力学/pdf) | [LaTeX与TikZ](output/静力学/latex) |
| 能量与动量 | 6 | [阅读](output/能量与动量/pdf) | [LaTeX与TikZ](output/能量与动量/latex) |
| 振动与波 | 3 | [阅读](output/振动与波/pdf) | [LaTeX与TikZ](output/振动与波/latex) |
| 热学 | 4 | [阅读](output/热学/pdf) | [LaTeX与TikZ](output/热学/latex) |
| 静电 | 6 | [阅读](output/静电/pdf) | [LaTeX与TikZ](output/静电/latex) |
| 电路 | 6 | [阅读](output/电路/pdf) | [LaTeX与TikZ](output/电路/latex) |
| 静磁 | 4 | [阅读](output/静磁/pdf) | [LaTeX与TikZ](output/静磁/latex) |
| 电磁感应 | 6 | [阅读](output/电磁感应/pdf) | [LaTeX与TikZ](output/电磁感应/latex) |
| 光学与近代物理 | 7 | [阅读](output/光学与近代物理/pdf) | [LaTeX与TikZ](output/光学与近代物理/latex) |

每讲按知识正文、例题与分析、本讲小结、练习、练习解答组织。题设图与解答过程图使用TikZ绘制，并保留在源码中。

## 编译

使用包含中文字体与宏包的TeX Live或MacTeX，采用XeLaTeX。主要依赖包括ctex、Fandol字体、TikZ、PGFPlots、amsmath、hyperref等。

克隆后进入任意一讲的源码目录，例如：

```sh
git clone https://github.com/sabercldong/physics-olympiad-lectures.git
cd physics-olympiad-lectures/output/微积分/latex/01_极限与导数
latexmk -xelatex -interaction=nonstopmode -halt-on-error main.tex
```

也可以连续运行两次`xelatex main.tex`；交叉引用仍有变化时继续编译，直至引用稳定。保留同目录全部源码文件，各讲的`main.tex`会引用所需文件。公共排版规范见[讲义编写规范](output/讲义编写规范.md)和[统一样式](output/讲义统一样式.tex)。

## 目录说明

- `output/专题名/latex/`与`output/专题名/pdf/`：上表所列当前61讲源码及PDF。
- `output/运动学/课件/`：相关课件及素材。
- `output/天体运动/`与`output/微积分基础导论/`：补充资料，不计入上述61讲。
- `output/讲义审查/`与`output/讲义比较/`：历次审查、修改及核对记录。

较早的`output/latex/`、`output/pdf/`目录及试题整理规范中有尚未下载到本机的iCloud占位文件，本次未纳入仓库；上表所列当前61讲的PDF与源码完整提供。

## 审校范围

当前记录覆盖1152道题与719个知识单元的源码审查及相应修订，并完成全61讲编译。PDF采用重点页面渲染复核；主审单独查看了38讲的134个页面，未对全部2400页重新逐页目视检查。

记录见[审查说明](output/讲义审查/全套逐题审查与完善说明_20261101.md)和[重点页面记录](output/讲义审查/页面验收_主审_20261101.json)。编译与结构检查的通过不等同于逐式独立验算或全部页面精校。
