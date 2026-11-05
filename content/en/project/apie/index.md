---
{
  "title": "APIE / RSI Infra: LLM inference for recursive self-improvement",
  "date": "2026-06-01T00:00:00Z",
  "summary": "An independently developed inference framework with optimization skills, benchmarks, fused graphs, asynchronous speculation and Rust parallel tokenization.",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**June 2026–present · Independently developed**

- **Designed for RSI**: separate the stable runtime from model adaptations; give agents structured tool results, diagnostics, state capture/replay and layered numerical validation. Track hypotheses and evidence in issues, and validate changes through PR review and CI.
- **Fused graphs and asynchronous speculation**: execute target verification and draft generation in one graph; reuse fixed-address CPU/NPU buffers and update block tables incrementally to overlap device proposals with host scheduling.
- **Parallel tokenization**: implement LoPT with a bounded Rust pool and per-worker BPE caches. With DeepSeek-V4's tokenizer, 16 threads and a 21.8K-token input, measured latency fell from 13.51 ms to 9.79 ms.

[Source code](https://github.com/CAKE-math/APIE) · [LoPT paper](https://aclanthology.org/2026.acl-long.1529/)
