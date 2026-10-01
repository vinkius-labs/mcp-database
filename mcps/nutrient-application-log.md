# Nutrient Application Log MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nutrient-application-log)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Track and analyze cumulative nutrient applications and target rate compliance.

## Description
This MCP server provides tools to manage agricultural nutrient data. It allows for calculating the total nutrient load applied to specific areas using `get_cumulative_nutrient_load`, comparing current application rates against desired targets with `compare_application_to_target`, reviewing historical application logs via `get_application_history`, and inspecting product chemical compositions through `get_product_analysis_details`.


## Available Tools (4)
- **compare_application_to_target**: Compares the applied nutrient rate against a target rate
- **get_cumulative_nutrient_load**: g., N, P, K) and the area ID to get cumulative totals.

Calculates the total amount of a specific nutrient applied to an area
- **get_product_analysis_details**: Gets the chemical composition and nutrient concentrations of a product
- **get_application_history**: Retrieves the history of all nutrient applications for a specific area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutrient Application Log** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total amount of Nitrogen applied to Field-A?"

**🤖 AI Agent:**
> A total of 45.5 kg of Nitrogen has been applied to Field-A.

---

**👤 You:**
> "Is the current Potassium application meeting the target rate of 20 units per area?"

**🤖 AI Agent:**
> The current application is MEETING the target rate.

---

**👤 You:**
> "Show me the history of applications for Zone-7."

**🤖 AI Agent:**
> On 2024-05-12, 50kg of Product-X was applied. On 2024-06-01, 40kg of Product-Y was applied.


## ❓ FAQ

**Q: How do I check if my nitrogen levels are sufficient?**
You can use the `compare_application_to_target` tool by providing the nitrogen nutrient ID, your area ID, and your desired target rate.

**Q: Can I see a list of all previous fertilizer applications?**
Yes, the `get_application_history` tool provides a chronological list of all recorded application events for a specific area.

**Q: How is the total nutrient amount calculated?**
The `get_cumulative_nutrient_load` tool calculates the total weight by summing the nutrient mass from every application log entry matching your criteria.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nutrient-application-log](https://vinkius.com/en/ai-agent-connect/nutrient-application-log)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutrient Application Log** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nutrient-application-log` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutrient Application Log** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutrient-application-log": {
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
