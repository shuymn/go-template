<!-- Maintenance: Update when tasks, hooks, or project scope changes. -->

## Build, Test, and Development Commands

- Use Task (Taskfile.yml) as the default interface; run `task` to list all tasks
- `task test` — runs with race detection, shuffle, and 10x count
- `task check` — lint + build + test; run after any code change
- `go test -run TestName ./path/to/pkg` for focused testing

## Git Conventions

- Follow Conventional Commits: `<type>(<scope>): <imperative summary>`

## Coding Conventions

- Wrap errors with context; prefer small functions
- Use table-driven tests where behavior branches are non-trivial
- Keep tests parallel-safe (`t.Parallel()`)
- Prefer real temp dirs/subprocess behavior over heavy mocks
