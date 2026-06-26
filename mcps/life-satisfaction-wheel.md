# Life Satisfaction Wheel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/life-satisfaction-wheel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify and analyze balance across essential life dimensions.

## Description
The Life Satisfaction Wheel MCP provides a diagnostic framework to evaluate how well you are balancing different sectors of your existence. By using tools like `compute_global_satisfaction`, `get_critical_area`, and `measure_imbalance_degree`, you can transform raw ratings into actionable insights about your stability and well-being.


## Available Tools (3)
- **identify_critical_area**: Identify the life dimension with the lowest satisfaction score
- **measure_imbalance**: Calculate the degree of imbalance between life dimensions
- **calculate_global_satisfaction**: Calculate the average satisfaction score across all life dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Life Satisfaction Wheel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my global satisfaction score for these ratings: {"Career": 80, "Health": 70, "Finance": 60, "Relationships": 90, "Leisure": 50, "Spirituality": 75}."

**🤖 AI Agent:**
> Your global satisfaction score is 70.83.

---

**👤 You:**
> "Which area of my life is most critical based on these scores: {"Career": 40, "Health": 90, "Finance": 85}."

**🤖 AI Agent:**
> The most critical area is Career.

---

**👤 You:**
> "How much imbalance is there in my life with these ratings: {"Career": 10, "Health": 95}."

**🤖 AI Agent:**
> The imbalance index is 85.


## ❓ FAQ

**Q: What is the Life Satisfaction Wheel?**
It is an analytical tool used to quantify balance across key life dimensions like career, health, and finance.

**Q: How do I use the tools?**
Provide a JSON object containing scores (0-100) for various life dimensions to tools like `compute_global_satisfaction`.

**Q: What does the imbalance index represent?**
It measures the gap between your highest and lowest performing life areas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/life-satisfaction-wheel](https://vinkius.com/mcp/life-satisfaction-wheel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Life Satisfaction Wheel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `life-satisfaction-wheel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Life Satisfaction Wheel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "life-satisfaction-wheel": {
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
