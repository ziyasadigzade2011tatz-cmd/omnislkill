# Git Commit Writer — OmniSkill Module

## Purpose

Generate accurate, concise and meaningful Git commit messages based on actual repository changes.

## When to Use

Activate when the user requests:
- Commit message generation
- Conventional Commits
- Commit history cleanup
- Git change summaries
- Commit organization and grouping

## Workflow

### 1. Inspect Changes
- Check git status.
- Read staged and unstaged diffs when accessible.
- Identify the purpose of each modification.
- Never assume files were changed without evidence.

### 2. Classify Changes

Use Conventional Commits:

- feat: New functionality
- fix: Bug fixes
- refactor: Internal restructuring
- perf: Performance improvements
- docs: Documentation updates
- test: Test additions and changes
- build: Build system changes
- ci: CI/CD changes
- chore: Maintenance work

### 3. Generate Commit Messages

Preferred structure:

<type>(optional-scope): concise description

Optional body:
- Explain why the change was necessary.
- Summarize significant implementation details.
- Describe compatibility or migration considerations.

Optional footer:
BREAKING CHANGE: describe the breaking change

### 4. Validate

Ensure that:
- The message reflects actual changes.
- The subject is specific and concise.
- No unsupported claims are included.
- Sensitive data is excluded.
- Unrelated changes are separated when practical.

## Safety Rules

- Do not create commits unless explicitly authorized.
- Never force-push without explicit authorization.
- Do not rewrite Git history without approval.
- Do not stage unrelated files automatically.
- Do not include tokens, passwords, or secrets.

## Output Format

1. Recommended commit message
2. Explanation of selected type and scope
3. Optional commit body
4. Warnings about unrelated or risky changes

## Completion Criteria

The proposed message must accurately describe the changes and comply with Conventional Commits.
