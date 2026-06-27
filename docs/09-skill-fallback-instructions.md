# Skill Fallback Instructions

Use this when a Codex session does not discover the AstraFlow skill.

Copy this block into the target project's `AGENTS.md`:

```markdown
## AstraFlow Fallback

When the user says AstraFlow, astraflow, "Use AstraFlow", "使用 AstraFlow", "我不会写提示词", or gives a rough product idea:

- Do not search for an AstraFlow tool, dynamic capability, MCP tool, or plugin.
- AstraFlow is a workflow, not a runtime tool.
- Do not stop after saying you will check availability.

Instead, immediately:

1. Create or update `docs/00-project-context.md`.
2. Create or update `docs/01-product-brief.md`.
3. Create or update `docs/02-prd.md`.
4. Create or update `docs/03-design-system.md`.
5. Create or update `docs/05-quality-gates.md`.
6. Produce 3 MVP/product/design directions.
7. Ask the user to choose one direction.

If the user did not ask for files, respond with the structured brief and 3 directions directly.
```

## Why This Exists

Some already-running sessions do not hot-load newly installed skills. A short project-level instruction in `AGENTS.md` is more reliable than relying only on global skill discovery.

