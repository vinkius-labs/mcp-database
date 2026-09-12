# Circular Economy Opportunity Identifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/circular-economy-opportunity-identifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Identify circular economy pathways in oil and gas by analyzing waste streams and material flows.

## Description
This MCP server connects AI agents to circular economy frameworks for the oil and gas industry. It enables precise mapping of material movements using `analyze_material_flows` to pinpoint waste generation. Agents can then use `evaluate_circular_options` to rank reuse, recycling, and recovery pathways based on value or compliance. The server also provides `assess_compliance_risk` to ensure actions meet USA or EU regulations and `calculate_economic_impact` to estimate the financial benefits of transitioning from disposal to circularity.


## Available Tools (4)
- **calculate_economic_impact**: Estimate the financial benefit of implementing a specific circular economy opportunity
- **analyze_material_flows**: Map the movement of specific materials through a facility to identify waste generation
- **assess_compliance_risk**: Check if a proposed circular economy action meets regional environmental regulations
- **evaluate_circular_options**: Determine the most viable circularity pathways for a specific waste stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circular Economy Opportunity Identifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trace the flow of produced water in facility FAC-99 to find waste points."

**🤖 AI Agent:**
> The material flow for produced water in FAC-99 shows waste generation at the separation stage and the filtration stage.

---

**👤 You:**
> "What are the best circular options for waste stream WS-402 if I want to maximize value?"

**🤖 AI Agent:**
> The optimal path for WS-402 is Reuse, which offers the highest feasibility score and estimated value.

---

**👤 You:**
> "Is reusing flare gas for local power generation compliant with EU regulations?"

**🤖 AI Agent:**
> The proposed action is compliant with EU environmental standards for energy recovery.


## ❓ FAQ

**Q: How can I find where waste is being generated in my facility?**
You can use the `analyze_material_flows` tool to trace a specific substance through its entire lifecycle within a facility to identify exact waste points.

**Q: Does this tool support regulatory checks for the European Union?**
Yes, the `assess_compliance_risk` tool supports regulatory validation for both the USA and the EU.

**Q: Can I estimate the savings from a recycling project?**
Yes, by using `calculate_economic_impact`, you can determine net value creation and cost savings compared to current disposal methods.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/circular-economy-opportunity-identifier](https://vinkius.com/en/ai-agent-connect/circular-economy-opportunity-identifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circular Economy Opportunity Identifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circular-economy-opportunity-identifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circular Economy Opportunity Identifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circular-economy-opportunity-identifier": {
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
