# Destemming & Crushing Efficiency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/destemming-crushing-efficiency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate throughput, stem removal, and berry damage for winemaking machinery.

## Description
This MCP server provides precise calculations for the destemming and crushing stage of vinification. It helps winemakers optimize machine performance by analyzing how grape variety and cluster morphology affect processing. Use `get_current_throughput` to monitor real-time mass flow, `analyze_stem_removal` to evaluate stem detachment efficiency, and `calculate_berry_damage` to predict breakage. You can also use `optimize_machine_settings` to find the ideal balance between roller spacing and drum speed for your specific target damage rate.


## Available Tools (4)
- **analyze_stem_removal**: Evaluate how effectively the machine is separating stems from the fruit
- **calculate_berry_damage**: Predict the percentage of berry breakage based on machine settings
- **get_current_throughput**: Determine the actual mass of grapes being processed per hour
- **optimize_machine_settings**: Recommend ideal roller spacing and drum speed to meet a target damage rate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Destemming & Crushing Efficiency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current throughput for a Cabernet Sauvignon with a 5kg cluster weight and 2% MOG at 1000kg/h capacity?"

**🤖 AI Agent:**
> The actual throughput is 945 kg/h with an Optimal efficiency rating.

---

**👤 You:**
> "Predict the berry damage for Pinot Noir with 4kg clusters, 15mm roller spacing, and 30 drum speed at a 10% target damage rate."

**🤖 AI Agent:**
> The predicted berry breakage is 12%, with a juice loss of 3% and a deviation of 2% from your target.

---

**👤 You:**
> "Recommend settings for Merlot with 6kg clusters to hit a 5% damage rate."

**🤖 AI Agent:**
> The recommended settings are 18mm roller spacing and 25 drum speed, with a predicted efficiency of 0.85.


## ❓ FAQ

**Q: How does grape variety affect the calculations?**
Different varieties have different cluster morphologies. The tools use this data to adjust throughput and stem removal predictions, as compact clusters resist detachment more than loose ones.

**Q: Can I optimize my machine settings for a specific damage rate?**
Yes, the `optimize_machine_settings` tool recommends the best roller spacing and drum speed to achieve your desired berry damage target.

**Q: What is MOG and how does it impact throughput?**
MOG stands for Material Other than Grapes (like leaves or twigs). High MOG levels can reduce actual throughput and decrease stem removal efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/destemming-crushing-efficiency](https://vinkius.com/en/ai-agent-connect/destemming-crushing-efficiency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Destemming & Crushing Efficiency** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `destemming-crushing-efficiency` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Destemming & Crushing Efficiency** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "destemming-crushing-efficiency": {
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
