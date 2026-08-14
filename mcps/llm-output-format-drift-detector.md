# LLM Output Format Drift Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-output-format-drift-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Quantifies structural deviations in LLM responses by comparing exact syntax and markdown hierarchies against a reference template.

## Description
This MCP server provides specialized tools to measure how much an LLM's output deviates from a target structural blueprint. By using deterministic string alignment, it identifies 'Structural Drift'--differences in markdown headers, list styles, and punctuation--without being distracted by semantic meaning. Use `calculate_drift_score` to get a precise percentage of divergence, `validate_format_compliance` for a binary pass/fail verdict based on a tolerance threshold, and `analyze_structural_anomalies` to pinpoint specific failures like broken markdown hierarchies or missing sections.


## Available Tools (3)
- **validate_format_compliance**: Provides a strict pass/fail verdict on whether an output matches the required structural blueprint
- **analyze_structural_anomalies**: Identifies specific types of structural failures such as broken markdown hierarchies or inconsistent list styles
- **calculate_drift_score**: Computes the numerical degree of structural divergence between a generated output and a reference template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM Output Format Drift Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this output matches my template."

**🤖 AI Agent:**
> The output is compliant with a drift percentage of 0.0.

---

**👤 You:**
> "What structural issues are in this response?"

**🤖 AI Agent:**
> The analysis detected `hasHeaderDrift` and `hasListStyleDrift` due to inconsistent markdown usage.

---

**👤 You:**
> "Calculate the drift score for this text."

**🤖 AI Agent:**
> The structural drift is 15.5% with 85 alignment points.


## ❓ FAQ

**Q: Does this tool check the meaning of the text?**
No. This tool focuses exclusively on structural drift, such as markdown headers and list markers, rather than semantic content.

**Q: How is the drift percentage calculated?**
The `calculate_drift_score` tool uses deterministic string alignment to compare the target output against the reference template, measuring the proportion of structural mismatches.

**Q: Can I set a custom tolerance for compliance?**
Yes, when using `validate_format_compliance`, you can provide a `toleranceThreshold` between 0.0 and 1.0 to define your acceptable drift limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-output-format-drift-detector](https://vinkius.com/mcp/llm-output-format-drift-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM Output Format Drift Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-output-format-drift-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM Output Format Drift Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-output-format-drift-detector": {
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
