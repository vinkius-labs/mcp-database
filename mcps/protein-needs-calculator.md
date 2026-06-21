# Protein Needs Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/protein-needs-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate your daily protein requirements based on weight, activity level, and goals.

## Description
The Protein Needs Calculator connects AI agents to precise nutritional science. By using tools like `calculate_total_protein_requirement`, users can determine their optimal daily protein intake in grams. The server considers body weight, physical activity intensity (from sedentary to highly active), fitness objectives (such as muscle gain or weight loss), and special physiological conditions like pregnancy or elderly status. This MCP allows for automated nutritional planning and feasibility checks using `check_protein_plan_feasibility`.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Protein Needs Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much protein do I need if I weigh 80kg, am moderately active, and want to gain muscle?"

**🤖 AI Agent:**
> Based on your weight of 80kg and moderate activity level, you should aim for approximately 128 grams of protein per day to support muscle gain.

---

**👤 You:**
> "Calculate protein for a 70kg person who is sedentary and focused on weight loss."

**🤖 AI Agent:**
> For a 70kg individual with a sedentary lifestyle focusing on weight loss, the recommended daily protein intake is 56 grams.

---

**👤 You:**
> "Is 100g of protein enough for an 85kg athlete?"

**🤖 AI Agent:**
> No, 100g is not sufficient. For an 85kg person with high activity levels, the requirement exceeds 100g.


## ❓ FAQ

**Q: How is the protein requirement calculated?**
The calculation starts with your body weight multiplied by an activity level multiplier, then adjusts for your fitness goal and adds any necessary grams for special conditions. Tools available: `your_tool_name`.

**Q: Can I check if my current protein intake is enough?**
Yes, you can use the `check_protein_plan_feasibility` tool to compare your target intake against your calculated physiological minimum.

**Q: What activity levels are supported?**
The tool supports Sedentary, Lightly Active, Moderately Active, and Highly Active intensity categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/protein-needs-calculator](https://vinkius.com/mcp/protein-needs-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Protein Needs Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `protein-needs-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Protein Needs Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protein-needs-calculator": {
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
