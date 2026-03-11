# YCode.Designer.Fluxo

YCode.Designer.Fluxo 是一个面向 WPF 的可视化设计器实验项目，主要围绕节点拖拽、流程编辑、视口控制、连线绘制等图形化交互能力展开。

Pages: [https://ycode-lin.github.io/YCode.Designer.Fluxo/](https://ycode-lin.github.io/YCode.Designer.Fluxo/)

## 项目简介

这个仓库的目标，不只是做出一个“能显示出来”的界面，而是尽量把可视化编辑器里真正影响使用体验的部分做清楚，例如：

- 节点拖拽与交互反馈
- 设计面板的缩放、平移与视口管理
- 连线绘制与不同线型策略
- 面向 MVVM 的控件化组织方式

如果你正在实现 WPF 中的流程设计器、节点编辑器、图形化编排界面，或者只是想研究这类控件应该如何拆分与组织，这个仓库可以作为一个持续演进中的参考样本。

## 当前分支正在做什么

当前 `master` 分支的重点，是把 `YCodeFlowUI` 从更偏 Canvas 的实现方式，逐步整理为更清晰、更接近纯控件化、也更方便结合 MVVM 的结构。

这次重构并不是为了证明旧方案“不好”，而是一次认真回看与再实现的过程。我希望借这个过程继续学习图形化编辑控件的组织方式，也学习如何从其他优秀开源项目中吸收经验，例如 `Notify` 这样的项目。

## 分支说明

- `master`
  当前正在进行中的重构分支，重点是控件化与 MVVM 方向的整理。
- `CanvasDesigner`
  较早期的 Canvas 方案实现。这个分支已经能够满足当时的 MVVM 使用需求，也保留了不少值得参考的思路。

如果你想对比两种实现方式，建议一起阅读这两个分支。

## 仓库结构

- `YCode.Designer.Fluxo/`
  核心控件库代码。
- `YCode.Designer.Demo/`
  演示项目与试验入口。
- `docs/`
  GitHub Pages 静态页面文件。

## 相关链接

- GitHub Pages: [https://ycode-lin.github.io/YCode.Designer.Fluxo/](https://ycode-lin.github.io/YCode.Designer.Fluxo/)
- 旧方案分支: [CanvasDesigner](https://github.com/ycode-lin/YCode.Designer.Fluxo/tree/CanvasDesigner)
- 相关视频教程: [Bilibili 视频](https://www.bilibili.com/video/BV177421N76v/?share_source=copy_web&vd_source=09ea16918da424f6bed95ad4cd89fcf1)

## 致谢

这个仓库的很多思考，都来自开源社区已经公开分享出来的经验与方法。

尤其是在当前这轮重构里，我非常感谢像 `Notify` 这样具有开源精神的项目和作者。这里的“感谢”并不是一句客套话，而是真实地承认：很多时候，正是这些愿意公开实现、公开思路、公开取舍的人，让后来者能少走很多弯路。

同样，我也感谢所有愿意把时间投入开源的开发者。无论是完整项目、片段代码、文章、回答，还是一个微小但关键的思路，它们都会在另一个人的项目里继续产生价值。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=ycode-lin/YCode.Designer.Fluxo&type=Date)](https://star-history.com/#ycode-lin/YCode.Designer.Fluxo&Date)
