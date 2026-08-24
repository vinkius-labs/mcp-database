# Accelerator Application Quality Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-application-quality-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

A diagnostic engine to evaluate startup accelerator applications.

## Description
This MCP server provides a diagnostic engine for evaluating startup accelerator applications. It uses a specialized scoring algorithm to assess core business metrics including problem clarity, solution uniqueness, team completeness, traction evidence, and market size validation. Using `calculate_application_score`, agents can generate comprehensive reports including a quality score, identified weak areas, and strategic improvement recommendations. Additionally, `get_dimension_benchmarks` allows for checking performance thresholds, while `compare_applications` enables ranking multiple startups to assist in shortlisting processes.


## Available Tools (3)
- **compare_applications**: Evaluates the relative quality of multiple applications to assist in ranking or shortlisting
- **calculate_application_score**: Provides a comprehensive quantitative and qualitative assessment of a single accelerator application
- **get_dimension_benchmarks**: Retrieves the threshold values used to define "weak" versus "strong" performance for each dimension


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Application Quality Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate this startup: Problem clarity is 8, solution uniqueness is 7, team completeness is 90%, traction is 5, market size is 8, and the application is complete."

**🤖 AI Agent:**
> The startup has a quality score of 76/100. The main weak area is traction evidence. To improve, the startup should focus on providing more quantifiable proof of market interest, such as user growth or revenue.

---

**👤 You:**
> "Compare these two applications: App A has a score of 85 and App B has a score of 72."

**🤖 AI Agent:**
> App A is ranked 1st and App B is ranked 2nd. The average score is 78.5 with a score spread of 13.

---

**👤 You:**
> "What is the threshold for a strong performance in traction?"

**🤖 AI Agent:**
> The threshold for traction is a score of 7 or higher to avoid being flagged as a weak area.


## ❓ FAQ

**Q: How is the quality score calculated?**
The score is an aggregate of all input dimensions. If `isApplicationComplete` is false, the final score is heavily penalized to reflect the lack of evidentiary support.

**Q: Can I compare multiple startup applications at once?**
Yes, you can use the `compare_applications` tool to evaluate the relative quality of multiple applications, providing a rank list, average score, and score spread.

**Q: What happens if a dimension score is low?**
If a dimension falls below the threshold defined in `get_dimension_benchmarks`, it will be flagged as a weak area, and the tool will provide specific improvement recommendations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-application-quality-score](https://vinkius.com/ai-agent-connect/accelerator-application-quality-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Application Quality Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-application-quality-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Application Quality Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-application-quality-score": {
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
