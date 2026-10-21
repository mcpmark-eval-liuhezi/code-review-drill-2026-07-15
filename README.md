# code-review-drill-2026-07-15

> **⚠️ This is a throwaway practice repository.**
> It exists purely for code-review exercises during our hands-on new-hire
> workshop. Nothing here is production code, nothing here is precious, and the
> whole repository is safe to delete at any time.

## What this is

A self-contained sandbox that you can click through together in class:

- **`main`** — the stable "production" branch of a pretend project.
- **`trainee-exercise`** — a branch carrying a small, deliberately
  imperfect change set that is opened as a pull request into `main`.
- **A pull request** — the thing you will actually review. Read the PR
  description first: it tells you what the author claims the change does and
  what you should be looking for.
- **A CI workflow** — `.github/workflows/demo-ci.yml` on
  `trainee-exercise` contains a `demo` job that simply sleeps for roughly ten
  minutes on every push. It is intentionally slow so the class can practice
  spotting a stuck run and cancelling it from the Actions tab.

## How to use it

1. Open the open pull request from `trainee-exercise` into `main`.
2. Read the PR description, then read the diff file by file.
3. Note what you'd push back on — a real reviewer always finds *something*.
4. Check the **Actions** tab: is the `demo` job still queued or running?
   Practice cancelling it.
5. Read the review left by the workshop author to compare notes.

## House rules

- Everything here is disposable. Delete, reset, or re-run at will.
- No secrets, no real users, no real data — only fabricated examples.
