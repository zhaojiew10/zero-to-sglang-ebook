---
title: "资料来源、许可与版本"
---

# 资料来源、许可与版本

## 原课程与源码快照

本书是基于官方课程整理的独立阅读版，不是 Datawhale 或 SGLang 官方新发布的电子书。

- 原项目：[datawhalechina/zero-to-sglang](https://github.com/datawhalechina/zero-to-sglang)
- 原课程作者与组织：**Datawhale × RadixArk**
- 参考 commit：[`296fec5d215408f918c0e4007e71c962e804ef7e`](https://github.com/datawhalechina/zero-to-sglang/commit/296fec5d215408f918c0e4007e71c962e804ef7e)
- Commit 日期：2026-11-16
- 原在线文档：[https://datawhalechina.github.io/zero-to-sglang/](https://datawhalechina.github.io/zero-to-sglang/)
- mini-sglang 参考实现：[sgl-project/mini-sglang](https://github.com/sgl-project/mini-sglang)
- SGLang：[sgl-project/sglang](https://github.com/sgl-project/sglang)

## 改编方式与许可

原课程采用 [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)（CC BY-NC-SA 4.0）。

本书按相同许可证提供，主要改动包括：

- 将概念文档与代码走读合并为连续的 23 章阅读路径；
- 按“概念—机制—边界—验证”重组部分文字；
- 增加章内小结、实践检查和统一导航；
- 从对应课程视频中选择教学帧并添加解释性图注；
- 统一术语、公式和相关参考链接。

再分发或继续改编时，应保留原课程署名、许可链接和改动说明，并遵守非商业与相同方式共享要求。

## 视频与图片

- 视频：[【全23讲】从零手搓SGLang推理引擎：调度/KV Cache/量化/PD分离/开源PR全流程](https://www.bilibili.com/video/BV1Y7Wd6rEhp/)
- BV 号：`BV1Y7Wd6rEhp`，共 23 个分 P，与本书第 1—23 章对应。
- 视频封面及课程标识：zero-to-sglang 官方仓库 `course-material/eng/images/zero_to_sglang.png`。
- 正文图注标明视频帧对应的课程章节和来源。

视频、课件封面和相关素材的权利归其权利人所有，公开分发时应同时遵守原课程与视频素材的授权要求。

## 验证口径

本书各章中的官方命令和案例用于读者复现，未在本机执行时会明确标注。原 PR 的案例数据属于原作者和原课程，不列为本书实测结果；静态阅读也不能代替服务部署、模型生成、分布式实验或 Profiling 验证。
