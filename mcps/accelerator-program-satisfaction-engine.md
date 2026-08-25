# Accelerator Program Satisfaction Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-program-satisfaction-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Analyzes accelerator program success through satisfaction scores, NPS, and module performance.

## Description
This MCP server provides a specialized analytical engine for accelerator programs to measure founder satisfaction. It synthesizes survey data to calculate an aggregate satisfaction score, computes Net Promoter Scores (NPS), and identifies specific curriculum areas needing improvement. Using tools like `calculate_overall_satisfaction`, `compute_nps`, and `identify_improvement_areas`, program managers can gain deep insights into cohort performance and adjust their curriculum based on data-driven feedback.


## Available Tools (3)
- **calculate_overall_satisfaction**: Determines the aggregate satisfaction level of the program
- **compute_nps**: Calculates the Net Promoter Score to gauge program loyalty
- **identify_improvement_areas**: Pinpoints specific curriculum or operational modules that are underperforming


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Program Satisfaction Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the overall satisfaction for the current survey data."

**🤖 AI Agent:**
> The overall satisfaction score is 85/100, with an average module rating of 8.2.

---

**👤 You:**
> "What is the NPS score for these responses: [9, 10, 5, 8, 10, 2, 7]?"

**🤖 AI Agent:**
> The Net Promoter Score is 28.6, with 3 Promoters, 1 Passive, and 2 Detractors.

---

**👤 You:**
> "Which modules need improvement if the threshold is 7.0? Ratings: {"mentorship": 8.5, "fundraising": 6.0, "product_dev": 7.5}"

**🤖 AI Agent:**
> The module requiring improvement is `fundraising` with a rating of 6.0.


## ❓ FAQ

**Q: How is the overall satisfaction score calculated?**
The score is a weighted synthesis of module ratings and outcome satisfaction, which can be adjusted for response bias using `calculate_overall_satisfaction`.

**Q: Can I segment the results by cohort?**
Yes, you can provide a `segmentId` to the `calculate_overall_satisfaction` tool to filter results for specific groups.

**Q: How does the system identify weak modules?**
By using `identify_improvement_areas`, the system flags any module whose rating falls below your specified threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-program-satisfaction-engine](https://vinkius.com/ai-agent-connect/accelerator-program-satisfaction-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Program Satisfaction Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-program-satisfaction-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Program Satisfaction Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-program-satisfaction-engine": {
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
