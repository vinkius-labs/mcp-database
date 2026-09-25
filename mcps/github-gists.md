# GitHub Gists MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/github-gists)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage GitHub Gists: list public Gists, read files, and create, edit, fork and delete your Gists. Public reads work keyless; a token unlocks the full suite.

## Description
Turn any AI agent into a Gist power-user. Read shared code snippets, configs and scripts without setting up anything — then, with a single GitHub token, create, edit, fork and delete Gists on your own account.

### What you can do

- **Discover public Gists** — browse recently updated Gists across GitHub or a specific user's Gists, with no credential required
- **Read any file** — pull a whole Gist or a single file; files over 1 MB are streamed in full from their raw URL
- **Publish Gists** — create Gists from one or many files, secret by default or public on demand
- **Edit** — update files, description or visibility; remove files or clear their content in one call
- **Fork & manage** — fork a Gist to work on your own copy, or delete a Gist permanently

### How it works

1. Subscribe to this server
2. Leave the token empty to read public Gists keyless, or paste a GitHub token to unlock private Gists and all write operations
3. Ask your agent to find, read or publish Gists

The GITHUB_TOKEN credential is optional. Without it the server operates keyless (about 60 requests/hour per IP); with a token you get the full authenticated budget (about 5000 requests/hour) and access to your private Gists. Rate-limit responses are turned into clear retry hints.

### Who is this for?

- **Developers** — keep snippets, configs and notes as Gists and manage them from the agent
- **Platform/DevRel engineers** — surface shared code and docs snippets programmatically
- **Automation builders** — publish, version and distribute scripts through Gists


## Available Tools (8)
- **fork_gist**: Use when you want to modify or extend someone else's Gist without touching the original. Forking the same Gist twice is a conflict — fetch your fork from the user's Gist list instead.

Fork a Gist to your account so you can edit it independently. Requires a token
- **create_gist**: files_json maps file names to content: {"setup.py": {"content": "print(1)"}} — plain string values are accepted too. Gists default to secret; set public=true to publish. Needs a configured token (a missing one is reported as an error, not silently skipped). Confirm destructive or outbound actions with the user first.

Create a new Gist — publish code, snippets or configs to GitHub. Requires a token
- **delete_gist**: The Gist and all its files are gone; this is irreversible, so confirm with the user before calling. The token must own the Gist (forks of your own Gists cannot be deleted through the original).

Delete a Gist permanently. Requires a token — confirm before calling
- **get_gist**: Public Gists are readable without a credential; private Gists need a configured token that has access.

Fetch a single Gist with its files (public Gists work without a token)
- **list_user_gists**: With a configured token the call also returns the user's private Gists. Use to survey what a person or team has published. Paginate with limit (max 100) and page; direction "asc"/"desc" orders by update time.

List the Gists of a GitHub user (public without a token)
- **get_gist_file**: Small files come straight from the Gist payload; files over 1 MB are downloaded in full from their raw URL. Works without a token for public Gists; private Gists need a configured token. If you do not know the file names, call get_gist first — errors list the available files. Use the raw git URL from get_gist to clone Gists with files over 10 MB.

Read one file from a Gist as plain text
- **list_public_gists**: Use this to discover shared snippets, configs and scripts. Works without any credential, so keep calls modest when keyless. Paginate with limit (max 100) and page; direction "asc"/"desc" orders by update time; since filters to Gists updated after an ISO date. For a specific Gist call get_gist with its id.

List recently updated public Gists across GitHub (no token required)
- **update_gist**: files_json uses the same shape as create_gist; a null value removes the file and {} clears its content. At least one of files_json, description or public is required. The token must own or fork the Gist.

Edit an existing Gist: files, description or visibility. Requires a token


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitHub Gists** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recently updated public Gists and tell me what each one is about."

**🤖 AI Agent:**
> I listed the 10 most recently updated public Gists. They include a CI pipeline tweak, a Docker compose snippet, a SQL migration and a few Python utilities. The top ones: owner-a/abc… (Kubernetes config, updated today) and owner-b/def… (bash deploy script). Want me to open any of them in full?

---

**👤 You:**
> "Create a private Gist from this bash script with the description "deploy helper"."

**🤖 AI Agent:**
> I created a secret Gist "deploy helper" with your script (2.1 KB, deploy.sh). It is not public. You can make it public or add more files with update_gist whenever you like.

---

**👤 You:**
> "Fork this Gist so I can edit my own copy without touching the original."

**🤖 AI Agent:**
> I forked the Gist to your account (new id …). It has 4 files: main.py, config.json, README.md and test_main.py. You can now edit your copy — the original stays unchanged.


## ❓ FAQ

**Q: Do I need a GitHub token to use this?**
No. Public Gists can be listed, read and opened as files without any credential. A token is only required for your private Gists and for write operations (create, update, fork, delete).

**Q: What permissions does the token need?**
Only the "gist" permission — a classic personal access token with gist scope, or a fine-grained token with access to Gists. No repo access is required. Create the token under Settings > Developer settings > Personal access tokens.

**Q: Can I read large Gist files in full?**
Yes. The Gist payload includes up to 1 MB of content per file; get_gist_file transparently downloads larger files in full from their raw URL. For Gists whose files exceed 10 MB, clone them with the git URL (git_pull_url) returned by get_gist.

**Q: How does rate limiting work?**
Keyless (public reads) is limited to about 60 requests/hour per IP; with a token the budget is about 5000 requests/hour. When a limit is hit the tool returns a clear error with the time to wait and when the budget resets, instead of failing silently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/github-gists](https://vinkius.com/en/ai-agent-connect/github-gists)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitHub Gists** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `github-gists` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitHub Gists** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "github-gists": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
