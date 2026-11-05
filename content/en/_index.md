---
{
  "title": "",
  "type": "landing",
  "sections": [
    {
      "block": "about.biography",
      "id": "about",
      "content": {
        "title": "About",
        "username": "admin"
      }
    },
    {
      "block": "experience",
      "id": "experience",
      "content": {
        "title": "Experience",
        "date_format": "Jan 2006",
        "items": [
          {
            "title": "AI Infrastructure Researcher",
            "company": "Huawei Technologies · 2012 Laboratories",
            "company_url": "https://www.huawei.com/",
            "location": "Shanghai",
            "date_start": "2025-02-01",
            "date_end": "",
            "description": "Computational Mathematics Group, Theory Research Department (Yuwei Fan).\n\nGrade 15; **A+** performance rating in my first year. Work on inference engines, MTP, communication optimization and pretraining data infrastructure."
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
        "title": "Selected projects",
        "text": "[Earlier graphics work and all projects](./project/)",
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
        "title": "Publications & research",
        "text": "[Google Scholar: academic profile](https://scholar.google.com/citations?user=jrTzf5UAAAAJ&hl=zh-CN)",
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
        "title": "Skills",
        "text": "**Platforms** — GPU / NPU; PyTorch, torch_npu and Triton; Ascend adaptation and performance optimization.\n\n**Inference** — Continuous batching, paged KV cache, P/D disaggregation, MTP, fused graphs and asynchronous pipelines; vllm-ascend (ascend-vllm/omni-infer).\n\n**Training & parallelism** — Familiar with Megatron and PyTorch FSDP; DP / TP / PP / CP / SP / EP; collectives and computation–communication overlap.\n\n**Development & data** — Python, C++, Rust and Git; Data-Juicer, distributed pipelines, document parsing and code deduplication.\n\n**Agent development** — Claude Code / Codex / DeepSeek Harness; skills, issue/PR workflows and automated validation.\n\n**Languages** — TOEFL 107; CET-6."
      },
      "design": {
        "columns": "2"
      }
    },
    {
      "block": "collection",
      "id": "posts",
      "content": {
        "title": "Technical notes",
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
        "title": "Contact",
        "text": "Get in touch about LLM infrastructure, efficient inference and agent systems.",
        "email": "pzheng46@qq.com",
        "address": {
          "city": "Shanghai",
          "country": "China",
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
            "name": "Resume",
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
