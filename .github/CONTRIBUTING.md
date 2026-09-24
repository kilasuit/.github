# Contributing to kilasuit Projects

Welcome — and thank you for considering a contribution. 

This document covers org-wide polices and Individual repos may have
project-specific guidance in their own `README.md` or `CONTRIBUTING.md`; where
they conflict with this document, the repo-level doc takes precedence.

---

## Scope and governance

I focus mainly on PowerShell tooling. Before proposing a large feature or
a significant design change, raise an issue so that it can be discussed & 
importantly agreed upon.

---

## Before you contribute

1. **Check existing issues and PRs.** Someone may already be working on it.
2. **Read the repo's README.** Each project documents its purpose, status, and
   any project-specific constraints.
3. **Agree to the license terms.** By submitting a contribution you agree that
   your work is licensed under the repo's license (MIT unless noted otherwise).
   See [License by contribution](#license-by-contribution) below.

---

## Development setup

Each repo may have a unique development setup, whilst we look in time to standardise this.

**Target platforms:** 

Whilst we could aim to support Windows PowerShell 5.1, as a forward
thinking developer we now build for and support only the in support versions
of PowerShell 7.x on Windows, Linux, and macOS. 

This is inline with PowerShell 7 being likely included in a future version of 
both the Windows Client & Server Operating Systems.

Support on Linux and MacOS is a best effort basis.
---

## Branching and commits

- **Fork the repo**
- Start work on a new branch using the following format:
  `username/issueNumber-briefDescriptionOfIssue`
  this should look like
  `kilasuit/9-variableRenames`
- **Keep commits focused.** One logical change per commit. You may use the [Conventional
  Commits][conventional-commits] style as below - we don't follow this today:
  - `fix: correct null reference in Invoke-PSDepend`
  - `feat: add -WhatIf support to Install task`
  - `docs: clarify quickstart example`
  - `chore: bump Pester to 5.6`
  - `test: add coverage for empty dependency file`
- Feel free to locally clean your commits up using rebase & fixup
- If your branch diverges from the main branch we recommend you rebase from main,
  as opposed to a merge commit. 
- Please Sign your commits!
- **Keep `main` green.**
- You should not be able to force-push to `main` & you should not do so to any shared branches.
- However, you own that branch, so you can force push to it - however we recommend using `--force-with-lease` 
---

## Pull request expectations

Before opening a PR:

If there is a PR Template
 - Fill out the PR template completely.  
PRs with empty templates or no linked issue
for non-trivial changes will be asked to complete the template before review
starts or will be outright rejected.
 
**Draft PRs** are welcome for early feedback. Mark them ready for review when
you want the full review pass.

---

## Issue & PR review expectations

- I aim to respond to Issues & PR's within **14 days**.
- If an issue or PR sits without response after this time then please tag me to bring it to my attention.

---

## Releases

Releases are ad-hoc and as per each repository & downstream platforms.
However we try and run with the idea that latest code in main 
is working code that can be classified as "release ready" 

Therefore, commits to main/master branches, could be seen as a release.

We are working on adding automation using git tags to properly formalise the releases & release process 

---

## License by contribution

By submitting a pull request or other contribution, you agree that your
contribution is made under the same license as the project you are contributing
to (MIT unless the repo states otherwise). You represent that you have the right
to make the contribution under those terms.

If your employer has rights to code you write, by submitting to these repo's, I make 
the assumption that you have chosen to do so as part of your own time, and not your employers, 
or that in doing so even whilst using their time, the act of doing so aids them and their work & is by inclusion 
of mutual benefit by the submission. 
This assumption, whether `technically correct or not` protects the code submission. 
If this is not the case, and we have then merged the code you've submitted we 
invite your employer to engage with us on this, however we will not step back and remove the submission.

We instead, when approached by a current/previous employer, will update documentation to point out that they have been supportive as a user of the software and via submitted PR's have helped improve the
open source software that these repos contain.

---

## Questions?

Raise an issue in the respective repo.
