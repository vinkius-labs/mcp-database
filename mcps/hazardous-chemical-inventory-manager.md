# Hazardous Chemical Inventory Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hazardous-chemical-inventory-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Manage chemical safety, storage compliance, and regulatory reporting.

## Description
This MCP server provides essential tools for managing hazardous chemical inventories and ensuring regulatory compliance. Use `get_chemical_safety_profile` to retrieve hazard classifications and reportable quantities for specific substances. Verify storage safety using `check_storage_compliance` to detect incompatible chemicals or capacity violations. Automatically determine regulatory needs with `calculate_reporting_obligations` for EPCRA and emergency planning, and ensure all safety documentation is present via `verify_documentation_status`.


## Available Tools (4)
- **calculate_reporting_obligations**: Calculate regulatory reporting requirements based on inventory
- **check_storage_compliance**: Check if a list of chemicals can be safely stored in a specific area
- **get_chemical_safety_profile**: Get the specific hazard classifications and regulatory thresholds for a chemical
- **verify_documentation_status**: Verify if all chemicals in the inventory have required SDS and labels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hazardous Chemical Inventory Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the safety profile for Acetone?"

**🤖 AI Agent:**
> Acetone is classified as a Flammable liquid with a reportable quantity threshold defined by regulatory standards.

---

**👤 You:**
> "Is it safe to store 50kg of Ethanol and 20kg of Nitric Acid in Cabinet A?"

**🤖 AI Agent:**
> No, the storage is non-compliant. Incompatible chemicals detected: Flammables and Oxidizers.

---

**👤 You:**
> "Do I need to file an emergency plan for my current inventory?"

**🤖 AI Agent:**
> Yes, the cumulative quantity of certain hazard classes has reached the Threshold Planning Quantity, requiring an emergency plan.


## ❓ FAQ

**Q: How do I check if my chemicals are stored safely?**
You can use the `check_storage_compliance` tool by providing your current inventory list and the specific storage area ID.

**Q: Can this tool help with EPCRA reporting?**
Yes, the `calculate_reporting_obligations` tool identifies if any chemical quantities have triggered EPCRA reporting requirements.

**Q: How do I verify if my SDS documentation is complete?**
Use the `verify_documentation_status` tool to check if all chemicals in your inventory have the required Safety Data Sheets and labels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hazardous-chemical-inventory-manager](https://vinkius.com/en/ai-agent-connect/hazardous-chemical-inventory-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hazardous Chemical Inventory Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hazardous-chemical-inventory-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hazardous Chemical Inventory Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hazardous-chemical-inventory-manager": {
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
