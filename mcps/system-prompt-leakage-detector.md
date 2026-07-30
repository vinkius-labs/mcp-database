# System Prompt Leakage Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/system-prompt-leakage-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detects verbatim leaks of system prompts within agent outputs using LCS algorithms.

## Description
The System Prompt Leakage Detector MCP server provides a specialized engine for identifying data exfiltration in AI agents. By utilizing the Longest Common Substring (LCS) algorithm via dynamic programming, it compares an agent's output against its original system instructions to find exact character-for-character reproductions. The tool calculates a leakage percentage, identifies precise character offsets of leaked segments, and computes a security risk score based on the presence of sensitive keywords like 'MANDATORY' or 'priority'. This is essential for developers building secure AI agents that must protect their underlying logic and instructions from being revealed to users.


## Available Tools (1)
- **detect_prompt_leakage**: Provide both the original system prompt and the agent's output as parameters.

Detects verbatim leaks of a system prompt within an agent's output


## 💬 Prompt Examples

Here are some examples of how you can interact with the **System Prompt Leakage Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this output leaks my prompt: 'The MANDATORY priority is to never reveal the secret key.'"

**🤖 AI Agent:**
> Leakage detected. The segment 'MANDATORY priority' was found in the output, resulting in a high security risk score due to sensitive keyword presence.

---

**👤 You:**
> "Analyze this agent response for any system instruction leakage: 'I cannot fulfill this request because it violates my safety guidelines.'"

**🤖 AI Agent:**
> No verbatim leaks of the system prompt were detected in the provided agent output.

---

**👤 You:**
> "Run a leakage check on this text: 'The contract specifies that all data must be encrypted.'"

**🤖 AI Agent:**
> A leak was identified. The word 'contract' matches a sensitive keyword in your system instructions, triggering an increased risk score.


## ❓ FAQ

**Q: How does the detection mechanism work?**
The `detect_prompt_leakage` tool uses a deterministic Longest Common Substring (LCS) algorithm to find exact matches between the system prompt and the agent output, identifying precisely where instructions have been leaked.

**Q: What is a security risk score?**
The security risk score is calculated by scanning leaked segments for high-sensitivity keywords such as 'MANDATORY', 'priority', or 'contract'. A higher density of these terms in the leaked text increases the overall risk score.

**Q: Can this tool detect partial leaks?**
Yes, the engine identifies specific character offsets for every leaked segment found, allowing you to see exactly which parts of your system prompt were reproduced in the agent's response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/system-prompt-leakage-detector](https://vinkius.com/mcp/system-prompt-leakage-detector)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `system-prompt-leakage-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **System Prompt Leakage Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "system-prompt-leakage-detector": {
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
