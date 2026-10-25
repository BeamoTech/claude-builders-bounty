# Claude Builders Bounty — agent guide

`AGENTS.md` is the canonical project guide. Read `~/dev/AGENTS.md` for workspace
safety, CI cost and storage rules when available.

This is a Markdown bounty board, not an application. Read `README.md` and
`LICENSE`; issue state and acceptance criteria need current source evidence.

- Keep descriptions, links and acceptance criteria clear and factual. Do not
  claim validation, acceptance, payment or completion without actual evidence.
- Guide maintenance does not authorize posting/claiming bounties, issue comments,
  payments or other external actions. Preserve contributor licensing/notices.
- Review Markdown and relative links, then run `git diff --check`. There is no
  application build or configured hosted gate to run for instruction edits.
- Fetch current refs, preserve shared changes, stage explicit owned paths and
  use normal pushes. Never commit credentials, payment records or private messages.

<!-- BEGIN BEAMO UNFINISHED WORK -->
## Unfinished work

- Read the project's unfinished work record at task start. Use its existing
  canonical backlog, or `.ai/memory/unfinished-work.md` if none exists; link
  the record from `.ai/memory/MEMORY.md` when creating it. Chat is not storage.
- Always save every incomplete requested item, deferred issue, blocked check
  and pending merge/release step as they arise and before ending, pausing,
  handing off or changing tasks. Checkpoint after meaningful progress.
- Each item needs an ID/status, remaining acceptance criteria, exact next
  action, blockers/required approval, date/author, repo/branch/commit/worktree
  and relevant files or links. Separate completed checks and their evidence
  from failed, skipped and unrun checks; distinguish local, pushed and deployed
  state. Preserve partial source work without staging another agent's changes.
- Resume from the record, recheck current source and evidence, and update or
  mark items done only when their acceptance criteria pass. Record reasons for
  canceled/superseded items. Preserve useful history and others' entries; reread
  before editing and append separate items when concurrent work would overwrite
  them.
- Never store credentials or raw personal/customer records. Notes do not grant
  approval or prove deployment. If project writing is blocked, save a durable
  workspace handoff with the exact project/ref, record the blocker, and report
  its location before stopping; do not silently lose unfinished work.
<!-- END BEAMO UNFINISHED WORK -->

## Greptile review rules

Greptile reviews pull requests in this repo. Its feedback is part of the work, not decoration.

### The loop (required before merge)
1. After opening a PR, wait for the Greptile review and read **every** Greptile comment on the PR — inline comments and the summary review.
2. Fix every valid point in code. If you believe a point is wrong, reply to that comment on the PR explaining why — never silently ignore it.
3. Push the fixes and let Greptile re-review. Repeat until the review is clean or every remaining comment has an on-PR rebuttal.
4. Do not merge a PR with unaddressed Greptile comments.

### Credit discipline (hard cap — no overage exists)
- Each author gets **50 included review credits per billing period**. Flex/overage billing is capped at **$0** at the account level: when the credits run out, Greptile simply stops reviewing until the next period. There is no paid overflow and nobody may re-enable it.
- Every push to a PR can trigger a re-review and burn credits. Batch related fixes into fewer, larger pushes instead of drip-pushing commit-by-commit.
- Don't open throwaway or duplicate PRs against reviewed branches; close superseded PRs promptly.
- If reviews stop mid-cycle, assume the allowance is exhausted — finish the loop by reading the last Greptile comments you already have, and note it in the PR.

### Reporting
- When you finish a PR, state in your summary: Greptile comments received, how many you fixed, how many you rebutted and why.
