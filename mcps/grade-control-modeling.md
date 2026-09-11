# Grade Control Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grade-control-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Models grade control for ore/waste discrimination to optimize extraction accuracy.

## Description
This MCP server provides specialized tools for mining grade control. It allows AI agents to identify ore blocks, define operational dig limits, predict dilution impacts, and assess misclassification risks. By using `calculate_ore_blocks`, agents can quantify material meeting economic criteria, while `generate_dig_limits` defines the physical boundaries for mining equipment. The server also includes `estimate_dilution_impact` to predict grade reduction and `evaluate_misclassification_risk` to manage the probability of ore loss or waste misclassification.


## Available Tools (4)
- **calculate_ore_blocks**: Identify and quantify volumes of material meeting economic criteria
- **estimate_dilution_impact**: Predict grade reduction caused by waste inclusion during excavation
- **evaluate_misclassification_risk**: Assess probability of ore loss or waste misclassification
- **generate_dig_limits**: Define operational boundaries for mining equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grade Control Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ore blocks for this assay data with a cutoff grade of 0.5."

**🤖 AI Agent:**
> The identified ore blocks include 3 volumes with an average grade of 0.65, located at coordinates (X:10, Y:20, Z:5).

---

**👤 You:**
> "What are the dig limits for these ore blocks with a selectivity factor of 0.8?"

**🤖 AI Agent:**
> The operational boundaries have been defined as a polygon covering the area from X:5 to X:15 and Y:15 to Y:25.

---

**👤 You:**
> "Estimate the dilution impact for the current dig limits."

**🤖 AI Agent:**
> The expected dilution is 4.2%, resulting in a predicted final grade of 0.58.


## ❓ FAQ

**Q: How can I identify ore volumes?**
You can use the `calculate_ore_blocks` tool by providing assay data, geological interpretation, and the required cutoff grade.

**Q: How do I define excavation boundaries?**
Use the `generate_dig_limits` tool with the identified ore blocks and a selectivity factor to define operational boundaries.

**Q: Can I predict dilution in my mining plan?**
Yes, the `estimate_dilution_impact` tool predicts the expected percentage of dilution and the final grade based on your dig limits and assay data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grade-control-modeling](https://vinkius.com/en/ai-agent-connect/grade-control-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grade Control Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grade-control-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grade Control Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grade-control-modeling": {
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
