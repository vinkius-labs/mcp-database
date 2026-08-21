# Job-Hop ROI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/job-hop-roi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze the financial and career impact of switching jobs in Singapore.

## Description
A deterministic financial analysis tool for Singaporean professionals to evaluate the ROI of a new job offer. Use `calculate_immediate_roi` to find your salary jump and annual gain, `calculate_break_even_period` to see how quickly you recover transition costs, `assess_career_timing` to evaluate your tenure, and `project_five_year_wealth` to compare long-term earnings growth.


## Available Tools (4)
- **assess_career_timing**: Assess career growth timing based on tenure
- **calculate_break_even_period**: Calculate the time required to recover transition costs
- **calculate_immediate_roi**: Calculate immediate financial gain and salary jump
- **project_five_year_wealth**: Project cumulative wealth difference over five years


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Job-Hop ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I currently earn 8000 SGD and have a new offer for 10000 SGD with a 2000 SGD signing bonus. What is my immediate ROI?"

**🤖 AI Agent:**
> Your salary increment is 25% and your total annual gain is 26,000 SGD.

---

**👤 You:**
> "If I have 3 years of tenure at my current company, is it a good time to move?"

**🤖 AI Agent:**
> Your career growth score is Optimal.

---

**👤 You:**
> "It will cost me 5000 SGD to relocate for a new job that pays 1000 SGD more per month. How long to break even?"

**🤖 AI Agent:**
> It will take 5 months to break even.


## ❓ FAQ

**Q: How do I calculate my immediate salary increase?**
You can use the `calculate_immediate_roi` tool by providing your current salary, the new offer salary, and any signing bonus.

**Q: Can I estimate my long-term wealth difference?**
Yes, the `project_five_year_wealth` tool compares the cumulative earnings of staying at your current job versus moving to the new role over a five-year period.

**Q: What determines if my career timing is optimal?**
The `assess_career_timing` tool evaluates your tenure. It labels timing as 'Good Timing' if you have less than 2 years, 'Optimal' for 2-4 years, and 'Overdue' if you have been there for more than 4 years.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/job-hop-roi-calculator](https://vinkius.com/ai-agent-connect/job-hop-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Job-Hop ROI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `job-hop-roi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Job-Hop ROI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "job-hop-roi-calculator": {
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
