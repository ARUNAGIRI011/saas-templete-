# Framer Agent in GitHub Actions

## What the workflow does

The workflow at `.github/workflows/framer-agent-setup.yml`:

1. Starts an ephemeral Ubuntu GitHub Actions runner.
2. Installs Node.js 24.
3. Runs the official Framer setup command: `npx --yes @framer/agent@latest setup`.
4. Checks that skill files were installed under the runner's agent skill directories.

Run it manually from **Actions → Install Framer Agent skills → Run workflow**, or let it run when the Framer setup files change on `main`.

## Important limitation: installation is not project authorization

GitHub Actions runners are temporary. The installed skills disappear when the job ends. The workflow installs and verifies the Framer Agent setup; it does not keep an authenticated Framer session.

Framer's external-agent setup requires a user to connect a project and approve access in a browser. Do not put a personal Framer password, browser cookie, or OAuth session export in GitHub Secrets.

For a durable, interactive Framer editing connection, use Framer MCP from a supported agent client and authorize it with your Framer account. Framer's MCP endpoint is:

`https://mcp.framer.com/mcp`

Framer currently recommends MCP for most new connections. The local `@framer/agent` CLI remains supported, including workflows that use its installed skills.

## What this workflow does not do

- It does not run an autonomous LLM agent. GitHub Actions is the CI runner; an agent runtime/model must be separately configured.
- It does not authenticate to or modify a Framer project.
- It does not publish a Framer site.
- It does not store Framer credentials.

After the setup job passes, use a connected Framer MCP/External Agent client with the target Framer project link to create or edit the native Framer pages and CMS.
