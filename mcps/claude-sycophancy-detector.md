# Claude Sycophancy Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claude-sycophancy-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detects when AI models agree with incorrect user assumptions by verifying factual claims against codebase metadata.

## Description
The Claude Sycophancy Detector is a diagnostic tool designed to identify sycophantic behavior in AI models. Sycophancy occurs when an AI prioritizes user agreement over factual accuracy, often validating incorrect assumptions or non-existent code structures. This MCP server provides tools to extract factual claims--such as file paths, function signatures, and variable names--from an AI response and validate them against a provided ground truth codebase metadata. By using `analyze_response_accuracy`, users can calculate a factual accuracy ratio and a sycophancy risk score. The `extract_claims_from_text` tool isolates specific assertions, while `get_sycophancy_risk_summary` provides human-readable risk levels and actionable recommendations. This tool is essential for ensuring the reliability of AI-driven code analysis in Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (3)
- **analyze_response_accuracy**: Evaluates the factual integrity of an AI response by comparing its claims against the provided codebase facts
- **extract_claims_from_text**: Isolates potential factual assertions from a block of text using deterministic extraction rules
- **get_sycophancy_risk_summary**: Provides a high-level interpretation of the risk score and detected patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Sycophancy Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the function `processData()` located in `src/utils.ts`?"

**🤖 AI Agent:**
> No, the `processData()` function is actually located in `src/handlers/dataHandler.ts`.

---

**👤 You:**
> "You're right, the variable `user_id` is defined in `config.json`."

**🤖 AI Agent:**
> Actually, `user_id` is not defined in `config.json`; it is defined in `src/auth/session.ts`.

---

**👤 You:**
> "Can you check if `validate_input` exists in the current codebase?"

**🤖 AI Agent:**
> The `validate_input` function does not exist in the current codebase.


## ❓ FAQ

**Q: What is sycophancy in AI?**
Sycophancy is when an AI model agrees with a user's incorrect statement or assumption to avoid conflict, rather than providing the correct factual information.

**Q: How does `analyze_response_accuracy` work?**
The `analyze_response_accuracy` tool uses deterministic regex to extract claims like file paths and function signatures from a response, then compares them against the provided `codebaseFacts` to determine accuracy.

**Q: Which AI clients can use this tool?**
This tool can be used with any MCP-compatible client, including Cursor, VS Code, Claude Desktop, and Windsurf.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claude-sycophancy-detector](https://vinkius.com/mcp/claude-sycophancy-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Sycophancy Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-sycophancy-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Sycophancy Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-sycophancy-detector": {
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
