---
{
  "title": "openPangu-v2：先导选型与 MTP 推理优化",
  "date": "2025-08-01T00:00:00Z",
  "summary": "深度参与三头 MTP 与 2048 滑窗选型、多 MTP 层调用和全图推理，为长上下文提供高效的自投机解码路径。",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**2025.08—2026.06 · 深度参与**

- **MTP 架构选型**：开展接收率优化与理论分析，支撑三头 MTP 与 2048 滑窗落地，以多 token 草稿改善访存受限的解码效率，以局部注意力控制计算和 KV Cache 开销；开发快速验证工具支撑候选方案迭代。
- **Multi-MTP 全图推理**：补齐框架侧多 MTP 层调用，结合 TND 输入、动态序列边界与 draft padding，使 P/D 分离下单步输入仅 1–3 token 的请求仍走静态图。
- **支撑整网优化**：A3 单机、128K 输入/1K 输出、单并发下，Flash / Pro TPOT 为 5.63 / 9.55 ms；Pro 在 P/D 分离、128K 输入/8K 输出、每 NPU batch 24 下达到 1,326 tokens/s/NPU（TPOT 18.1 ms）。这些为整网联合优化结果。

[模型与技术报告](https://huggingface.co/openpangu/openPangu-2.0-Pro)
