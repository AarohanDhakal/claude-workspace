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

- Personal skills live at `~/.claude/skills/` — always check there first before using global or built-in skills.
- Skill priority order (highest to lowest):
  1. **Project-level skills** — defined inside the current project
  2. **Personal skills** — located at `~/.claude/skills/`
  3. **Global skills** — built-in or platform-wide defaults
- If a personal skill and a global skill overlap or do the same thing, always use the personal skill.
- If a project-level skill and a personal skill overlap, always use the project-level skill.

### Personal Skills Available (`~/.claude/skills/`)

| Skill | Skill | Skill |
|---|---|---|
| ab-test-setup | ad-creative | ai-seo |
| analytics-tracking | churn-prevention | cold-email |
| competitor-alternatives | content-strategy | copy-editing |
| copywriting | email-sequence | explain-code |
| form-cro | free-tool-strategy | launch-strategy |
| lead-magnets | marketing-ideas | marketing-psychology |
| onboarding-cro | page-cro | paid-ads |
| paywall-upgrade-cro | popup-cro | pricing-strategy |
| product-marketing-context | programmatic-seo | referral-program |
| revops | sales-enablement | schema-markup |
| seo | seo-audit | seo-competitor-pages |
| seo-content | seo-geo | seo-hreflang |
| seo-images | seo-page | seo-plan |
| seo-programmatic | seo-schema | seo-sitemap |
| seo-technical | signup-flow-cro | site-architecture |
| social-content | | |

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
