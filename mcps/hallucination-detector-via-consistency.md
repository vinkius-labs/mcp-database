# Hallucination Detector via Consistency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hallucination-detector-via-consistency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reliability](../categories/reliability.md)

Detects factual contradictions across multiple LLM responses to identify potential hallucinations.

## Description
This MCP server provides a diagnostic suite for evaluating the reliability of Large Language Model outputs. By analyzing multiple responses to the same query, it identifies factual inconsistencies that signal potential hallucinations. The system uses deterministic extraction to isolate dates, numbers, and entities, then performs logical comparisons to find contradictions. Use `analyze_consistency` to get a high-level reliability score, `extract_claims` to break down text into verifiable atoms, or `identify_contradictions` to pinpoint specific logical conflicts between claims.


## Available Tools (3)
- **extract_claims**: Decomposes raw text into individual, verifiable factual atoms
- **analyze_consistency**: Performs the primary evaluation of multiple LLM responses to determine if they agree on the facts
- **identify_contradictions**: Compares a set of claims to find logical conflicts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hallucination Detector via Consistency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these three responses about the launch date of Apollo 11 are consistent: 1. Apollo 11 launched on July 16, 1969. 2. The Apollo 11 mission began on July 16, 1969. 3. Apollo 11 was launched on July 17, 1969."

**🤖 AI Agent:**
> The responses are inconsistent. The third response claims a launch date of July 17, 1969, which contradicts the first two responses stating July 16, 1969.

---

**👤 You:**
> "Extract the factual claims from this text: 'The company was founded in 2010 and has 500 employees.'"

**🤖 AI Agent:**
> The extracted claims are: Date: 2010, Number: 500.

---

**👤 You:**
> "Are these responses consistent? 1. The capital of France is Paris. 2. Paris is the capital of France."

**🤖 AI Agent:**
> Yes, the responses are consistent.


## ❓ FAQ

**Q: How does the tool detect hallucinations?**
It uses `analyze_consistency` to compare multiple LLM responses. If the responses provide conflicting dates, numbers, or entities, the consistency score drops, flagging the output as potentially unreliable.

**Q: What kind of data can be extracted?**
The `extract_claims` tool specifically targets dates, numeric values, and named entities to ensure the analysis remains deterministic and verifiable.

**Q: Can I adjust the sensitivity of the detection?**
Yes, when using `analyze_consistency`, you can provide a custom threshold to make the detection more strict or more lenient.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hallucination-detector-via-consistency](https://vinkius.com/mcp/hallucination-detector-via-consistency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hallucination Detector via Consistency** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hallucination-detector-via-consistency` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hallucination Detector via Consistency** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hallucination-detector-via-consistency": {
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
