# Confined Space Entry Program MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/confined-space-entry-program)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Generates OSHA-compliant safety protocols, atmospheric monitoring, and rescue plans for confined space entries.

## Description
This MCP server provides a compliance-driven engine for managing confined space safety. It uses OSHA Permit-Required Confined Space (PRCS) standards to automate critical safety calculations. Use `evaluate_space_hazard` to classify spaces and identify risks, `calculate_atmospheric_monitoring` to establish gas testing protocols, `determine_ventilation_strategy` to calculate required airflow, and `generate_entry_roles_and_rescue` to define staffing and rescue requirements.


## Available Tools (4)
- **calculate_atmospheric_monitoring**: Determines the required testing frequency and the specific gases that must be monitored
- **determine_ventilation_strategy**: Calculates the necessary mechanical ventilation requirements to maintain a safe atmosphere
- **evaluate_space_hazard**: Determines if a space qualifies as a Permit-Required Confined Space (PRCS) and identifies the primary hazard types
- **generate_entry_roles_and_rescue**: Defines the staffing requirements and the specific rescue protocol required for the entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Confined Space Entry Program** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this tank a permit-required confined space? It has a tapering bottom and potential for engulfment."

**🤖 AI Agent:**
> The space is classified as a Permit-Required Confined Space (PRCS) due to the tapering geometry and engulfment hazard.

---

**👤 You:**
> "What is the required ventilation for a 500 cubic meter space with a contaminant generation rate of 2?"

**🤖 AI Agent:**
> The required airflow rate is calculated based on the volume and contaminant rate to maintain safe levels.

---

**👤 You:**
> "What gases should I monitor in a space with known flammable vapors?"

**🤖 AI Agent:**
> The monitoring protocol requires testing for oxygen levels, flammable gases, and specific toxic contaminants.


## ❓ FAQ

**Q: How does this tool ensure OSHA compliance?**
The engine is built directly upon the OSHA Permit-Required Confined Space (PRCS) standard, ensuring that hazard classification, monitoring, and rescue planning follow regulatory requirements.

**Q: Can I use this to determine if a space needs a permit?**
Yes. By using the `evaluate_space_hazard` tool with specific space attributes and hazard profiles, the system will determine if the space qualifies as a Permit-Required Confined Space.

**Q: What happens if rescue equipment is not available on-site?**
If you indicate that rescue equipment is not available, the `generate_entry_roles_and_rescue` tool will automatically set the rescue plan to 'External Emergency Response'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/confined-space-entry-program](https://vinkius.com/en/ai-agent-connect/confined-space-entry-program)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Confined Space Entry Program** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `confined-space-entry-program` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Confined Space Entry Program** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "confined-space-entry-program": {
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
