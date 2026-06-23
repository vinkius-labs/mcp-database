# StackPath (Edge Computing & CDN API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stackpath-edge-computing-cdn-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage edge computing workloads and CDN delivery via StackPath — list stacks, deploy workloads, and purge cached content directly from any AI agent.

## Description
Connect your **StackPath** account to any AI agent to orchestrate edge infrastructure and content delivery through natural conversation.

### What you can do

- **Stack Management** — List and organize your logical containers (stacks) across the global edge network using `list_stacks`.
- **CDN Operations** — Create new CDN sites and purge cached content instantly with `create_cdn_site` and `purge_content` to ensure your users see the latest updates.
- **Edge Computing** — Deploy and monitor containerized or VM workloads at the edge for low-latency performance using `create_workload` and `list_workloads`.
- **Infrastructure Visibility** — Query active workloads and site configurations without logging into the portal via `list_cdn_sites`.

### How it works

1. Subscribe to this server
2. Enter your StackPath Client ID and Client Secret
3. Start managing your edge infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate CDN purges and workload deployments directly from the terminal or chat.
- **Full-stack Developers** — check the status of edge containers without breaking focus from the code editor.
- **SRE Teams** — quickly list and inspect infrastructure stacks during incident response.


## Available Tools (6)
- **create_cdn_site**: Create a new CDN site
- **create_workload**: Create a new edge workload
- **list_cdn_sites**: List CDN sites in a stack
- **list_stacks**: List all StackPath stacks
- **list_workloads**: List edge workloads in a stack
- **purge_content**: Purge CDN content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StackPath (Edge Computing & CDN API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my StackPath stacks."

**🤖 AI Agent:**
> I've retrieved your stacks. You have 2 active stacks: 'Production-Edge' (ID: st-12345) and 'Staging-Global' (ID: st-67890).

---

**👤 You:**
> "Purge the cache for https://example.com/logo.png in stack st-12345."

**🤖 AI Agent:**
> The purge request for 'https://example.com/logo.png' has been successfully submitted to stack st-12345.

---

**👤 You:**
> "List all CDN sites in stack st-12345."

**🤖 AI Agent:**
> I found 1 CDN site in stack st-12345: 'www.example.com' pointing to origin 'origin.example.com'.


## ❓ FAQ

**Q: How do I clear the CDN cache for specific assets?**
You can use the `purge_content` tool. Provide the `stack_id` and a list of `urls` you want to invalidate. You can also set `recursive` to true to purge entire directories.

**Q: Can I deploy a new container to the edge using this agent?**
Yes! Use the `create_workload` tool. You'll need to specify the `stack_id`, a `name`, `slug`, and the container `image` (e.g., 'nginx:latest').

**Q: How do I find the ID of my infrastructure stacks?**
Simply run the `list_stacks` tool. It will return all logical stacks associated with your account along with their unique IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stackpath-edge-computing-cdn-api](https://vinkius.com/mcp/stackpath-edge-computing-cdn-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StackPath (Edge Computing & CDN API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stackpath-edge-computing-cdn-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StackPath (Edge Computing & CDN API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stackpath-edge-computing-cdn-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
