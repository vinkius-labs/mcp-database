# Deep Diff Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deep-diff-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Find every single change between two JSON objects — additions, deletions, and edits with exact structural paths. Stop relying on AI to 'spot the difference'.

## Description
You pass two Kubernetes configs to an AI and ask what changed. It says 'The replica count increased' but completely misses that a critical security label was deleted deep in the spec. When the AI says 'they look the same', this engine proves otherwise.

This MCP uses `deep-diff` (1M+ weekly downloads) to compute exact structural differences between any two JSON objects or arrays. It returns machine-readable edit paths that agents can use to generate patch files, trigger alerts, or validate deployments.

### The Superpowers

- **Exact Edit Paths:** Get the exact property path (e.g., `spec.template.metadata.labels.env`) where a change occurred.
- **Change Types:** Accurately classifies changes as Additions (N), Deletions (D), or Edits (E).
- **Array Aware:** Detects items added or removed from deep nested arrays.
- **Structural Fidelity:** Ignores formatting and whitespace. Only alerts on real data changes.


## Available Tools
- **calculate_json_diff**: Calculate structural differences between two JSON objects. Returns an array of changes (add, edit, delete) with exact paths


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deep Diff Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the staging database config with the production config and list the exact paths that differ."

**🤖 AI Agent:**
> Differences found: 1 Edit (host URL), 1 Addition (readReplica node).

---

**👤 You:**
> "Our CI pipeline blocked a deployment. Run a deep diff on the modified IAM policy JSON to see what permissions were added."

**🤖 AI Agent:**
> Diff: New item added to 'Statement[0].Action' array: 's3:DeleteBucket'.

---

**👤 You:**
> "Check if there is any semantic difference between these two large API response payloads."

**🤖 AI Agent:**
> No structural differences found. The payloads are semantically identical.


## ❓ FAQ

**Q: Why shouldn't I just use string comparison?**
String comparison fails if the keys are reordered (e.g., `{"a":1,"b":2}` vs `{"b":2,"a":1}`). This engine understands JSON structure, so it correctly identifies that reordered keys are not semantic changes.

**Q: What do the 'kind' letters mean in the output?**
'N' means a newly added property. 'D' means a deleted property. 'E' means an edited/changed property. 'A' means a change occurred within an array.

**Q: Can this be used for config drift detection?**
Absolutely. Agents can fetch the desired state from Git, fetch the actual state from the live API, and use this engine to generate a list of exact properties that have drifted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deep-diff-engine](https://vinkius.com/mcp/deep-diff-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deep Diff Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deep-diff-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deep Diff Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deep-diff-engine": {
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
