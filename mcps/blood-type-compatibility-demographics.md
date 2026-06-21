# Blood Type Compatibility & Demographics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blood-type-compatibility-demographics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Check blood and plasma transfusion compatibility, pregnancy risks, and regional blood type distributions.

## Description
This MCP server provides specialized tools for medical and demographic inquiries regarding blood types. Use `get_rbc_compatibility` to determine if red blood cells can be safely transfused between donors and recipients. Use `get_plasma_rag_compatibility` (wait, checking tool name... it's `get_plasma_compatibility`) to check plasma transfusion safety. The `analyze_pregnancy_risk` tool evaluates Rh incompatibility risks for expectant mothers, while `get_population_distribution` provides statistical data on blood type prevalence in specific regions.


## Available Tools
- **get_plasma_compatibility**: Determines if a donor blood type can safely provide plasma to a recipient
- **get_population_distribution**: Retrieves the blood type distribution for a specific region
- **analyze_pregnancy_risk**: Evaluates the risk of Rh incompatibility between two partners
- **get_rbc_compatibility**: Determines if a donor blood type can safely provide red blood cells to a recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blood Type Compatibility & Demographics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is O- compatible with AB+ for red blood cells?"

**🤖 AI Agent:**
> Yes, O- is a universal donor and is compatible with AB+ for red blood cell transfusion.

---

**👤 You:**
> "What is the risk if the mother is A- and the father is O+?"

**🤖 AI Agent:**
> There is a risk of Rh sensitization because the mother is Rh-negative and the father is Rh-positive.

---

**👤 You:**
> "Show me the blood type distribution in Brazil."

**🤖 AI Agent:**
> In Brazil, the distribution is: O+ (36%), A+ (34%), B+ (7%), O- (5%), A- (4%), AB+ (2%), B- (1%), and AB- (1%).


## ❓ FAQ

**Q: How do I check if a blood transfusion is safe?**
You can use the `get_rbc_compatibility` tool by providing the donor's blood type and the recipient's blood type.

**Q: Can this tool assess pregnancy risks?**
Yes, the `analyze_pregnancy_risk` tool evaluates the risk of Rh incompatibility based on the maternal and paternal blood types.

**Q: Does it provide population data?**
Yes, the `get_population_distribution` tool allows you to retrieve blood type statistics for specific regions like Brazil.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blood-type-compatibility-demographics](https://vinkius.com/mcp/blood-type-compatibility-demographics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blood Type Compatibility & Demographics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blood-type-compatibility-demographics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blood Type Compatibility & Demographics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blood-type-compatibility-demographics": {
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
