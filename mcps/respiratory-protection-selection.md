# Respiratory Protection Selection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/respiratory-protection-selection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [oil-and-gas](../categories/oil-and-gas.md)

Selects appropriate respiratory protection for oil and gas operations using NIOSH standards.

## Description
This MCP server provides critical safety tools for selecting respiratory protection in hazardous environments. It uses NIOSH standards to calculate required protection factors, recommend specific respirator types, and estimate cartridge service life. Use `get_protection_requirement` to assess hazard levels, `select_respirator_type` to find compatible equipment, `calculate_cartridge_service_life` to manage filter changes, and `validate_safety_compliance` for final safety verification.


## Available Tools (4)
- **select_respirator_type**: Recommends a specific respirator model or type based on the required protection factor
- **validate_safety_compliance**: Performs a final check to ensure all safety parameters align with NIOSH guidelines
- **calculate_cartridge_service_life**: Estimates when a chemical cartridge will lose effectiveness
- **get_protection_requirement**: Determines the minimum required protection level and whether the environment is safe for air-purifying respirators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Respiratory Protection Selection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What protection is needed for organic vapors at 50 ppm with a PEL of 10 ppm?"

**🤖 AI Agent:**
> A respirator with an Assigned Protection Factor (APF) of at least 5 is required to maintain safety at this concentration.

---

**👤 You:**
> "How long will a cartridge last for acid gas at 15 ppm if I work 8 hours a day?"

**🤖 AI Agent:**
> The estimated service life is 40 hours, meaning the cartridge should be changed every 5 days.

---

**👤 You:**
> "Is a half-face respirator compliant for an IDLH environment?"

**🤖 AI Agent:**
> No, a half-face respirator is not compliant in an IDLH environment; supplied-air equipment is required.


## ❓ FAQ

**Q: How does the tool handle oxygen-deficient environments?**
In oxygen-deficient environments, the `get_protection_requirement` tool identifies that air-purifying respirators are unsafe and mandates the use of supplied-air respirators.

**Q: Can I use this to manage my cartridge replacement schedule?**
Yes, you can use `calculate_cartridge_service_life` to estimate the hours until breakthrough and determine the recommended change interval based on contaminant concentration.

**Q: What happens if the environment is IDLH?**
If the environment is IDLH, the `validate_safety_compliance` tool ensures that only the highest level of protection, such as supplied-air equipment, is used to maintain safety.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/respiratory-protection-selection](https://vinkius.com/en/ai-agent-connect/respiratory-protection-selection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Respiratory Protection Selection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `respiratory-protection-selection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Respiratory Protection Selection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "respiratory-protection-selection": {
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
