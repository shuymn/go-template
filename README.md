# go-template

Template repository for bootstrapping a new Go project.

This README is intentionally temporary. After you start your own project, replace it with project-specific documentation.

## What This Template Includes

- `Taskfile.yml` as the single entrypoint for local tasks, CI, and hooks
- `golangci-lint` for linting and formatting
- `lefthook` for `pre-commit` and `pre-push` automation
- GitHub Actions-friendly task structure
- Project-local caches under `.cache/` for Go and lint tooling
- Starter docs for repository rules and review conventions

## First Things To Edit

Use this checklist right after creating a repository from the template:

1. Change the module path in [`go.mod`](go.mod).
2. Rename the binary in [`Taskfile.yml`](Taskfile.yml) by updating `BINARY_NAME`.
3. Replace [`main.go`](main.go) and any starter code with your actual application entrypoint and package layout.
4. Rewrite this README with project-specific purpose, setup, run, test, and deployment information.
5. Review [`AGENTS.md`](AGENTS.md) and [`docs/`](docs/) and keep only the rules and guidance you want in the new repository.

## Local Setup

Install the required tools, then enable hooks:

```bash
lefthook install
```

Useful commands:

```bash
task
task build
task test
task lint
task fmt
task check
```

## Recommended Bootstrap Pass

After your first round of edits:

1. Run `task build`.
2. Run `task test`.
3. Run `task check`.
4. Commit only after the README and template defaults no longer describe `go-template`.

## Replace This README With

When the repository stops being a template, replace this file with sections like:

- Project overview
- Requirements
- Setup
- Local development commands
- Testing
- Deployment or release process
- Repository layout
- Links to deeper docs if needed
