---
{
  "title": "DeepSeek-V3: inference performance on Ascend",
  "date": "2025-02-01T00:00:00Z",
  "summary": "Core work on lossless parallel tokenization and FlashComm communication/stream adaptation, with LoPT published at ACL 2026.",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**February–August 2025 · Core contributor**

- **LoPT**: implement overlap splitting, character-position matching and dynamic chunk expansion in vllm-ascend (ascend-vllm/omni-infer). DeepSeek-V3 tokenizer latency falls from 622.4 ms to 108.2 ms on LongBenchV2 with 32 processes, with token IDs identical to serial output.
- **FlashComm 1/2/3**: adapt computation reordering, low-dimensional All2All, weight redundancy and multi-stream overlap. At concurrency 8 and input 2K, FlashComm 1/2 reduce prefill from 951 ms to 699/631 ms. FlashComm3 improves high-concurrency decode throughput by 25%–30%; its shared-expert TP8 configuration saves about 2.08 GB per node. These are separate scheme-specific benchmarks.

[LoPT · ACL 2026](https://aclanthology.org/2026.acl-long.1529/)
