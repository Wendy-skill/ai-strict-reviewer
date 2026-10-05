# AI Strict Reviewer

AI Strict Reviewer is a bilingual, evidence-based review Skill for scientific manuscripts, engineering papers, and PhD theses. It checks methodology, evidence, statistics, interpretation, and whether conclusions are supported. It distinguishes what a document reports from what has been independently checked, and it does not silently rewrite the manuscript.

## Files

```text
ai-strict-reviewer/
├── SKILL.md
└── references/
    ├── phd-thesis-review.md
    ├── cfd-wind-tunnel-extension.md
    └── output-templates.md
```

Keep the `references/` folder beside `SKILL.md`. Install the complete `ai-strict-reviewer` folder in your AI agent's Skills directory, or upload it as a ZIP in a host that supports custom Skills. The exact installation steps depend on the host.

## Basic use

Upload or enable the Skill, provide the manuscript, then ask:

```text
Use AI Strict Reviewer.

Review this manuscript in Full Scientific Review mode.
Focus on methodology, evidence, statistics, and claim support.
Do not rewrite the manuscript.
```

For a thesis, you can start with:

```text
调用 AI Strict Reviewer，按 PhD Thesis Review 模式审这篇博士论文。
先建立审查框架，然后停止；不要改写正文。
```