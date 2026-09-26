---
name: github-implementation-tracking
description: Track implementation from GitHub issue through pull request and closeout. Use when a change needs a planning issue, reviewable delivery, or cross-repository handoff.
---

# GitHub implementation tracking

Follow repository `AGENTS.md`, `CONTRIBUTING.md`, templates, merge policy, and related history. They govern branches, checks, commits, and merges. Treat other repositories as read-only unless requested.

## Choose the record

- Bounded work: use one PR; skip an issue if the PR holds result, scope, proof, risk, and rollback. Commit directly to the default branch only where explicitly allowed.
- Investigation, multiple acceptance items, dependent proof, or rollout: use a narrow issue. Program: use an umbrella with independently provable PRs. Split for ownership, review, or rollback; keep behavior and proof together. If a companion repository disables issues, link its PR to the owning tracker.

## Track the work

- Issue: state result, verified causes versus assumptions, scope, exclusions, handoffs, safety rules, and checkboxes for code, tests, evidence, docs, delivery, and cleanup. Pin external authority to a source revision plus relevant build, schema, fixture, or device identity.
- Updates: record strategy, PR-ready, and merged checkpoints; add progress when scope or evidence changes. Link PRs and commits, exact checks and results, remaining work, and next slice. Explain regrouping; uncheck invalidated proof.
- PR: use its template. State result and cause, issue link, pushed head, checks, environment, results, omissions, relevant safety, privacy, permission, dependency, size, or compatibility impact, risk, and rollback. Use synthetic or redacted evidence; a CI non-start is no proof. Keep in-scope fixes in the open PR and refresh proof.
- Use `Closes #N` only for full resolution. For an umbrella, write `Tracked by #N; this PR does not close it.` Keep owner PRs draft until evidence is complete if ready status triggers merge.

## Close out

Recheck the exact head, checklist, evidence, and merge policy. Confirm the merge; after rebase merge, compare merged and tested trees. Sync the default branch, remove task-owned branches and artifacts, and update the issue. Close a narrow issue when complete; keep an umbrella open through rollout and cleanup. Reopen if later evidence invalidates closeout.
