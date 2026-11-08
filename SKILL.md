
---
name: omniskill
description: A modular AI skill system for Claude Code and OpenAI Codex, covering software engineering, debugging, Git, DevOps, documentation, and product workflows.
---

# OmniSkill

OmniSkill is a modular AI engineering skill system designed for Claude Code and OpenAI Codex.

## Purpose

Help AI coding agents approach development tasks systematically, select relevant workflows, verify results, and explain their work clearly.

## Core Rules

1. Understand the request before acting.
2. Inspect relevant project context when available.
3. Select the appropriate workflow for the task.
4. Avoid unnecessary changes.
5. Verify results when tools are available.
6. Never claim a test passed unless it was executed.
7. Respect user permissions and project boundaries.


## Available Modules

### Code Reviewer

Reference: `references/code-reviewer.md`

Activate this module when the user requests:
- Code review
- Pull request analysis
- Security vulnerability review
- Code quality assessment
- Regression risk analysis

When activated:
1. Read `references/code-reviewer.md` completely.
2. Follow its review workflow.
3. Prioritize verifiable defects over stylistic preferences.
4. Report findings by severity.
5. Never fabricate test results, file paths, or line numbers.
6. Do not modify code unless the user requests changes.

### Git Commit Writer

Reference: `references/git-commit-writer.md`

Activate this module when the user requests:
- Git commit message generation
- Conventional Commits
- Git change summaries
- Commit organization
- Commit history cleanup

When activated:
1. Read `references/git-commit-writer.md` completely.
2. Inspect actual repository changes when accessible.
3. Choose an appropriate Conventional Commit type.
4. Generate an accurate and concise commit message.
5. Never invent changes that have not been verified.
6. Do not create commits unless explicitly authorized.

## Module Selection  

Select modules according to the user's task.
Load only relevant reference files.
More specialized modules will be added later.

  
