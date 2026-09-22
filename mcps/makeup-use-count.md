# Makeup Use Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/makeup-use-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate product longevity and application frequency.

## Description
This MCP server provides tools to determine how long cosmetic products will last. Use `get_use_count` to find the total number of applications available, `validate_application_dose` to check if a dose is realistic for a product type, `get_product_standard_dose` to find recommended amounts, and `estimate_lifespan_days` to predict the total days of usage based on daily frequency.


## Available Tools (4)
- **estimate_lifespan_days**: Predicts how many days a product will last based on daily usage frequency
- **get_product_standard_dose**: Retrieves the recommended average application dose for a given product category
- **get_use_count**: Calculates how many times a specific product can be used
- **validate_application_dose**: Checks if a proposed application dose is realistic for a specific product type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Makeup Use Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many times can I use a 50ml bottle of serum if I use 0.5ml each time?"

**🤖 AI Agent:**
> You can use the serum 100 times.

---

**👤 You:**
> "If I have 30g of powder and use 1g per day, how many days will it last?"

**🤖 AI Agent:**
> The powder will last for 30 days.

---

**👤 You:**
> "Is 5ml a reasonable dose for a liquid toner?"

**🤖 AI Agent:**
> The dose is valid for the liquid product type.


## ❓ FAQ

**Q: How do I know how many times my foundation will last?**
You can use the `get_use_count` tool by providing the total volume of the foundation and the amount you use per application.

**Q: Can I estimate the days until my serum runs out?**
Yes, the `estimate_lifespan_days` tool allows you to predict the total days of usage if you provide the volume, dose, and how many times you use it daily.

**Q: Is the dose validation accurate for different product types?**
Yes, `validate_application_dose` checks the proposed dose against standard ranges for liquids, creams, and powders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/makeup-use-count](https://vinkius.com/en/ai-agent-connect/makeup-use-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Makeup Use Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `makeup-use-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Makeup Use Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "makeup-use-count": {
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
