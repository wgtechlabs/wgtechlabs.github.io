# WG Technology Labs

The official website for [WG Technology Labs](https://wgtechlabs.github.io/), an open-source organization publishing libraries, community support tools, and shipping conventions.

## About the site

This is a static one-page site built with [Vite](https://vite.dev/) and deployed to GitHub Pages. It introduces the organization, highlights selected projects and sponsors, and links to the places where WG Technology Labs publishes its work.

## Development

The project uses [Bun](https://bun.sh/).

```bash
bun install
bun run dev
```

Create a production build with:

```bash
bun run build
```

Preview that build locally with:

```bash
bun run preview
```

## Project structure

```text
.
├── .github/workflows/deploy.yml  # GitHub Pages deployment
├── public/                       # Logos, fonts, and favicon
├── src/
│   ├── main.js                   # Vite entry point
│   └── style.css                 # Site styles and motion
├── index.html                    # Page content and structure
└── vite.config.js                # Vite configuration
```

## Contributing

This repository follows the [WG Tech Labs Clean Workflow](https://github.com/wgtechlabs/clean-workflow). Read [`AGENTS.md`](./AGENTS.md) before making changes.

In short:

- Branch from `dev`.
- Use a short-lived branch such as `feature/...`, `fix/...`, or `docs/...`.
- Open feature pull requests against `dev`.
- Promote stable changes from `dev` to `main`.
- Keep commits focused and use the Clean Commit format.

## Deployment

Pushes to `main` trigger the GitHub Pages workflow. The workflow installs dependencies with Bun, builds the site, and deploys the generated `dist/` directory.

## Sponsors

Thank you to [Unthread](https://unthread.io), [Docker](https://www.docker.com), and [Railway](https://railway.com) for supporting the work.
