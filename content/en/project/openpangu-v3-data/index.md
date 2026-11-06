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
- **Distributed GitHub processing**: use Data-Juicer for files / commits / PRs, with Kubernetes (K8s) orchestrating parallel processing across **40,000 CPU cores**. Separate sample-wise cleaning from aggregation. Combine commit-SHA and content hashes with MinHashLSH and semantic deduplication; reuse syntax-validation signals for scoring, then apply quality/language sampling, packing, decontamination and loss masks.
