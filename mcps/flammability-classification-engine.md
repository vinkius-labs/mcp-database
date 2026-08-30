# Flammability Classification Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/flammability-classification-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Classifies flammable liquids and gases using GHS and NFPA standards.

## Description
This MCP server provides specialized tools for chemical safety analysis. It determines GHS hazard categories and NFPA flammability ratings for liquids and gases based on thermal properties like flash point and boiling point. Users can evaluate immediate ignition risks with `check_ambient_risk` and retrieve regulatory storage guidelines using `get_storage_compliance`. The engine also handles specific liquid and gas classifications via `classify_liquid` and `classify_gas`.


## Available Tools (4)
- **check_ambient_risk**: Evaluates the immediate ignition risk based on current environmental conditions
- **classify_gas**: Determines the hazard classification for flammable gases
- **classify_liquid**: Determines the GHS and NFPA classifications for a flammable liquid
- **get_storage_compliance**: Provides specific regulatory storage guidelines for a classified substance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flammability Classification Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify a liquid with a flash point of -20C, boiling point of 78C, and a flammable range of 1.5 to 10.0."

**🤖 AI Agent:**
> The liquid is classified as GHS Category 2 with an NFPA rating of 3. Required pictograms: Flame. Storage instructions: Store in a cool, well-ventilated area in an explosion-proof cabinet.

---

**👤 You:**
> "What is the risk if the ambient temperature is 25C and the flash point is 20C for a Category 2 liquid?"

**🤖 AI Agent:**
> The risk level is Extreme. Ignition probability is high because the ambient temperature exceeds the flash point. Immediate evacuation or specialized safety protocols are required.

---

**👤 You:**
> "What are the storage requirements for a substance with GHS Category 1 and NFPA rating 4?"

**🤖 AI Agent:**
> The substance must be stored in a specialized Flammable Cabinet with high-volume mechanical ventilation. Use explosion-proof containment and ensure the storage zone temperature remains below the specified maximum safety threshold.


## ❓ FAQ

**Q: What standards does this tool use for classification?**
The tool uses the Globally Harmonized System (GHS) for hazard categories and the NFPA 704 standard for flammability ratings.

**Q: How can I check if a substance is safe to store in my current environment?**
You can use the `check_ambient_risk` tool by providing the substance's flash point and the current ambient temperature to assess immediate ignition probability.

**Q: Does this tool provide storage instructions?**
Yes, both `classify_liquid` and `classify_gas` return specific storage instructions, and `get_storage_compliance` provides detailed regulatory guidelines for storage zones and containment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/flammability-classification-engine](https://vinkius.com/ai-agent-connect/flammability-classification-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flammability Classification Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flammability-classification-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flammability Classification Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flammability-classification-engine": {
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
