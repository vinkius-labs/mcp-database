# Silent Change Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/silent-change-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Identifies unauthorized or unrequested code modifications by comparing file state snapshots.

## Description
Silent Change Detector monitors AI agent execution cycles to identify unauthorized or unrequested code modifications. By capturing a cryptographic SHA-256 state snapshot before an agent turn and comparing it to the state after, it classifies changes as intended, cascading, or unintended. This tool helps users detect 'silent' changes where agents refactor code or align with outdated documentation without explicit permission. Use `snapshot_state` to establish a baseline, `detect_changes` to classify modifications, and `analyze_documentation_drift` to find discrepancies between code and documentation.


## Available Tools (3)
- **analyze_documentation_drift**: Detects if code was modified to align with incorrect or outdated documentation
- **detect_changes**: Compares a previous snapshot against the current state to identify changes and their relation to user intent
- **snapshot_state**: Captures the current state of the workspace to establish a baseline for comparison


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Silent Change Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a snapshot of my current workspace."

**🤖 AI Agent:**
> Snapshot created successfully with ID: snap_12345.

---

**👤 You:**
> "Check if any unintended changes were made after my last instruction to fix the typo in main.ts."

**🤖 AI Agent:**
> No unintended changes detected. The only modification was in main.ts, which matches your request.

---

**👤 You:**
> "Did the agent change any code to match the outdated documentation in docs/api.md?"

**🤖 AI Agent:**
> Drift detected in src/utils.ts. The agent modified the logic to match the outdated documentation provided.


## ❓ FAQ

**Q: What is a silent change?**
A silent change is any modification categorized as unintended or any change that occurs without a corresponding instruction in the user's prompt.

**Q: How does the tool classify changes?**
Changes are classified into three types: Intended (direct goal), Cascading (necessary side effects), and Unintended (unrequested refactors or rogue changes).

**Q: Which files are monitored?**
The system only monitors files that are actively tracked by Git to avoid noise from build artifacts or local environment files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/silent-change-detector](https://vinkius.com/mcp/silent-change-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Silent Change Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `silent-change-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Silent Change Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "silent-change-detector": {
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
