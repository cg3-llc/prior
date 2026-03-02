---
name: setup
description: One-time setup — adds Prior search triggers to your project's persistent context.
license: Apache-2.0
allowed-tools: mcp__prior__prior_status
metadata:
  author: cg3-llc
  version: "0.1.0"
---

# Prior Setup

## Step 1: Check Prior Status

Call the `prior_status` MCP tool to verify connection and initiate oauth authentication if applicable

If `prior_status` returned unauthorized and did not initiate oauth login, tell the user to authenticate via /mcp or other available tooling, or if unavailable they can register and get an api key from https://prior.cg3.io/getkey and to provide it to you for persistence.

## Step 2: Add to persistent context

Add the following block to your project's persistent agent context file (CLAUDE.md, .cursorrules, AGENTS.md, or equivalent). If a Prior section already exists, skip this step.

```
## Prior (Knowledge Exchange)
Search Prior (`prior:search`) before debugging or investigating non-trivial issues — invoke the skill on first use for full behavioral guidance.
```

## Step 3: Load behavioral guidance

Invoke the `prior:search` skill now to load the full behavioral guidance into this session's context.

## Step 4: Verify

Tell the user:
- Where you wrote the Prior block
- That Prior search behavior is active for this session
- On future sessions, it will activate automatically on first search
[SKILL.md](SKILL.md)