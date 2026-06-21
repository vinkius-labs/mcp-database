# JSON Diff Visualizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-diff-visualizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate human-readable visual diffs between two JSON objects — added lines in green, removed in red, unchanged in gray. Like 'git diff' but for JSON structures.

## Description
Your deployment pipeline just changed a config file. You need to review the changes before approving. The deep-diff engine gives you machine-readable change objects — but you need to show the diff to a human for approval.

This MCP generates visual, colorized diffs with `+` and `-` markers — the same format every developer reads in git. But for JSON structures, not file lines.

### The Superpowers

- **Visual Format:** Green `+` for additions, red `-` for removals — instantly scannable by humans.
- **Structural Awareness:** Diffs JSON by structure, not by text lines. Reordered keys don't show as changes.
- **Human Review Ready:** Output designed for Slack messages, PR comments, and approval workflows.
- **Complementary:** Use with deep-diff-engine for programmatic processing, json-diff-visualizer for human review.


## Available Tools
- **diff_json**: Pass two JSON strings and receive both a structural diff (machine-readable) and a visual diff (human-readable with + and - markers). Essential for CI/CD agents comparing config versions, deployment manifests, or database schema snapshots.

Generates structural and visual diffs between two JSON objects. Shows added, removed, and modified fields with exact paths


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Diff Visualizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a visual diff between our staging and production API configs so I can review before approving the deploy."

**🤖 AI Agent:**
> Visual diff with + (added), - (removed) markers. 3 changes highlighted for human review.

---

**👤 You:**
> "Post the JSON config changes to our Slack #deployments channel for team review."

**🤖 AI Agent:**
> ```diff
- "replicas": 2
+ "replicas": 3
``` Ready to paste into Slack.

---

**👤 You:**
> "Compare the old and new Terraform state files and show me what infrastructure changed."

**🤖 AI Agent:**
> Visual diff: 2 resources modified, 1 added, 0 destroyed.


## ❓ FAQ

**Q: How is this different from deep-diff-engine?**
deep-diff-engine returns structured change objects for programmatic processing (CI/CD pipelines, automated alerts). json-diff-visualizer returns human-readable text with +/- markers for visual review (Slack, PR comments, approval workflows). Use both together.

**Q: Does reordering keys show as a change?**
No. The diff is structural — {a:1,b:2} and {b:2,a:1} show zero differences because the data is semantically identical.

**Q: Can I use the output in Slack or GitHub PR comments?**
Yes. The output is plain text with +/- markers — paste directly into code blocks in Slack, GitHub, or any markdown-compatible platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-diff-visualizer](https://vinkius.com/mcp/json-diff-visualizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON Diff Visualizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `json-diff-visualizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON Diff Visualizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-diff-visualizer": {
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
