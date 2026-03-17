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

## Skills

- Always use global skills by default.
- If a project-level skill exists, give it priority over the global equivalent.
- If a global skill and a project-level skill do the same thing or overlap significantly, always prefer the project-level skill.

## Design

- For any design work (images, visuals, illustrations, graphics), always use the Nano Banana image generation connector — it has already been added to this workspace.

## Memory & History

- A running work log is maintained in [`WORKLOG.md`](./WORKLOG.md).
- At the **start of every session**, read `WORKLOG.md` to restore context on what has been worked on previously.
- At the **end of every session** (or when wrapping up a significant piece of work), append a new dated entry to `WORKLOG.md` with:
  - A short session summary describing what was done and why
  - A list of files created, modified, or deleted
  - Any decisions made, open questions, or next steps
- Always commit and push updates to `WORKLOG.md` along with the related code changes.
- Never overwrite or delete past entries — only append.
