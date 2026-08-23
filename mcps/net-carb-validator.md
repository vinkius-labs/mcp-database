# Net Carb Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/net-carb-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise net carbohydrates and keto suitability from nutrition labels.

## Description
This MCP server provides deterministic tools to calculate net carbohydrate content from nutritional label data. It accounts for dietary fiber and the varying metabolic impacts of different sugar alcohols. Use `calculate_net_carbs` to determine the final digestible carb count and keto-friendly status, or `validate_label_integrity` to ensure a label's fiber and carbohydrate values are mathematically plausible.


## Available Tools (3)
- **calculate_net_carbs**: 
- **get_sugar_alcohol_impact**: 
- **validate_label_integrity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Net Carb Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the net carbs for a snack with 20g total carbs, 5g fiber, and 4g erythritol."

**🤖 AI Agent:**
> The final net carbs are 11g, and this snack is not keto-friendly.

---

**👤 You:**
> "Is a food with 10g total carbs, 6g fiber, and 2g allulose keto-friendly?"

**🤖 AI Agent:**
> The final net carbs are 2g, so this food is keto-friendly.

---

**👤 You:**
> "Check if a label with 15g total carbs and 20g fiber is valid."

**🤖 AI Agent:**
> The label is invalid because the fiber content exceeds the total carbohydrate content.


## ❓ FAQ

**Q: How does the tool handle different sugar alcohols?**
The tool applies specific metabolic rules: 100% of erythritol and allulose are subtracted, while only 50% of maltitol and glycerin are subtracted from the total carbohydrate count.

**Q: What defines a food as keto-friendly?**
A food is flagged as keto-friendly if the final net carbohydrate count is less than 5 grams per serving.

**Q: Can I verify if a nutrition label is valid?**
Yes, you can use `validate_label_integrity` to check if the reported dietary fiber exceeds the total carbohydrates, which would indicate an invalid label.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/net-carb-validator](https://vinkius.com/ai-agent-connect/net-carb-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Net Carb Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `net-carb-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Net Carb Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "net-carb-validator": {
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
