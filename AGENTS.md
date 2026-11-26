<!-- BEGIN:nextjs-agent-rules -->

# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` (resolved from this file's directory; in monorepos the `next` package may not be visible from the repo root) before writing any code. Heed deprecation notices.

This block is written and re-added by `next dev` — verify at `node_modules/next/dist/server/lib/generate-agent-files.js`. Removing it from a diff only re-creates the uncommitted change; committing it with your work keeps the tree clean.

<!-- END:nextjs-agent-rules -->

## Verification does not depend on GitHub CI

Since 2026-11-25 this repository does not use GitHub Actions for verification, nor for building, releasing or deploying (publishing GitHub Pages is the only exception). `.github/workflows/` may only hold a workflow that publishes GitHub Pages; do not add any other workflow.

- Run tests, checks and builds locally (or on a verification host through calltable `ct`) before pushing.
- Commit and push notes state the commands actually run and where; never write "CI passed" and do not wait for CI results.
- The remaining `.github/workflows/deploy.yml` only publishes GitHub Pages; its result is not verification evidence. `npm run deploy` publishes the same site locally.
