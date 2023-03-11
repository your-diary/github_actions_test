# About

A test repository to play around with GitHub Actions.

# Workflow Files

- [`./.github/workflows/rust.yaml`](./.github/workflows/rust.yaml)

CI/CD for Rust. It creates a draft release with a built binary.

- [`./.github/workflows/pr_check.yaml`](./.github/workflows/pr_check.yaml)

Only pull requests which pass this workflow can be merged into `master`.

- [`./.github/workflows/mdbook.yaml`](./.github/workflows/mdbook.yaml)

Builds `./mdbook` via `mdbook` and deploys it to GitHub Pages (https://your-diary.github.io/github_actions_test/).

<!-- vim: set spell: -->

