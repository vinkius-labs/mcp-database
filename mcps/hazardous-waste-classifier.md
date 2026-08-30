# Hazardous Waste Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hazardous-waste-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Classifies waste streams as hazardous or non-hazardous using RCRA and EU standards.

## Description
This MCP server provides regulatory intelligence to identify hazardous waste. It uses `classify_waste_stream` to evaluate waste composition and physical properties against RCRA (USA) and EU Waste Framework Directive standards. Users can also use `get_hazard_code_details` to retrieve specific regulatory codes and `determine_disposal_protocol` to identify required handling methods for specific facilities.


## Available Tools (4)
- **classify_waste_stream**: Performs the primary classification of a waste stream based on its constituents and properties
- **determine_disposal_protocol**: Identifies the required handling and disposal methods for the classified waste
- **get_hazard_code_details**: Provides specific regulatory codes and the formal reasoning for a given classification
- **validate_composition_thresholds**: Checks if specific chemical constituents exceed legal toxicity limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hazardous Waste Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify this waste: composition is 5% Lead, 95% Water; region is USA."

**🤖 AI Agent:**
> The waste is classified as Hazardous due to toxicity levels exceeding RCRA limits.

---

**👤 You:**
> "What is the disposal protocol for hazardous waste at a standard landfill?"

**🤖 AI Agent:**
> Disposal at a standard landfill is prohibited for this hazardous waste; specialized treatment or a hazardous waste landfill is required.

---

**👤 You:**
> "Check if this waste is toxic in the EU: composition is 10% Mercury, 90% Water."

**🤖 AI Agent:**
> Yes, the concentration of Mercury exceeds the legal toxicity threshold for the EU.


## ❓ FAQ

**Q: Which regulatory frameworks are supported?**
The server supports both RCRA (USA) and the EU Waste Framework Directive.

**Q: How do I find the specific hazard code for my waste?**
After running `classify_waste_stream`, pass the result to `get_hazard_code_details` to obtain the specific regulatory codes and risk levels.

**Q: Can I determine if a landfill is suitable for my waste?**
Yes, use `determine_disposal_protocol` and specify the facility type to see if it is permitted for your specific waste classification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hazardous-waste-classifier](https://vinkius.com/ai-agent-connect/hazardous-waste-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hazardous Waste Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hazardous-waste-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hazardous Waste Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hazardous-waste-classifier": {
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
