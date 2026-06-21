# Deep Diff Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deep-diff-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deep-diff-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deep-diff-engine-mcp)
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


## Installation & Usage

To install and use the **Deep Diff Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deep-diff-engine](https://vinkius.com/mcp/deep-diff-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
