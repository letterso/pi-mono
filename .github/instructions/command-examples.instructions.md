---
description: "Use when proposing shell commands, scripts, setup steps, or troubleshooting instructions. Enforces runnable command examples with concrete placeholders and no vague tokens."
name: "Runnable Command Examples"
---
# Runnable Command Examples

- This is a hard rule: command examples must be directly runnable with concrete values.
- Never use vague placeholders such as `your_xxx`, `some_path`, `foo`, or `bar`.
- Prefer explicit sample values that show valid shape and location.
- Keep command snippets copy-paste friendly.

## Good Patterns

```bash
# specific path + concrete value
npm run check --workspace packages/ai
```

```bash
# concrete issue number and file path
gh issue view 123 --json title,body,comments,labels,state
```

```bash
# concrete URL and output file
curl -L "https://example.com/api/v1/status" -o /tmp/status.json
```

## Avoid

```bash
npm run check --workspace your_workspace
```

```bash
gh issue view <number>
```

```bash
cp some_path/file.txt /tmp/out.txt
```
