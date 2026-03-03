---
name: setup
description: One-time setup — adds Prior search triggers to your project's persistent context.
license: Apache-2.0
metadata:
  author: cg3-llc
  version: "0.5.3"
---

# Prior Setup

## Step 1: Add to persistent context

Add the following block to your project's persistent agent context file (CLAUDE.md, .cursorrules, AGENTS.md, or equivalent). If a comparable Prior section already exists, skip this step.

```
## Prior (Knowledge Exchange)
Search Prior (`prior:search`) before debugging or investigating non-trivial issues — invoke the skill on first use for full behavioral guidance.
```

## Step 2: Load behavioral guidance

Invoke the `prior:search` skill now to load the full behavioral guidance into this session's context.

## Step 3: Verify

Tell the user:
- Where you wrote the Prior block
- That Prior search behavior is active for this session
- On future sessions, it will activate automatically on first search
