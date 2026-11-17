---
title: "SGLang 术语表"
---

# SGLang 术语表

| 术语 | 英文 / 缩写 | 含义 |
|---|---|---|
| 大语言模型 | LLM | 基于大规模文本训练、通过概率分布生成 token 的模型。 |
| 推理 | Inference | 使用固定模型权重完成前向和生成，不更新参数。 |
| 预填充 | Prefill | 对整段 Prompt 计算表示并建立初始 KV Cache 的阶段。 |
| 解码 | Decode | 逐 token 生成并增量读写 KV Cache 的阶段。 |
| KV 缓存 | KV Cache | 保存各层历史 Key/Value，避免生成时重复计算历史投影。 |
| 计算受限 | Compute-Bound | 主要受算力限制，增加数据搬运效率未必能解决瓶颈。 |
| 访存受限 | Memory-Bound | 主要受权重、KV 或中间数据的带宽和搬运限制。 |
| 算术强度 | Arithmetic Intensity | 计算量与数据搬运量之比，用于 Roofline 分析。 |
| 屋顶线模型 | Roofline Model | 根据硬件算力、带宽与任务算术强度判断性能上限和瓶颈。 |
| 首 Token 时延 | TTFT | 请求到达到首个输出 token 可用的时间。 |
| 每输出 Token 时间 | TPOT | 首个 token 后平均每个输出 token 的时间。 |
| Token 间时延 | ITL | 相邻输出 token 到达时间的间隔。 |
| 端到端时延 | E2E Latency | 从请求提交到完整响应结束的时间。 |
| 有效吞吐 | Goodput | 满足指定延迟或服务等级目标的有效请求吞吐。 |
| 连续批处理 | Continuous Batching | 按迭代动态增删请求，减少固定批次等待。 |
| 分页 KV 缓存 | Paged KV Cache | 用固定大小物理块和 Block Table 管理非连续缓存。 |
| 前缀缓存 | Prefix Caching | 复用请求之间相同前缀对应的 KV。 |
| RadixAttention | RadixAttention | 使用 Radix Tree 组织 token 前缀与缓存映射，实现最长前缀复用。 |
| 调度器 | Scheduler | 决定每轮接收、运行、暂停或完成哪些请求，并管理资源预算。 |
| 张量并行 | TP | 将层内权重和计算分片到多设备，并通过集合通信组合。 |
| 数据并行注意力 | DP Attention | 在多个数据并行工作副本间分配注意力相关请求或计算。 |
| 专家并行 | EP | 将 MoE 专家分布到不同设备，通过路由和通信处理 token。 |
| 流水线并行 | PP | 将模型层分段放到不同设备，通过微批次流水执行。 |
| 投机解码 | Speculative Decoding | 草稿模型提出候选，目标模型验证并按规则接受、纠正或重采样。 |
| 注意力后端 | Attention Backend | 负责不同布局和阶段的注意力计算，如 FlashInfer、Triton、FA3、FlashMLA。 |
| 量化 | Quantization | 用较低位宽表示权重、激活或 KV，降低存储和搬运成本并引入误差。 |
| 分层缓存 | Hierarchical Caching | 在 GPU、主机内存和外部存储之间迁移不同热度的缓存。 |
| PD 分离 | Prefill-Decode Disaggregation | 将 Prefill 与 Decode 部署到独立资源池，并传输 KV Cache。 |
| 性能分析 | Profiling | 采集 CPU、GPU、通信和内存事件，定位时间或资源消耗。 |
| 跟踪 | Trace | 按时间顺序记录事件及依赖，用于分析排队、重叠和空闲区间。 |
| 持续集成 | CI | 对提交自动执行构建、测试和检查，作为 PR 质量门禁。 |
| 拉取请求 | PR | 向原项目提交修改并接受 CI 与代码评审的协作流程。 |
