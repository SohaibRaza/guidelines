# Conventional Commits

Conventional Commit is a commit message format and convention that helps standardize commit messages, making it easier to understand the purpose and impact of each commit.
Conventional Commit messages have a specific structure:

```bash
<type>(<scope>): <subject>

<body>

<footer>
```

- **`<type>`**: Describes the purpose or category of the commit. It can be one of the following types:
  - feat: A new feature introduction.
  - fix: A bug fix.
  - chore: Routine tasks, maintenance, or refactoring.
  - docs: Documentation changes.
  - style: Code style changes (e.g., formatting).
  - test: Adding or modifying tests.
  - perf: Performance improvements.
  - build: Changes related to the build process.
  - ci: Continuous integration and deployment changes.
  - revert: Reverting a previous commit.
  - feat(scope)!: <subject>: A breaking change for a new feature.
  - fix(scope)!: <subject>: A breaking change for a bug fix.
- **`<scope>`** (optional): Describes the part of the project affected by the commit. It can be a module, component, or directory.
- **`<subject>`**: A brief, imperative description of the change. It should start with a lowercase letter and not exceed 50 characters.
- **`<body>`** (optional): Provides additional context, explanation, or details about the change. Use a blank line between the subject and body.
- **`<footer>`** (optional): Contains metadata or references to issues (Jira Tickets) or pull requests. You can reference issues or pull requests using keywords like "Closes," "Fixes," or "Resolves."

Examples:

sample git commits consisting of <type>(<scope>): <subject>

```bash
git commit -m "feat(auth): add OAuth2 authentication"

git commit -m "chore(build): update webpack configuration"
```

sample git commit with body:

```bash
git commit -m "docs(readme): update installation instructions
```

- Added detailed steps for installation.
- Clarified usage examples."

sample git commit with footer:

```bash
git commit -m "fix(AssignUser): add toast notification

Closes #RAK-76"
```
