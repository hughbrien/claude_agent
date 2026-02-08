# CLAUDE.md

## Project Overview

`claude_agent` is a documentation and configuration hub for a multi-repository Claude Agent system. The agent monitors multiple GitHub repositories owned by `hughbrien` for changes and sends email notifications. This repository is in early-stage development — it currently contains documentation and configuration only, with no source code implementation yet.

## Repository Structure

```
claude_agent/
├── .gitignore          # Comprehensive Python project gitignore
├── README.md           # Project title (minimal)
├── Basic_Agent.md      # Agent specification and monitored repositories
└── CLAUDE.md           # This file
```

## What the Agent Does

As defined in `Basic_Agent.md`, the agent has two core responsibilities:

1. **Monitor GitHub repositories for changes** — scans the following repos:
   - [claude_agent](https://github.com/hughbrien/claude_agent)
   - [frontend](https://github.com/hughbrien/frontend)
   - [rest-application](https://github.com/hughbrien/rest-application)
   - [basic_event_agent](https://github.com/hughbrien/basic_event_agent)

2. **Send email notifications** — delivers change notifications to hbrien@gmail.com

## Technology Stack

- **Language:** Python (inferred from `.gitignore`)
- **No build/test/CI configuration exists yet** — no `pyproject.toml`, `requirements.txt`, `Makefile`, or CI/CD workflows

## Development Commands

No build, test, lint, or format commands are configured yet. When implementation begins, this section should be updated.

## Conventions for AI Assistants

- **No source code exists yet.** If implementing features, follow standard Python conventions (PEP 8, type hints, docstrings on public APIs).
- **The `.gitignore` is pre-configured** for Python with coverage for virtual environments, pytest, mypy, Ruff, Jupyter, and common IDEs.
- **`Basic_Agent.md` is the specification document** — treat it as the source of truth for agent behavior and monitored repositories.
- **Keep documentation files concise** and focused on their purpose.
- **Do not commit** `.env` files, credentials, or API keys — the gitignore already excludes these.

## Related Repositories

This project references and monitors these sibling repositories under the `hughbrien` GitHub account:

| Repository | Description |
|---|---|
| [frontend](https://github.com/hughbrien/frontend) | Frontend application |
| [rest-application](https://github.com/hughbrien/rest-application) | REST API application |
| [basic_event_agent](https://github.com/hughbrien/basic_event_agent) | Event-based agent |
