# LLM Output Format Drift Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-output-format-drift-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

Detect structural deviations in LLM outputs against reference templates.

## Description
The LLM Output Format Drift Detector is a specialized comparison engine designed to ensure that AI-generated content adheres strictly to predefined structural patterns. By using deterministic string alignment, it analyzes markdown syntax and punctuation markers—such as headers, list styles, and bold text—to calculate a precise drift percentage. This tool is essential for developers building automated evaluation pipelines where the structural integrity of an LLM response is just as critical as its semantic content. You can use `calculate_drift_score` to quantify deviations, `detect_structural_anomalies` to find missing sections or altered list styles, and `verify_compliance_truth` to get a definitive pass/fail verdict based on your specific tolerance levels.


## Available Tools (3)
- **calculate_drift_score**: Quantify the degree of structural deviation as a percentage
- **detect_structural_anomalies**: Identify specific types of structural failures
- **verify_compliance_truth**: Defaults to zero-tolerance (0% drift).

Provide a definitive pass/fail verdict on structural integrity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM Output Format Drift Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this output matches my template: # Header
- Item 1"

**🤖 AI Agent:**
> The `calculate_drift_score` tool reports a drift percentage of 0.0%, indicating perfect structural alignment with your template.

---

**👤 You:**
> "Identify what is wrong with this markdown: # Title
1. First item"

**🤖 AI Agent:**
> The `detect_structural_anomalies` tool identified a list style mismatch: the template expected bulleted items, but found a numbered list.

---

**👤 You:**
> "Is this output compliant with a 5% drift threshold?"

**🤖 AI Agent:**
> The `verify_compliance_truth` tool returned isCompliant: true, as the actual drift score was 2.5%, which is within your allowed threshold.


## ❓ FAQ

**Q: What exactly is structural drift?**
Structural drift refers to the deviation of an LLM output's markdown structure from a reference template. This includes changes in header hierarchy, list markers (like switching from bullets to numbers), or unexpected punctuation.

**Q: How does the tool calculate the drift percentage?**
The `calculate_drift_score` tool uses deterministic string alignment to compare structural markers in your template against the actual output. The percentage is calculated as the ratio of mismatched or missing markers to the total number of elements found in the template.

**Q: Can I set a tolerance for compliance?**
Yes. When using `verify_compliance_truth`, you can provide an `allowedDriftThreshold`. If no threshold is specified, the tool defaults to a zero-tolerance policy.


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
