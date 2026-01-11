# Contributing to Vibe Kanban

First off, **thank you** for considering contributing! I truly believe in open source and the power of community collaboration. Unlike many repositories, I actively welcome contributions of all kinds - from bug fixes to new features.

## My Promise to Contributors

- **I will respond to every PR and issue** - I guarantee feedback on all contributions
- **Bug fixes are obvious accepts** - If it fixes a bug, it's getting merged
- **New features are welcome** - I'm genuinely open to new ideas and enhancements
- **Direct line of communication** - If I'm not responding to a PR or issue, email me directly at johnvondrashek@gmail.com

## Getting Started

### Prerequisites

- [Rust](https://rustup.rs/) (latest stable)
- [Node.js](https://nodejs.org/) (>=18)
- [pnpm](https://pnpm.io/) (>=8)

Additional development tools:
```bash
cargo install cargo-watch
cargo install sqlx-cli
```

### Setup

```bash
# Clone the repository
git clone https://github.com/BloopAI/vibe-kanban.git
cd vibe-kanban

# Install dependencies
pnpm i

# Run the development server
pnpm run dev
```

### Project Structure

- `crates/` - Rust workspace crates (server, db, executors, services, utils, deployment)
- `frontend/` - React + TypeScript app (Vite, Tailwind)
- `shared/` - Generated TypeScript types (do not edit directly)
- `npx-cli/` - Files published to the npm CLI package
- `docs/` - Documentation files

### Running Tests

```bash
# Rust tests
cargo test --workspace

# Frontend type checks
pnpm run check

# Lint
pnpm run lint
```

## Submitting Changes

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Run tests and ensure they pass
5. Commit your changes with a clear message
6. Push to your fork
7. Open a Pull Request

## Code Style

- **Rust**: `rustfmt` enforced; snake_case for modules, PascalCase for types
- **TypeScript/React**: ESLint + Prettier; PascalCase for components, camelCase for variables/functions

## Code of Conduct

This project follows the [Rule of St. Benedict](CODE_OF_CONDUCT.md) as its code of conduct.

## Questions?

- Open an issue
- Email: johnvondrashek@gmail.com
