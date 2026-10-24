# Hermes Night — install Hermes Agent

**Wednesday, October 21, 2026 · 6:00–7:30 PM CT · Hermes Night stage, DEVSA Discord**

DEVSA's first Discord-exclusive live session. [Hermes Agent](https://github.com/NousResearch/hermes-agent) is an open-source AI agent from [Nous Research](https://nousresearch.com), MIT-licensed, that runs on your own machine and grows with you: it keeps memory, learns skills, and works through a terminal, a desktop app, or your messaging apps.

## Set it up

The official instructions are the source of truth and change often: [installation docs](https://hermes-agent.nousresearch.com/docs/getting-started/installation).

**macOS, Linux or WSL2**

```sh
curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash
```

**Windows (PowerShell)**

```powershell
iex (irm https://hermes-agent.nousresearch.com/install.ps1)
```

The installer brings its own Python environment and dependencies. On Windows, some antivirus tools flag the bundled `uv.exe` (Astral's Python package manager); Nous Research's README covers that false positive.

As with any install script piped to a shell: read it first if you want to know what it does. It's at the URL in the command.

## Links

- Repository: [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)
- Docs: [hermes-agent.nousresearch.com](https://hermes-agent.nousresearch.com)

## What people built

Set up Hermes and made it do something worth showing? Add a line here with a pull request: what you had it do, and a link if there is one.

<!-- Add below this line: - What you built — link. By @your-github -->
