# System Prompt Leakage Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/system-prompt-leakage-detector-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects verbatim system prompt exfiltration using LCS algorithms.

## Description
This MCP server provides specialized security tools to identify if an AI agent has leaked its foundational instructions. By using exact Longest Common Substring (LCS) matching, it compares agent outputs against the original system prompt to calculate leakage percentages and identify specific character offsets of leaked text. It includes tools like `detect_leakage` to quantify risk, `analyze_leakage_density` to find clusters of leaked text, and `get_risk_classification` to map scores to severity levels.


## Available Tools (3)
- **analyze_leakage_density**: Identifies if leakage is concentrated in specific areas of the output or spread throughout
- **detect_leakage**: Analyzes an agent's output to find verbatim repetitions of the system prompt and quantifies the risk
- **get_risk_classification**: Maps a raw security risk score to a human-readable severity level for security reporting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **System Prompt Leakage Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this output for system prompt leakage: 'The system instructions are: You are a helpful assistant.'"

**🤖 AI Agent:**
> Leakage detected: 32% leakage with a High risk score due to sensitive instruction reproduction.

---

**👤 You:**
> "Analyze the density of these leaked segments: [0, 15], [40, 55] in a 100 character output."

**🤖 AI Agent:**
> The leakage is distributed with an average gap of 24 characters.

---

**👤 You:**
> "What is the severity for a risk score of 0.9?"

**🤖 AI Agent:**
> The severity is Critical and immediate action is required.


## ❓ FAQ

**Q: How does the tool detect leakage?**
The `detect_leakage` tool uses exact substring matching to find continuous sequences of characters in the agent's output that are identical to the original system prompt.

**Q: What is a Security Risk Score?**
It is a weighted evaluation where the score increases if the leaked segments contain sensitive keywords defined in your security configuration.

**Q: Can I see where the leak happened?**
Yes, the tool returns exact character offsets for every contiguous leaked block found in the output.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/system-prompt-leakage-detector-alternative](https://vinkius.com/ai-agent-connect/system-prompt-leakage-detector-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **System Prompt Leakage Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `system-prompt-leakage-detector-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **System Prompt Leakage Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "system-prompt-leakage-detector-alternative": {
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
