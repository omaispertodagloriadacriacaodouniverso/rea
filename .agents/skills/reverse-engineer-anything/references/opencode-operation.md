# Operating REA skills under opencode

- Subagents here expose MCP only (no host `read`/`grep`): paste the artifact
  excerpt into the review prompt; the reviewer returns hypotheses, the executor
  verifies each with evidence. Never send a bare file path for review.
- Recency is executor-owned: subagents have `websearch` deny, so version/API
  claims from the last 12 months must be checked by the executor with live
  sources, never delegated unchecked.
- Destructive analysis (overwrite, `git push --force`, sudo, system config)
  needs explicit confirmation at the tool boundary; if approval is unavailable,
  fail closed (do not run).
