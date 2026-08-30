# Safety Data Sheet Synthesis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/safety-data-sheet-synthesis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Generates regulatory-compliant GHS Safety Data Sheet (SDS) summaries from chemical data.

## Description
This MCP server automates the generation of critical Safety Data Sheet (SDS) sections using GHS standards. It allows AI agents to analyze chemical mixtures via `analyze_composition`, assign hazard categories with `classify_hazards`, retrieve standardized safety phrases using `generate_precautionary_statements`, and suggest protective measures through `recommend_exposure_controls`. It is designed to ensure regulatory compliance for chemical safety documentation.


## Available Tools (4)
- **analyze_composition**: Total concentration must be 100%.

Determines the hazard profile of a chemical mixture based on its constituents
- **classify_hazards**: Assigns GHS hazard categories based on physical and health data
- **generate_precautionary_statements**: Selects the appropriate safety phrases based on identified hazards
- **recommend_exposure_controls**: Suggests engineering controls and Personal Protective Equipment (PPE)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Safety Data Sheet Synthesis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this mixture: 70% Ethanol (CAS 64-17-5) and 30% Water."

**🤖 AI Agent:**
> The mixture is classified as a Flammable Liquid, Category 2, due to the high concentration of Ethanol.

---

**👤 You:**
> "What are the hazard classes for a substance with a flash point of 15°C?"

**🤖 AI Agent:**
> The substance is classified as a Flammable Liquid, Category 2.

---

**👤 You:**
> "Generate precautionary statements for a Flammable Liquid Category 2."

**🤖 AI Agent:**
> Keep away from heat, hot surfaces, sparks, open flames and other ignition sources. No smoking.


## ❓ FAQ

**Q: What standards does this server follow?**
The server follows the Globally Harmonized System (GHS) for the classification and labeling of chemicals.

**Q: Can I analyze mixtures?**
Yes, you can use the `analyze_composition` tool to determine the hazard profile of a mixture based on its individual components.

**Q: Does it provide PPE recommendations?**
Yes, the `recommend_exposure_controls` tool provides suggestions for engineering controls and Personal Protective Equipment based on identified hazards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/safety-data-sheet-synthesis](https://vinkius.com/ai-agent-connect/safety-data-sheet-synthesis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Safety Data Sheet Synthesis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `safety-data-sheet-synthesis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Safety Data Sheet Synthesis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "safety-data-sheet-synthesis": {
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
