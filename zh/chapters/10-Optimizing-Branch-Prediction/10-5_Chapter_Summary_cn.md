---
typora-root-url: ..\..\img
---

## 章节总结 {.unlisted .unnumbered}

* 现代处理器在预测分支结果方面非常出色。因此，我们建议只有当 TMA 报告显示高 `Bad Speculation` 指标时才开始修复分支预测错误的工作。
* 当分支结果模式变得难以让 CPU 分支预测器跟踪时，应用程序的性能可能会受到影响。在这种情况下，无分支版本的算法可能表现更好。本章展示了如何用查找表、算术和谓词替换分支。在某些情况下，还可以使用编译器内联函数消除分支，如 [[@IntelAvoidingBrMisp](../References.md#IntelAvoidingBrMisp)] 所示。
* 无分支算法并不是普遍有利的。始终测量以找出最适合您特定情况的方法。

\sectionbreak