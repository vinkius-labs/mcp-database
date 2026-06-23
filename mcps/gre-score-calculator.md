# GRE Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gre-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert raw GRE answers into scaled scores, percentiles, and check graduate program eligibility.

## Description
The GRE Score Calculator is a specialized tool for students preparing for graduate school. It bridges the gap between raw exam performance and official metrics. Using `calculate_scaled_scores`, you can transform your count of correct answers in Verbal Reasoning, Quantitative Reasoning, and Analytical Writing into their standardized scaled ranges (13/170 or 0/6). The tool also provides relative standing via `get_percentile_rank` by comparing your scores to historical distributions. Finally, use `check_program_eligibility` to see if your performance meets the minimum thresholds for specific academic tracks like STEM, Humanities, or Business.


## Available Tools (3)
- **calculate_scaled_scores**: Converts raw GRE correct answer counts into official scaled scores
- **check_program_eligibility**: Compares GRE scores against graduate program requirements
- **get_percentile_rank**: Determines the relative standing based on scaled GRE scores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GRE Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I got 30 correct in Verbal, 35 in Quant, and 4 in Writing. What are my scaled scores?"

**🤖 AI Agent:**
> Your scaled scores are: Verbal Reasoning: 150, Quantitative Reasoning: 155, and Analytical Writing: 4.0.

---

**👤 You:**
> "Am I eligible for a STEM program with a 155 Verbal, 165 Quant, and 4.0 Writing score?"

**🤖 AI Agent:**
> Yes, you are eligible for the STEM program track with these scores.

---

**👤 You:**
> "What is my percentile rank if I scored 160 in Verbal, 160 in Quant, and 5.0 in Writing?"

**🤖 AI Agent:**
> Your approximate percentiles are: Verbal Reasoning: 85%, Quantitative Reasoning: 85%, and Analytical Writing: 90%.


## ❓ FAQ

**Q: How do I convert my raw scores to scaled scores?**
You can use the `calculate_scaled_scores` tool. Simply provide the number of correct answers you achieved in the Verbal, Quantitative, and Analytical Writing sections.

**Q: Can I check if my scores meet program requirements?**
Yes, use the `check_program_eligibility` tool. Input your scaled scores and select a program type such as STEM, Humanities, or Business to see if you meet the minimum thresholds.

**Q: What does the percentile rank represent?**
The `get_percentile_rank` tool calculates your relative standing by comparing your scaled scores against historical ETS distribution data, showing the percentage of test-takers you scored at or above.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gre-score-calculator](https://vinkius.com/mcp/gre-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GRE Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gre-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GRE Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gre-score-calculator": {
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
