# Agent Guide

English · [简体中文](AGENTS.zh-CN.md)

This file applies to every agent working in the public DuanDu repository, including agents that do not have access to the private parent project or earlier conversations.

## Start here

Before changing anything:

1. Read [`README.md`](README.md).
2. Check the current branch, working tree, and remote state.
3. Preserve changes that are not part of the current task.
4. Confirm whether the task authorizes a local change only, a commit, or a public push.

## Project context

DuanDu is an experimental cross-platform device continuity project. It grew out of the everyday friction of moving text, screenshots, notifications, and files between Windows, macOS, Linux, Android, and iOS devices.

There is no usable release yet. The project is still exploring real use cases, platform restrictions, privacy expectations, and the scope of a sensible first version. Do not present planned features as implemented or promised.

## Current boundaries

- Do not start product implementation unless the user explicitly moves the project into development.
- Do not choose a framework, architecture, protocol, or dependency without an approved task.
- Do not assume feature parity across operating systems.
- Do not make unsupported security, privacy, compatibility, or performance claims.
- Do not add a license or state that reuse rights have been granted. A license has not been selected yet.
- Do not add contribution guidance that implies the project is ready to accept code contributions.

## Public repository scope

This repository is intended for public-facing source code and documentation. Never add private product plans, credentials, real user data, internal logs, billing details, infrastructure secrets, or unpublished security findings.

The private parent project tracks this repository as a Git submodule at `open-source/duandu`. After a public repository commit is pushed, the parent project must be updated to point to the new commit.

## Documentation

- English is the primary public language.
- Every public English document must have a matching Simplified Chinese file using the `.zh-CN.md` suffix.
- The two language versions must link to each other near the top.
- Keep both versions factually aligned in the same change.
- Write in a direct, personal, and natural tone. Avoid corporate filler, exaggerated claims, and generic AI-style wording.
- Clearly describe DuanDu as an experimental test project until a real release exists.
- Use Markdown for documentation.

## Git workflow

- Keep `main` usable and use short-lived branches for larger changes.
- Make focused commits with clear messages.
- Check formatting, links, and `git diff --check` before committing.
- Never point the parent project at a public commit that has not been pushed.
- Pushing, publishing releases, creating public issues, or changing repository settings requires explicit authorization for the current task.

## Before finishing

1. Review the diff for unintended or private information.
2. Confirm English and Chinese documents are aligned and cross-linked.
3. Check the repository status.
4. If a public commit was pushed, update and commit the submodule pointer in the parent project when it is available.
5. Report what changed, what was pushed, and any remaining decision or blocker.

