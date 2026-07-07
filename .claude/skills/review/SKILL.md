---
name: review
description: Use when reviewing GitLab merge requests, git diffs, changed files, or source code. Produces actionable review comments with file path, approximate line, severity, and suggested fix.
---

# Review

Review a GitLab merge request, diff, or file.

- Apply `references/review-standard.md`.
- Output actionable comments, one per finding:
  `path/to/file.ext:line` — **Severity** — issue. Fix: suggestion.
- Use approximate line numbers when exact ones aren't visible.
- Group by severity; skip generic summaries.
- Only produce a `templates/pr-review.md` summary if explicitly asked.
