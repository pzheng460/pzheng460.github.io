---
{
  "title": "",
  "type": "landing",
  "sections": [
    {
      "block": "about.biography",
      "id": "about",
      "content": {
        "title": "关于我",
        "username": "admin"
      }
    },
    {
      "block": "experience",
      "id": "experience",
      "content": {
        "title": "工作经历",
        "date_format": "2006.01",
        "items": [
          {
            "title": "AI Infra 算法研究员",
            "company": "华为技术有限公司 · 2012 实验室",
            "company_url": "https://www.huawei.com/",
            "location": "上海",
            "date_start": "2025-02-01",
            "date_end": "",
            "description": "理论研究部 · 计算数学组（樊玉伟）\n\n从事大模型训推与数据基础设施，覆盖推理引擎、MTP、通信优化及预训练数据处理。"
          }
        ]
      },
      "design": {
        "columns": "2"
      }
    },
    {
      "block": "collection",
      "id": "projects",
      "content": {
        "title": "核心项目",
        "text": "[早期图形学项目与完整项目列表](./project/)",
        "count": 4,
        "order": "desc",
        "filters": {
          "folders": [
            "project"
          ],
          "tag": "AI Infra"
        }
      },
      "design": {
        "columns": "2",
        "view": "compact"
      }
    },
    {
      "block": "collection",
      "id": "featured",
      "content": {
        "title": "论文与研究",
        "text": "[Google Scholar：完整学术档案](https://scholar.google.com/citations?user=jrTzf5UAAAAJ&hl=zh-CN)",
        "count": 0,
        "order": "desc",
        "filters": {
          "folders": [
            "publication"
          ]
        }
      },
      "design": {
        "columns": "2",
        "view": "compact"
      }
    },
    {
      "block": "markdown",
      "id": "skills",
      "content": {
        "title": "专业技能",
        "text": "**计算平台** — GPU / NPU；PyTorch、torch_npu、Triton；昇腾适配与性能优化。\n\n**推理系统** — Continuous Batching、Paged KV Cache、P/D 分离、MTP、融合图与异步流水；vllm-ascend（ascend-vllm/omni-infer）。\n\n**训练与并行** — 了解 Megatron、PyTorch FSDP；DP / TP / PP / CP / SP / EP；集合通信与计算通信重叠。\n\n**开发与数据** — Python、C++、Rust、Git；Data-Juicer、分布式数据管线、文档解析与代码去重。\n\n**Agent 开发** — Claude Code / Codex / DeepSeek Harness；Skill、Issue/PR 与自动化验证。\n\n**英语** — TOEFL 107；CET-6。"
      },
      "design": {
        "columns": "2"
      }
    },
    {
      "block": "collection",
      "id": "posts",
      "content": {
        "title": "技术笔记",
        "count": 3,
        "order": "desc",
        "filters": {
          "folders": [
            "post"
          ]
        }
      },
      "design": {
        "view": "compact",
        "columns": "2"
      }
    },
    {
      "block": "contact",
      "id": "contact",
      "content": {
        "title": "联系我",
        "text": "欢迎交流大模型基础设施、推理优化与 Agent 系统。",
        "email": "pzheng46@qq.com",
        "address": {
          "city": "上海",
          "country": "中国",
          "country_code": "CN"
        },
        "autolink": true,
        "contact_links": [
          {
            "icon": "github",
            "icon_pack": "fab",
            "name": "GitHub",
            "link": "https://github.com/pzheng460"
          },
          {
            "icon": "google-scholar",
            "icon_pack": "ai",
            "name": "Google Scholar",
            "link": "https://scholar.google.com/citations?user=jrTzf5UAAAAJ&hl=zh-CN"
          },
          {
            "icon": "file-pdf",
            "icon_pack": "fas",
            "name": "简历",
            "link": "https://pzheng460.github.io/uploads/resume.pdf"
          }
        ]
      },
      "design": {
        "columns": "2"
      }
    }
  ]
}
---
