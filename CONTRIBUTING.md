# Contributing to this sandbox

Welcome! This is a **practice repository** for the code-review workshop, so the
rules below are deliberately simple and designed to be exercised in class.

## Ground rules

1. **Work on branches, never on `main`.** `main` is the pretend production
   branch; every change reaches it through a pull request.

2. **Every change goes through a pull request.** No direct pushes to `main` —
   even for "tiny" fixes. That's the habit we're training.

3. **Keep pull requests small.** One logical change per PR. If it needs a
   paragraph of explanation in the title, it's probably two PRs.

4. **Write a real description.** A PR description should say *why* the change
   exists, not just restate the diff.

5. **CI must pass before review.** CI on this sandbox includes a deliberately
   slow `demo` job (it sleeps for about ten minutes) so the class can practise
   spotting and cancelling a stuck run — do not merge while it is pending.

6. **Reviews are discussions, not verdicts.** Ask questions, suggest
   alternatives, point out risks. "LGTM" alone is not a review.

## Review checklist (what reviewers look for here)

- Does the change do what the description claims?
- Is anything added that does not belong in this PR?
- Is there any way the CI setup could waste runner time or behave
  unexpectedly?
- Would this be easy to maintain six months from now?
