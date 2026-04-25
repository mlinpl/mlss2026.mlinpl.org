# Contributing to mlss2026.mlinpl.org

## Project structure

This repository contains the source code for the mlss2026.mlinpl.org website.
The site is built using Jekyll, and the generated output is placed in the `_site/` directory.

Do not edit generated files in `_site/` directly.

## Local setup

1. Clone the repository.
2. Install Ruby dependencies:

```bash
bundle install
```

3. Run the local build and preview server:

```bash
bash run_locally.sh
```

This script:
- builds the Jekyll site into `_site/`,
- starts a local Jekyll server at `http://localhost:4000`.

## Contribution workflow

1. Create a branch from `main`:

```bash
git switch -c feature/short-description
```

2. Make your focused changes. 
   - Content and data can be found in `_data/`, `pages/`, `_includes/` and `_layouts/`.
3. Verify your changes locally by checking `http://localhost:4000` (ensure `bash run_locally.sh` is running).
4. Commit with a clear and concise message.
5. Open a pull request against this repository.

Suggested branch prefixes:
- `feature/...`
- `fix/...`
- `chore/...`

## Troubleshooting

- If changes to `_config.yml` or files in `_data/` are not reflected, restart the Jekyll server by stopping `run_locally.sh` and running it again.
- If the output looks stale, stop the server and run `bash run_locally.sh` again.
