# Knitting Yarn Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/knitting-yarn-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate yarn requirements, ball counts, and leftover length for knitting projects.

## Description
This MCP server provides essential tools for knitters to plan their projects accurately. By providing row counts, stitches per row, and yarn usage per stitch, you can use `get_yarn_requirements` to determine exactly how many balls of yarn to purchase and how much will be left over. You can also use `validate_project_feasibility` to ensure your project stays within realistic yarn consumption limits, `get_yarn_consumption_summary` for a detailed breakdown of total stitches and length, or `compare_yarn_options` to find the most efficient yarn ball size to minimize waste.


## Available Tools (4)
- **compare_yarn_options**: Determines which of two different yarn ball options is more efficient (less waste) for the specific project
- **get_yarn_consumption_summary**: Provides a detailed breakdown of how much yarn is being used at different scales of the project
- **get_yarn_requirements**: Calculates the total number of yarn balls needed and the amount of yarn remaining after the project
- **validate_project_feasibility**: Checks if a project's yarn requirements are within realistic bounds for standard knitting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knitting Yarn Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm making a sweater with 100 rows, 50 stitches per row, using 5cm of yarn per stitch. Each ball is 100m. How many balls do I need?"

**🤖 AI Agent:**
> You will need 3 balls of yarn, and you will have 50m of yarn left over.

---

**👤 You:**
> "Give me a summary for a project with 200 rows and 40 stitches per row, where each stitch uses 0.04m of yarn."

**🤖 AI Agent:**
> The project consists of 8,000 total stitches and requires 320 meters of yarn.

---

**👤 You:**
> "Is a project with 5000 rows and 100 stitches per row feasible?"

**🤖 AI Agent:**
> No, the project is not feasible because the total yarn consumption exceeds the standard limit.


## ❓ FAQ

**Q: How do I know how much yarn is used per stitch?**
You can measure the length of yarn used for a single stitch from a sample swatch and input that value into the `get_yarn_requirements` tool.

**Q: Can I compare different yarn brands?**
Yes, use the `compare_yarn_options` tool to input the lengths of different yarn balls to see which one results in the least amount of leftover yarn.

**Q: What happens if my project is too large?**
The `validate_project_feasibility` tool will flag projects that exceed 5,000 meters of total yarn consumption as infeasible for standard individual knitting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/knitting-yarn-calculator](https://vinkius.com/en/ai-agent-connect/knitting-yarn-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Knitting Yarn Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knitting-yarn-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Knitting Yarn Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knitting-yarn-calculator": {
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
