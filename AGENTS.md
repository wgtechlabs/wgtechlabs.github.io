# Repository Instructions

## Scope

These instructions apply to the entire repository. Preserve the existing one-page design, brand assets, accessibility, responsive behavior, and reduced-motion support.

## Development

- Use Bun and the existing Vite setup; do not add dependencies without a clear need.
- Keep page structure in `index.html`, styles in `src/style.css`, and static assets in `public/`.
- Do not invent organization claims, projects, sponsors, metrics, or contact details.
- Use official brand assets and verified destinations for external links.
- Run `bun run build` after changes. Check desktop and mobile layouts for visual work.

## Clean Flow

- `main` is the stable production branch; `dev` is the integration branch.
- Create short-lived branches from `dev` using `feature/`, `fix/`, `docs/`, `chore/`, `test/`, or `refactor/`.
- Target feature pull requests at `dev` and squash merge them.
- Promote stable `dev` to `main` with a regular merge commit and a `🚀 release:` pull-request title.
- Avoid direct commits to `main` and `dev`. Delete merged feature branches when appropriate.

## Clean Commit

Use `<emoji> <type>: <description>` or `<emoji> <type> (<scope>): <description>`.

- `📦 new` — new features, files, or capabilities
- `🔧 update` — changes and bug fixes
- `🗑️ remove` — removals
- `🔒 security` — security fixes
- `⚙️ setup` — configuration, CI, and tooling
- `☕ chore` — maintenance
- `🧪 test` — tests
- `📖 docs` — documentation
- `🚀 release` — releases

Use present tense, lowercase descriptions, no final period, and keep the first line under 72 characters when practical.

## Safety

- Preserve unrelated user changes and never commit secrets.
- Do not commit generated `dist/` output.
- Do not commit, push, deploy, merge, or publish unless the user explicitly asks.
