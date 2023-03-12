# About

A test repository to play around with GitHub Actions.

# Workflow Files

- [`./.github/workflows/rust.yaml`](./.github/workflows/rust.yaml)

CI/CD for Rust. It creates a draft release with a built binary.

- [`./.github/workflows/pr_check.yaml`](./.github/workflows/pr_check.yaml)

Only pull requests which pass this workflow can be merged into `master`.

- [`./.github/workflows/mdbook.yaml`](./.github/workflows/mdbook.yaml)

Builds `./mdbook` via `mdbook` and deploys it to GitHub Pages (https://your-diary.github.io/github_actions_test/).

- [`./.github/workflows/act.yaml`](./.github/workflows/act.yaml)

Runs a different job depending on whether this workflow is run natively or run locally via [`act`](https://github.com/nektos/act):

    ```bash
    $ echo '{"act": true}' > ~/ramdisk/event.json
    $ act -e ~/ramdisk/event.json -W .github/workflows/act.yaml
    ```

<!-- vim: set spell: -->

