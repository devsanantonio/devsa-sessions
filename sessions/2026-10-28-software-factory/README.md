# Software Factory Night

**Wednesday, October 28, 2026 · 6:00–7:30 PM CT · Software Factory Night stage, DEVSA Discord**

An introduction to [On PAR Dev's Software Factory](https://github.com/on-par/software-factory), installed and used together. It's a local command-line tool, MIT-licensed, that takes a GitHub issue through four phases with AI coding agents (plan, build, check, ship) and stops at a pull request that's ready for you to review. Thanks to On PAR Dev for building it in the open.

## Before you start

- **Node.js 24 or newer**, and `git` with your name and email set.
- **The GitHub CLI** (`gh`), signed in with `gh auth login`.
- **One supported coding agent CLI**, installed and signed in, such as Claude Code or Codex. The project's [agents guide](https://github.com/on-par/software-factory/blob/main/docs/agents.md) lists them.
- **A practice repo you own**, with a few small open issues. Don't start on your work codebase.

## Read this first: safety

To run unattended, the factory starts the coding agents with their permission prompts turned off. Builds happen in a separate git worktree, never your main checkout, and are sandboxed where your OS supports it, but the agents still run as you, with your files and your GitHub token. **Only point it at repos and issues you trust.** It never merges on its own unless you turn auto-merge on. The project's [Safety section](https://github.com/on-par/software-factory#safety) has the details.

## Set it up

From the project's [quick start](https://github.com/on-par/software-factory#quick-start):

```sh
npm install -g @on-par/factory-cli
factory --version
factory doctor            # checks git, gh, your agent CLI and token; fix what it flags

cd path/to/your/practice-repo
factory init              # creates a local .factory/ folder (not committed)

factory triage            # a model proposes an order for your open issues
factory triage accept     # makes that the queue
factory ship 42           # plan → build → check → ship issue #42, ending at a PR
```

Merging stays with you: review the PR, then merge it yourself or run `factory land 42`.

## Links

- Repository: [on-par/software-factory](https://github.com/on-par/software-factory)
- On PAR Dev: [github.com/on-par](https://github.com/on-par)

## What people built

Shipped an issue with the factory? Add a line with a pull request: the issue, the PR it produced, and what you'd tell the next person.

<!-- Add below this line: - Repo / issue → PR link: what happened. By @your-github -->
