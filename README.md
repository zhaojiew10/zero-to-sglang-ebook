# Zero to SGLang 推理引擎教程

这是基于 **Datawhale × RadixArk** 的 [zero-to-sglang](https://github.com/datawhalechina/zero-to-sglang) 原课程重组的独立阅读版，采用与长篇源码教程一致的组织方式：**4 个部分、23 章**，与全 23 讲视频对应，同时结合原课程的概念文档和代码走读。它不是新的官方版本，也不替代原项目。

## 阅读入口

- [电子书首页](docs/index.md)
- [阅读与实践指南](docs/guide.md)
- [第 1 章：LLM 入门](docs/chapters/ch01.md)
- [SGLang 术语表](docs/glossary.md)

## 内容结构

1. **推理基础**：LLM、Prefill/Decode、GPU、KV Cache 和 Benchmark。
2. **构建 mini-sglang**：请求流程、前向生成、HTTP、连续批处理、分页缓存、RadixAttention、TP 和投机解码。
3. **进阶推理技术**：注意力后端、量化、分层缓存、横向扩展和 PD 分离。
4. **部署、分析与贡献**：Cookbook、Profiling、Trace 和 PR 工作流。

## 来源和许可

本书基于原课程内容重组，原课程采用 **CC BY-NC-SA 4.0**。本阅读版按相同许可证提供，保留 Datawhale × RadixArk 署名、原文件链接和改动说明，仅用于非商业学习与分享。

视频帧来自 Datawhale 官方课程视频，相关权利归原作者和课程方所有。详细来源与版本说明见 `docs/sources.md`。公开分发前请核对原课程的最新授权条款。
