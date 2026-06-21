# JSON Diff Visualizer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-diff-visualizer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/json-diff-visualizer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/json-diff-visualizer-mcp)
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


## Installation & Usage

To install and use the **JSON Diff Visualizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-diff-visualizer](https://vinkius.com/mcp/json-diff-visualizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
