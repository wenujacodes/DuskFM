# Contributing to Dawn FM

Thanks for helping improve Dawn FM.

## Workflow

We use **issues first**, then pull requests that close them.

1. **Open an issue** on [wenujacodes/DawnFM](https://github.com/wenujacodes/DawnFM/issues) describing the bug, feature, or chore.
2. **Fork** the repo (or use your existing fork) and create a branch named for the change (`feat/...`, `fix/...`, `docs/...`).
3. **Implement** on that branch with focused commits.
4. **Open a pull request** into `wenujacodes/DawnFM` from your fork.
5. In the PR body, include `Closes #<issue-number>` so the issue is linked and closed on merge.

## Guidelines

- Keep PRs focused on one issue.
- Prefer small, reviewable commits.
- Match existing code style and project structure.
- For macOS bundle or icon changes, verify with `macos/bundle.sh` after a release build.
- Do not commit secrets, signing keys, or local-only paths.

## Development

See the README for build and packaging steps:

```sh
cargo build --release
sh macos/bundle.sh target/release/dawnfm <version> out
```