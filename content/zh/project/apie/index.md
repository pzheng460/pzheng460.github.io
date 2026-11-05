---
{
  "title": "APIE / RSI Infra：RSI 大模型推理框架与 Agent 自动化优化",
  "date": "2026-06-01T00:00:00Z",
  "summary": "独立开发面向 RSI 的推理框架、优化 Skill 与 Benchmark，结合融合图、异步投机流水和 Rust 并行 Tokenizer，构建 Agent 可定位、验证和迭代的系统。",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**2026.06—至今 · 独立开发**

- **AI Native 与 RSI**：分离稳定运行时和模型适配代码，提供 Agent 可调用的工具接口、结构化结果和诊断信息；通过状态采集/回放、分层精度验证与源码/环境追踪支撑迭代，以 Issue 记录假设和证据，以 PR 审查和 CI 验证约束合入。
- **融合图与异步投机流水**：将 target 验证与 draft 生成融合为同一张执行图；复用固定地址 CPU/NPU 缓冲区，增量更新 block-table，使设备侧草稿生成与主机调度和输入准备重叠。
- **并行 Tokenizer**：Rust 有界线程池实现 LoPT，各 worker 使用独立 BPE cache。DeepSeek-V4 Tokenizer、16 线程、21.8K-token 输入下，耗时由 13.51 ms 降至 9.79 ms。

[源代码](https://github.com/CAKE-math/APIE) · [LoPT 论文](https://aclanthology.org/2026.acl-long.1529/)
