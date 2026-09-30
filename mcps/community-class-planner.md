# Community Class Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-class-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Manage enrollment, costs, and break-even analysis for community educational classes.

## Description
This MCP server provides essential financial and logistical tools for managing community-based educational programs. It allows users to calculate expected profit or loss using `calculate_class_financials`, determine the minimum number of students needed to cover costs with `determine_breakeven_point`, verify venue and instructor constraints via `validate_class_capacity`, and estimate material requirements with `get_material_budget`. It is designed to help organizers maintain financial stability and operational efficiency.


## Available Tools (4)
- **determine_breakeven_point**: 
- **validate_class_capacity**: 
- **calculate_class_financials**: 
- **get_material_budget**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Class Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected profit for a class with 20 students at $50 each, an instructor fee of $200, room rental of $150, and $10 material cost per student?"

**🤖 AI Agent:**
> The expected net profit for this class is $550.

---

**👤 You:**
> "How many students do I need to enroll to break even if the class price is $40, instructor fee is $100, room rental is $100, and material cost is $15 per student?"

**🤖 AI Agent:**
> You need to enroll 7 students to break even.

---

**👤 You:**
> "Is an enrollment of 35 students okay for a room with a capacity of 30?"

**🤖 AI Agent:**
> No, the enrollment exceeds the maximum room capacity.


## ❓ FAQ

**Q: How can I check if my class is profitable?**
You can use the `calculate_class_financials` tool by providing the class price, enrollment count, instructor fees, room rental, and material costs per student.

**Q: How do I know how many students I need to cover my costs?**
Use the `determine_breakeven_point` tool. It calculates the required enrollment based on your fixed costs and the margin per student.

**Q: Can I verify if my venue can accommodate the students?**
Yes, the `validate_class_capacity` tool checks your enrollment against both room capacity and instructor-to-student ratios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-class-planner](https://vinkius.com/en/ai-agent-connect/community-class-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Class Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-class-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Class Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-class-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
