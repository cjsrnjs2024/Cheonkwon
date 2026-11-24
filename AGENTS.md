<!-- BEGIN:nextjs-agent-rules -->

## This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` (resolved from this file's directory; in monorepos the `next` package may not be visible from the repo root) before writing any code. Heed deprecation notices.

This block is written and re-added by `next dev` — verify at `node_modules/next/dist/server/lib/generate-agent-files.js`. Removing it from a diff only re-creates the uncommitted change; committing it with your work keeps the tree clean.

<!-- END:nextjs-agent-rules -->

## Product TODO

Before planning or implementing product features, read `TODO.md` and account for the recorded roadmap items.

## Automatic GitHub deployment

For natural-language requests that modify this repository, treat the request as authorization to deploy the completed change unless the user explicitly says to keep it local, make a draft, or not deploy.

After implementing a requested change:

1. Run the relevant tests, lint checks, and production build in proportion to the change.
2. Commit only the files that belong to the current request. Never include unrelated pre-existing changes, local environment files, credentials, secrets, or generated build artifacts.
3. Push the commit to `origin/main` without force-pushing. A successful push triggers the connected Vercel production deployment.
4. Report the commit hash, push result, and any verification failures to the user.

Do not deploy when validation reveals a material failure caused by the requested change. If the remote branch has advanced, integrate it safely without discarding local or remote work. Never rewrite shared history.
