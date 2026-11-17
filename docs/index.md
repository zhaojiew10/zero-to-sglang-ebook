---
title: "Zero to SGLang 推理引擎教程"
---

# Zero to SGLang 推理引擎教程

![Zero to SGLang 官方课程封面：从推理本质出发，构建 mini-sglang，再阅读真实 SGLang 源码并参与开源贡献](resources/repo/zero_to_sglang.png)

*封面：Datawhale × RadixArk《zero-to-sglang》官方课程。（原课程官方仓库图片）*

基于 **Datawhale × RadixArk** 的 zero-to-sglang 原课程重组，结合概念文档、代码走读和全 23 讲视频，形成 **4 个部分、23 章**的连续中文阅读版。本书从推理的基本问题出发，逐步构建 mini-sglang，再进入真实 SGLang 的进阶技术、性能分析和开源协作。

[开始阅读：第 1 章](chapters/ch01.md){ .md-button .md-button--primary }  [阅读与实践指南](guide.md){ .md-button }  [术语表](glossary.md){ .md-button }  [来源与许可](sources.md){ .md-button }

!!! note "独立阅读版"
    本书保留原课程署名和 CC BY-NC-SA 4.0 许可，进行了章节重组、书面化整理和视频帧策展。它不是新的官方版本；原课程内容以 [zero-to-sglang 官方站点](https://datawhalechina.github.io/zero-to-sglang/)为准。

## 推荐阅读路径

- **系统学习**：按第 1 → 23 章顺序阅读，先概念、后构建、再进阶和贡献。
- **只做基础入门**：阅读第 1—5 章，无需先准备 GPU。
- **专注引擎实现**：从第 6 章进入 mini-sglang，完成第 7—15 章的递进改造。
- **关注生产级优化**：阅读第 16—22 章，结合真实 SGLang 和 Profiling 方法。
- **准备参与开源**：先读第 22 章的证据链，再学习第 23 章 PR 工作流。

## 全书目录

### 第一部分 · 推理基础（第 1—5 章）

建立从 Transformer 到推理系统的共同语言：阶段划分、GPU 瓶颈、KV Cache 和可复现 Benchmark。

[本部分导读](parts/part01.md)

- [第 1 章 LLM 入门](chapters/ch01.md)
- [第 2 章 推理入门](chapters/ch02.md)
- [第 3 章 GPU 入门](chapters/ch03.md)
- [第 4 章 KV Cache：推理的核心数据结构](chapters/ch04.md)
- [第 5 章 Benchmark：指标与实验方法](chapters/ch05.md)

### 第二部分 · 构建 mini-sglang（第 6—15 章）

从一个请求的生命周期出发，逐次加入前向生成、缓存、网络服务、调度、分页、前缀复用、多进程和投机解码。

[本部分导读](parts/part02.md)

- [第 6 章 mini-sglang：推理引擎长什么样](chapters/ch06.md)
- [第 7 章 一个请求的旅程](chapters/ch07.md)
- [第 8 章 前向与生成](chapters/ch08.md)
- [第 9 章 KV Cache 优化](chapters/ch09.md)
- [第 10 章 HTTP 服务与并发请求](chapters/ch10.md)
- [第 11 章 Continuous Batching 与调度](chapters/ch11.md)
- [第 12 章 Paged KV Cache 与显存管理](chapters/ch12.md)
- [第 13 章 RadixAttention 与前缀缓存](chapters/ch13.md)
- [第 14 章 多进程与张量并行](chapters/ch14.md)
- [第 15 章 投机解码](chapters/ch15.md)

### 第三部分 · 进阶推理技术（第 16—20 章）

从“能实现”进入“如何选择”：比较注意力后端、低精度、分层缓存、并行策略和 Prefill-Decode 分离的适用条件。

[本部分导读](parts/part03.md)

- [第 16 章 注意力后端](chapters/ch16.md)
- [第 17 章 量化与低精度推理](chapters/ch17.md)
- [第 18 章 分层缓存](chapters/ch18.md)
- [第 19 章 横向扩展：DP Attention、EP、PP](chapters/ch19.md)
- [第 20 章 Prefill-Decode 分离](chapters/ch20.md)

### 第四部分 · 部署、分析与开源贡献（第 21—23 章）

把模型服务跑起来，用 Trace 解释时间花在哪里，再将可复现的问题和验证充分的修改带入 PR 流程。

[本部分导读](parts/part04.md)

- [第 21 章 用 Cookbook 部署 SGLang](chapters/ch21.md)
- [第 22 章 Profiling 与 Trace 分析](chapters/ch22.md)
- [第 23 章 SGLang PR 工作流](chapters/ch23.md)

## 配套页面

- [阅读与实践指南](guide.md)：先修知识、环境、实验和校对原则。
- [SGLang 术语表](glossary.md)：统一常见术语和中英文表达。
- [资料来源、许可与版本](sources.md)：原课程署名、许可、源码快照和素材出处。
