# 前言 

## 关于作者 

Denis Bakhvalov是Intel的高级开发人员，负责C++编译器项目，旨在为各种不同架构生成优化代码。性能工程和编译器始终是他主要关注的领域之一。Denis于2008年开始作为软件开发人员的职业生涯，并在多个领域工作，包括开发桌面应用程序、嵌入式系统、性能分析和编译器开发。2016年，Denis开始了他的easyperf.net博客，专注于性能分析和调优、C/C++编译器以及CPU微体系结构。Denis是积极生活方式的支持者，在业余时间喜欢踢足球、打网球、跑步和下棋。此外，Denis还是两个美丽女儿的父亲。

联系方式：

- 电子邮件：dendibakh@gmail.com
- Twitter：[\@dendibakh](https://twitter.com/dendibakh)
- LinkedIn：[\@dendibakh](https://www.linkedin.com/in/dendibakh/)

## 作者的话 

我开始撰写这本书的初衷很简单：教育软件开发人员更好地理解其应用程序在现代硬件上的性能。我知道这对于初学者甚至有经验的开发人员来说可能是一个令人困惑的话题。这种困惑主要发生在没有先前处理性能相关任务的开发人员身上。这没关系，因为每个专家都曾经是初学者。

我记得我开始进行性能分析的日子。我盯着陌生的度量标准，试图匹配不符合的数据。我感到困惑。直到最后一切“豁然开朗”，所有的拼图才拼在一起。那时候，唯一的良好信息来源是软件开发人员手册，而这并不是主流开发人员喜欢阅读的。因此，我决定写这本书，希望能让开发人员更容易学习性能分析的概念。

认为自己在性能分析方面是初学者的开发人员可以从本书的开头开始顺序阅读，逐章阅读。第2至4章为开发人员提供了后续章节所需的最低知识集。已经熟悉这些概念的读者可以选择跳过这些章节。此外，本书还可以用作优化软件应用程序的参考或检查清单。开发人员可以将第7至11章作为调整其代码思路的来源。

## 目标受众 

本书将主要对那些从事性能关键应用程序和进行低级优化的软件开发人员有用。仅举几个领域：高性能计算（HPC）、游戏开发、数据中心应用程序（如Facebook、Google等）、高频交易。但是，本书的范围并不仅限于上述行业。任何想更好地了解其应用程序性能并知道如何进行诊断和改进的开发人员都会从中受益。作者希望本书所呈现的材料能帮助读者培养新的技能，可以应用于他们的日常工作中。

读者预期具备C/C++编程语言的最低背景，以理解本书的示例。能够阅读基本的x86汇编语言是理想的，但不是严格要求。作者还期望读者熟悉计算机体系结构和操作系统的基本概念，如中央处理器、内存、进程、线程、虚拟和物理内存、上下文切换等。如果上述术语中有任何新的术语，建议先学习这些材料。
