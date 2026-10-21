# review-drill-summary

> **Note:** this recap was intended as a **secret gist** named `review-drill-summary.md`,
> but the API token used to build this sandbox is not permitted to create gists
> (HTTP 403 "Resource not accessible by personal access token" on every attempt).
> The full recap is stored here in the repository instead. If you want it as a
> real gist, copy this file's content to https://gist.github.com/ — it's ready to paste.

## Recap of the code-review drill sandbox

| Item | Value |
| --- | --- |
| **Repository (full name)** | `mcpmark-eval-liuhezi/code-review-drill-2026-07-15` |
| **Repository URL** | https://github.com/mcpmark-eval-liuhezi/code-review-drill-2026-07-15 |
| **Pull request** | #1 — "Add CONTRIBUTING.md and demo CI workflow (trainee exercise)" |
| **Pull request URL** | https://github.com/mcpmark-eval-liuhezi/code-review-drill-2026-07-15/pull/1 |
| **Pull request state** | Open, non-draft, from `trainee-exercise` into `main` (2 files, +46 lines) |
| **Review** | Comment-style review (state: COMMENTED) by the repo author — GitHub does not allow approving your own PR |
| **Follow-up comment** | Separate PR comment telling the trainee their next exercise step |
| **Workflow(s)** | 1 — `demo-ci` (`.github/workflows/demo-ci.yml`), active |

## Verdict line

REVIEW-DRILL-VERDICT: Changes requested — narrow the workflow trigger, tighten the timeout, and reconcile the CONTRIBUTING.md policy with what CI actually enforces before merging.

## Workflow outcome

- One workflow exists in the repository: **`demo-ci`** (id 392281091, state active).
- At the time of checking, run **39693745168** (run #1, `demo-ci`, on
  `trainee-exercise`, commit `40cdd22`) was **in progress** — the ten-minute sleep job.
- The run was **cancelled** and the cancellation was verified: the `demo` job
  finished with `conclusion: cancelled` at 23:30:59Z, and the run itself now
  reports `status: completed` / `conclusion: cancelled`.
- Run URL: https://github.com/mcpmark-eval-liuhezi/code-review-drill-2026-07-15/actions/runs/39693745168

## What was built

1. Public repository `code-review-drill-2026-07-15` with a README declaring it a throwaway practice repo.
2. Branch `trainee-exercise` cut from `main`, carrying `CONTRIBUTING.md` and `.github/workflows/demo-ci.yml` (a `demo` job that sleeps 600 seconds on every push).
3. Open, non-draft pull request #1 from `trainee-exercise` into `main`, with a description telling the trainee what to review.
4. A comment-style review on PR #1 (names both added files, raises four reviewer objections, ends with the grep-able verdict line above).
5. A separate follow-up comment on PR #1 describing the trainee's next exercise step.
6. The in-progress workflow run was cancelled and the cancellation confirmed.
