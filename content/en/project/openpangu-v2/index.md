---
{
  "title": "openPangu-v2: pretraining architecture selection and MTP inference optimization",
  "date": "2025-08-01T00:00:00Z",
  "summary": "Core contributions to three-head MTP selection, 2048-token sliding windows and full-graph speculative execution for long contexts.",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**August 2025–June 2026 · Core contributor**

- **Architecture selection**: analyze acceptance and trade-offs for three-head MTP with a 2048-token sliding window. Multi-token drafts improve bandwidth-bound decoding, while local attention bounds draft compute and KV-cache costs. Build rapid validation tools for pilot experiments.
- **Full-graph execution**: implement missing multi-MTP calls, dynamic TND boundaries and draft padding so decode inputs as small as 1–3 tokens stay in the static graph under P/D disaggregation.
- **System outcomes**: at 128K input / 1K output and concurrency 1 on a co-located A3 node, Flash / Pro achieve 5.63 / 9.55 ms TPOT. With disaggregated P/D, Pro reaches 1,326 tokens/s/NPU at 18.1 ms TPOT (128K/8K, batch 24 per NPU). These figures cover the combined system optimizations.

[Model and technical report](https://huggingface.co/openpangu/openPangu-2.0-Pro)
