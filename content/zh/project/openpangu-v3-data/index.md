---
{
  "title": "openPangu-v3：Data Claw Dev 平台 Agent 自动化数据处理管线",
  "date": "2026-08-01T00:00:00Z",
  "summary": "独立建设 arXiv 论文解析和基于 Data-Juicer / Kubernetes 的 4 万 CPU 核规模 GitHub 分布式处理管线，以 Agent 与人工错误标注循环改进解析质量。",
  "tags": [
    "AI Infra"
  ],
  "featured": false
}
---

**2026.08—至今 · 独立开发**

- **arXiv 论文预训练数据**：针对模板兼容、公式保真与长尾耗时，实现主文档定位、依赖展开、宏规范化、公式占位/恢复和图文引用重写；以 PDF 回退和超时分流控制单篇处理开销。
- **循环式开发**：Agent 与人工每日标注解析错误，由 Agent 定时归集样本并改进解析逻辑，持续覆盖长尾模板及公式、图表问题。
- **GitHub 大规模分布式处理**：基于 Data-Juicer 采用分片数据并行，并行计算内容指纹和 MinHash 签名，通过 LSH 候选检索降低近重复比较开销；结合分桶加权采样与贪心打包，在 Kubernetes（K8s）上以 **4 万 CPU 核并行**完成约 **3.06 亿个仓库**处理，产出约 **2.3 万亿 Token** 预训练数据。
