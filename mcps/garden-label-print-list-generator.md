# Garden Label Print List Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/garden-label-print-list-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates optimized plant identification label print lists based on garden plot requirements and physical printing constraints.

## Description
This MCP server bridges the gap between garden planning and physical labeling. It allows AI agents to calculate exact printing needs for plant identification labels. Using tools like `get_print_summary` and `generate_print_manifest`, agents can determine how many sheets of labels are required, how many labels fit on a sheet using `validate_sheet_fit`, and provide a detailed breakdown of varieties via `calculate_variety_distribution`. It is designed to handle duplicate label preferences and physical sheet capacities to ensure gardeners have exactly what they need for their plots.


## Available Tools (4)
- **calculate_variety_distribution**: Breaks down the label requirements by specific plant variety
- **generate_print_manifest**: Produces the final ordered list of text to be printed on each label
- **get_print_summary**: Provides a high-level overview of the total printing requirements
- **validate_sheet_fit**: Determines if the label dimensions and sheet capacity are physically compatible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Garden Label Print List Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 5 Tomato plants and 3 Basil plants. I want 2 labels for each plant. My sticker sheets hold 10 labels each. How many sheets do I need?"

**🤖 AI Agent:**
> You will need 1 sheet. You have a total of 8 plants, and with a duplicate multiplier of 2, you need 16 labels. Since each sheet holds 10 labels, 2 sheets are required to cover all 16 labels.

---

**👤 You:**
> "Calculate the variety distribution for: [{ varietyName: 'Lavender', plotCount: 10 }, { varietyName: 'Peony', plotCount: 5 }] with a duplicate multiplier of 1."

**🤖 AI Agent:**
> The breakdown is: Lavender (10 labels) and Peony (5 labels). There are 2 unique varieties in total.

---

**👤 You:**
> "Will 2x2 inch labels fit on a 4x6 inch sheet?"

**🤖 AI Agent:**
> Yes, you can fit 6 labels on a 4x6 inch sheet using a 2x2 inch label size.


## ❓ FAQ

**Q: How do I know how many sheets of labels I need to buy?**
You can use the `get_print_summary` tool. By providing the total plant count, your duplicate multiplier, and the sheet capacity, the tool will return the exact number of physical sheets needed.

**Q: Can I check if my labels will fit on my specific sticker paper?**
Yes, the `validate_sheet_fit` tool allows you to input your label and sheet dimensions to confirm if they are physically compatible.

**Q: How does the tool handle multiple copies of the same plant?**
You can specify a duplicate multiplier. For example, setting it to 2 will ensure the `generate_print_manifest` tool produces two labels for every one plant in your list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/garden-label-print-list-generator](https://vinkius.com/en/ai-agent-connect/garden-label-print-list-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Garden Label Print List Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `garden-label-print-list-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Garden Label Print List Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "garden-label-print-list-generator": {
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
