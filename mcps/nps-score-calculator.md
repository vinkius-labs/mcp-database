# NPS Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nps-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Calculate Net Promoter Score, performance tiers, and statistical margin of error.

## Description
The NPS Score Calculator MCP server provides a complete toolkit for analyzing customer loyalty. Use `calculate_nps` to transform raw response counts into a meaningful Net Promoter Score, including performance classifications (Critical, OK, Good, Excellent) and statistical margin of error. You can also use `get_industry_benchmark` to find standard targets for sectors like Technology or Retail, and `compare_performance` to see how your results stack up against the industry baseline.


## Available Tools
- **get_industry_benchmark**: Retrieves the NPS benchmark for a specific industry
- **calculate_nps**: Calculates Net Promoter Score (NPS) and statistical margin of error
- **compare_performance**: Compares current NPS against industry benchmark


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NPS Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my NPS score from these responses: 10 people gave a 10, 5 people gave a 9, 2 people gave an 8, and 3 people gave a 5."

**🤖 AI Agent:**
> Your NPS score is 60. This falls into the 'Good' classification, with a total of 20 responses and a calculated margin of error.

---

**👤 You:**
> "What is the benchmark for the Retail industry?"

**🤖 AI Agent:**
> The standard NPS benchmark for the Retail industry is 30.

---

**👤 You:**
> "Compare an NPS of 45 in the Technology sector to the industry standard."

**🤖 AI Agent:**
> Your NPS of 45 is 15 points above the Technology industry benchmark of 30.


## ❓ FAQ

**Q: How do I calculate my NPS score?**
Use the `calculate_nps` tool by providing a JSON object where keys are scores (0-10) and values are the number of responses for each score.

**Q: What industries are supported for benchmarking?**
The server includes hardcoded benchmarks for Technology, Retail, Hospitality, Finance, and Healthcare.

**Q: Does the tool provide statistical confidence?**
Yes, the `calculate_nps` tool automatically computes the statistical margin of error based on your sample size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nps-score-calculator](https://vinkius.com/mcp/nps-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NPS Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nps-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NPS Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nps-score-calculator": {
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
