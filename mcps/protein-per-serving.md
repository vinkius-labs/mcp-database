# protein-per-serving MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/protein-per-serving)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates protein content per individual serving.

## Description
This MCP server provides precise nutritional calculations to determine protein density. Use `get_protein_per_serving` to find the mass of protein in a single portion, `validate_nutrition_data` to check if nutritional inputs are logically sound, `get_protein_distribution` to see the percentage of total protein per serving, or `summary_protein_stats` for a complete nutritional snapshot.


## Available Tools (4)
- **get_protein_distribution**: Determines what percentage of the total protein is represented by a single serving
- **get_protein_per_serving**: Calculates the amount of protein contained in a single serving
- **summary_protein_stats**: Provides a high-level overview of protein density relative to servings
- **validate_nutrition_data**: Ensures that the provided nutritional values are logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **protein-per-serving** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much protein is in one serving if there are 50g of total protein and 5 servings?"

**🤖 AI Agent:**
> There are 10g of protein in one serving.

---

**👤 You:**
> "What percentage of the total protein does one serving represent if there are 10 servings?"

**🤖 AI Agent:**
> One serving represents 10% of the total protein.

---

**👤 You:**
> "Give me a summary for 100g of protein and 4 servings."

**🤖 AI Agent:**
> The protein per serving is 25g, with a total of 100g protein across 4 servings.


## ❓ FAQ

**Q: How do I calculate protein per serving?**
You can use the `get_protein_per_serving` tool by providing the total protein mass and the total number of servings.

**Q: Can I validate my nutritional data first?**
Yes, use `validate_nutrition_data` to ensure your protein and serving counts are valid before performing calculations.

**Q: What if my serving count is zero?**
The tools will return an error if the serving count is zero or negative, as a valid calculation requires at least one serving.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/protein-per-serving](https://vinkius.com/en/ai-agent-connect/protein-per-serving)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **protein-per-serving** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `protein-per-serving` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **protein-per-serving** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protein-per-serving": {
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
