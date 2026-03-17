# Claude Workspace Rules

## Git & GitHub

- After every change or set of changes, stage the relevant files, write a clear and descriptive commit message, commit, and push to the remote repository at `https://github.com/AarohanDhakal/claude-workspace`.
- Commit messages must follow this format:
  - Use a short imperative subject line (e.g. `Add login page`, `Fix null pointer in auth handler`)
  - Add a body if the change is non-trivial, explaining the *why* not just the *what*
  - Keep the subject under 72 characters
- Never skip hooks (`--no-verify`) unless explicitly instructed.
- Never force push unless explicitly instructed.
- Always push to the `main` branch unless working on a feature branch that was explicitly requested.
