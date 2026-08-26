# Hallucination Detector via Consistency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hallucination-detector-via-consistency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reliability](../categories/reliability.md)

Detect factual contradictions across multiple LLM responses to identify potential hallucinations.

## Description
This MCP server provides a suite of tools to verify the reliability of LLM outputs by checking for factual consistency. By analyzing multiple responses to the same query, it uses deterministic claim extraction to identify conflicting dates, numbers, or entities. Use `analyze_consistency` to get a high-level report, `extract_claims` to break down specific assertions, or `find_contradictions` to pinpoint logical conflicts between sets of claims.


## Available Tools (3)
- **analyze_consistency**: Evaluates a set of LLM responses to determine if they are factually consistent
- **extract_claims**: Decomposes text into individual factual assertions
- **find_contradictions**: Compares sets of claims to identify logical conflicts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hallucination Detector via Consistency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these responses are consistent: ['The event happened in 2021.', 'The event occurred in 2022.']"

**🤖 AI Agent:**
> The responses are inconsistent. The event date is contradictory (2021 vs 2022).

---

**👤 You:**
> "Extract the factual claims from: 'The population is 5 million and the capital is Paris.'"

**🤖 AI Agent:**
> The extracted claims are: population is 5 million, capital is Paris.

---

**👤 You:**
> "Are these responses consistent? ['The price is $10.', 'The price is $10.']"

**🤖 AI Agent:**
> Yes, the responses are consistent.


## ❓ FAQ

**Q: How does the consistency score work?**
The score is calculated by subtracting the ratio of unique contradictions to the total number of extracted claims from 1.0. A score of 1.0 means perfect agreement.

**Q: What can I do with `analyze_consistency`?**
You can use `analyze_consistency` to pass a list of multiple LLM responses and receive a report containing a consistency score and indices of suspect responses.

**Q: Can I customize the strictness of the detection?**
Yes, you can provide a custom threshold value to `analyze_consistency` to define when a set of responses should be flagged as inconsistent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hallucination-detector-via-consistency](https://vinkius.com/ai-agent-connect/hallucination-detector-via-consistency)
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
