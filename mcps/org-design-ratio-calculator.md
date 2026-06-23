# Org Design Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/org-design-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Analyze organizational efficiency by comparing headcount ratios against industry benchmarks.

## Description
This MCP server provides a quantitative analysis engine for identifying structural gaps in scaleup organizations. By using tools like `evaluate_span_of_control`, `evaluate_gtm_efficiency`, `evaluate_cs_coverage`, and `evaluate_ga_overhead`, leaders can compare their current headcount distribution against established SaaS industry benchmarks (such as SaaStr and Bain). It helps identify management bloat, engineering-to-sales imbalances, insufficient customer success coverage, or excessive G&A overhead.


## Available Tools (4)
- **evaluate_span_of_control**: Determine if the current manager-to-IC ratio is healthy
- **evaluate_cs_coverage**: Verify if CS headcount is sufficient for the customer segment
- **evaluate_ga_overhead**: Monitor G&A growth relative to total headcount
- **evaluate_gtm_efficiency**: Assess Engineering vs Sales balance based on GTM motion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Org Design Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our company has 10 managers and 70 individual contributors. Is our span of control healthy?"

**🤖 AI Agent:**
> Your current ratio is 7.0, which falls within the optimal range of 6 to 8.

---

**👤 You:**
> "We have 50 engineers and 20 sales reps using a PLG motion. How is our efficiency?"

**🤖 AI Agent:**
> Your current Engineering-to-Sales ratio is 2.5, with a benchmark gap of -0.5 compared to the PLG standard.

---

**👤 You:**
> "We have 5 CS managers for 200 Enterprise customers. Are we under-resourced?"

**🤖 AI Agent:**
> Your ratio is 40 customers per CSM. This is below the benchmark for the Enterprise segment, indicating you are likely overburdened.


## ❓ FAQ

**Q: What is the ideal manager-to-IC ratio?**
The target range for high-performing scaleups is typically between 6 and 8 individual contributors per manager.

**Q: How does GTM motion affect headcount benchmarks?**
Different motions require different balances. For example, a PLG motion favors higher engineering density compared to an Enterprise motion which requires more sales presence.

**Q: Can I check for excessive G&A overhead?**
Yes, the `evaluate_ga_overhead` tool checks if your G&A headcount as a percentage of total workforce exceeds industry thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/org-design-ratio-calculator](https://vinkius.com/mcp/org-design-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Org Design Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `org-design-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Org Design Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "org-design-ratio-calculator": {
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
