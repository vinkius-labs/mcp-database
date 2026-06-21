# Deep Diff Engine MCP Server

Find every single change between two JSON objects — additions, deletions, and edits with exact structural paths. Stop relying on AI to 'spot the difference'.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deep-diff-engine)

## Overview
**Category:** utilities
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Deep Diff Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deep-diff-engine](https://vinkius.com/mcp/deep-diff-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
