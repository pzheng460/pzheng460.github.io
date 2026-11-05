---
{
  "title": "DeepSeek-V3：昇腾推理性能优化",
  "date": "2025-02-01T00:00:00Z",
  "summary": "深度参与 LoPT 无损并行 Tokenizer、FlashComm 1/2/3 通信与多流适配，成果发表于 ACL 2026 主会。",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**2025.02—2025.08 · 深度参与**

- **LoPT**：在 vllm-ascend（ascend-vllm/omni-infer）实现重叠分块、字符位置匹配与动态扩块。DeepSeek-V3 Tokenizer、LongBenchV2、32 进程配置下，耗时由 622.4 ms 降至 108.2 ms，与串行输出完全一致。
- **FlashComm 1/2/3**：适配通信间计算重排、低维 All2All、权重冗余及多流重叠。并发 8、输入 2K 下，FlashComm 1/2 将 Prefill 从 951 ms 降至 699/631 ms；FlashComm3 在高并发下提升 Decode 吞吐 25%–30%，共享专家 TP8 方案节省单机约 2.08 GB 内存。各指标来自对应方案的独立基准。

[LoPT · ACL 2026](https://aclanthology.org/2026.acl-long.1529/)
