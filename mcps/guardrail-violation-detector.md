# Guardrail Violation Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/guardrail-violation-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

Analyzes AI agent outputs for safety and compliance violations.

## Description
This MCP server provides deterministic scoring for agent outputs to ensure safety and structural integrity. It evaluates responses against specific constraints like PII detection, toxicity, off-topic drift, length requirements, and format compliance. Using `analyze_output_violations`, agents can receive a composite violation score and severity level (Info, Warning, or Block) to decide whether to proceed with a response. It also provides access to the `get_guardrail_configuration` to retrieve active rules and `get_historical_false_positive_rate` to monitor system accuracy.


## Available Tools (3)
- **get_guardrail_configuration**: Retrieves the current active rules and their definitions
- **analyze_output_violations**: Performs a full audit of an agent response against a set of rules
- **get_historical_false_positive_rate**: Retrieves the accuracy metric for a specific guardrail rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guardrail Violation Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this response is safe: 'My phone number is 555-0199 and I am very angry!'"

**🤖 AI Agent:**
> The response is flagged as a Block due to PII detection and high toxicity scores.

---

**👤 You:**
> "Analyze the compliance of a response that is 500 words long when the target was 100."

**🤖 AI Agent:**
> The response has a high length violation score due to the significant deviation from the target length.

---

**👤 You:**
> "What are the current active guardrail rules?"

**🤖 AI Agent:**
> The active rules include PII detection, toxicity monitoring, off-topic detection, length constraints, and format validation.


## ❓ FAQ

**Q: How is the violation severity determined?**
Severity is based on the composite score: Info for scores below 0.2, Warning for 0.2 to 0.5, and Block for scores above 0.5. Additionally, any single rule exceeding 0.8 triggers a Block.

**Q: Can I see which rules are currently active?**
Yes, you can use the `get_guardrail_configuration` tool to retrieve the current list of active rules and their thresholds.

**Q: What happens if both PII and toxicity are detected?**
The system is designed to handle cascading violations; if both PII and toxicity are detected in the same output, the severity level is automatically escalated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/guardrail-violation-detector](https://vinkius.com/ai-agent-connect/guardrail-violation-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guardrail Violation Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `guardrail-violation-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guardrail Violation Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guardrail-violation-detector": {
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
