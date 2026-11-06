---
{
  "title": "openPangu-v3: agent-assisted distributed pretraining data pipelines",
  "date": "2026-08-01T00:00:00Z",
  "summary": "Independently build arXiv parsing and Data-Juicer/Kubernetes-based GitHub processing across 40,000 CPU cores, combining distributed deduplication with human–agent error-driven iteration.",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**August 2026–present · Independently developed**

- **arXiv pretraining data**: implement main-document discovery, dependency expansion, macro normalization, equation preservation/restoration and figure/reference rewriting; bound long-tail costs with PDF fallback and timeout handling.
- **Human–agent improvement loop**: label parser errors daily, periodically collect failure cases with an agent, and use them to iterate on long-tail templates, equations and figures.
- **Distributed GitHub processing**: use Data-Juicer with sharded data parallelism and separate map and aggregation stages. Compute content fingerprints and MinHash signatures in parallel, and use LSH candidate retrieval to reduce near-duplicate comparisons. Combine bucket-weighted sampling with greedy sequence packing. Run across **40,000 CPU cores** on Kubernetes (K8s), processing approximately **306 million repositories** and producing approximately **2.3 trillion tokens** of pretraining data.
