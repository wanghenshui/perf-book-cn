# 介绍 {#sec .sec1} 

[TODO]: 更新介绍。这是书中最重要的部分。:) 更新说明我们现在正处于一个新时代的开端。PC -> 移动 -> 云 -> AI?

常说，“性能为王”。十年前是真的，现在当然也是如此。根据[[@Domo2017](../References.md#Domo2017)]的数据，在2017年，全球每天创造了2.5个万亿[^1]字节的数据，如[[@Statista2018](../References.md#Statista2018)]所预测的那样，这个数字每年增长25%。在我们日益数据中心化的世界中，信息交换的增长推动了对更快软件（SW）和更快硬件（HW）的需求。可以说，数据增长不仅对计算能力提出了需求，还对存储和网络系统提出了需求。

在个人电脑时代[^2]，开发人员通常直接在操作系统之上进行编程，可能之间会有一些库。随着世界进入云时代，软件堆栈变得更加深奥和复杂。开发人员大多数时间都在工作的顶层堆栈已经远离了硬件。这些额外的层次抽象出实际的硬件，从而允许使用新型加速器来处理新兴工作负载。然而，这种演进的负面影响是，现代应用程序的开发人员对其软件运行的实际硬件的了解较少。

多亏了摩尔定律，软件程序员几十年来一直“轻松愉快”。过去，一些软件供应商更倾向于等待新一代硬件以加速其应用程序，而不是花费人力资源改进其代码。从图@fig:50YearsProcessorTrend可以看出，单线程性能增长正在放缓。单线程性能是指在隔离环境中测量时CPU核心内的单个硬件线程的性能。

![50 Years of Microprocessor Trend Data. *© Image by K. Rupp via karlrupp.net*](https://raw.githubusercontent.com/dendibakh/perf-book/main/img/intro/50-years-processor-trend.png){#fig:50YearsProcessorTrend width=90%}

当不再每个硬件世代都能提供显著的性能提升[[@Leisersoneaam9744](../References.md#Leisersoneaam9744)]时，我们必须开始更加关注代码运行的速度。在寻求提高性能的方法时，开发人员不应依赖硬件。相反，他们应该开始优化其应用程序的代码。

> “当今软件非常低效；现在是软件程序员再次变得擅长优化的黄金时代。”- 美国企业家和投资者马克·安德森（Marc Andreessen），摘自a16z Podcast，2020年

\personal{在英特尔工作期间，我时常听到同样的故事：当英特尔的客户在其应用程序中遇到慢速时，他们会立即无意识地开始责怪英特尔的CPU速度慢。但是当英特尔派遣我们的性能高手与他们合作并帮助他们改进应用程序时，往往会将其加速2倍，有时甚至是10倍。}

达到高水平的性能具有挑战性，并且通常需要大量的努力，但希望这本书能给你提供帮助的工具。

[^1]: 万亿是千的六次方（10^18^）。

[^2]: 从1990年代末到2000年代末，个人电脑占据了计算设备市场的主导地位。