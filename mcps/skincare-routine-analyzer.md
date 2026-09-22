# Skincare Routine Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/skincare-routine-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze skincare regimens to count products and assess complexity.

## Description
This MCP server provides tools to analyze skincare routines. You can use `count_total_products` to find the total number of items used, `count_products_by_category` to filter by type, `analyze_routine_complexity` to determine if a regimen is minimal or intensive, and `get_step_breakdown` to see product counts per step.


## Available Tools (4)
- **analyze_routine_complexity**: Assesses the complexity level of the skincare routine
- **count_products_by_category**: Counts products belonging to a specific functional category
- **count_total_products**: Counts the total number of products used in the entire routine
- **get_step_breakdown**: Provides a breakdown of product counts for each step in the routine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skincare Routine Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total products are in my routine: Morning (Cleanser, Moisturizer), Evening (Cleanser, Treatment, Moisturizer)?"

**🤖 AI Agent:**
> There are 5 total products in your routine.

---

**👤 You:**
> "How many cleansers am I using in this routine: Morning (Cleanser, Sunscreen), Evening (Cleanser, Moisturizer)?"

**🤖 AI Agent:**
> You are using 2 cleansers.

---

**👤 You:**
> "Is my routine intensive? Morning (Cleanser, Toner, Serum, Moisturizer, Sunscreen), Evening (Cleanser, Serum, Moisturizer)."

**🤖 AI Agent:**
> Your routine is considered Advanced with 8 total products.


## ❓ FAQ

**Q: How can I find the total number of products in my routine?**
You can use the `count_total_products` tool by providing your list of routine steps.

**Q: Can I check how many cleansers I am using?**
Yes, use the `count_products_by_category` tool and specify 'Cleanser' as the target category.

**Q: How is routine complexity determined?**
The `analyze_routine_complexity` tool evaluates the total product volume to label the routine as Minimal, Standard, or Advanced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/skincare-routine-analyzer](https://vinkius.com/en/ai-agent-connect/skincare-routine-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skincare Routine Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `skincare-routine-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skincare Routine Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skincare-routine-analyzer": {
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
