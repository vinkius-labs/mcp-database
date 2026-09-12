# Radioactive Material Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/radioactive-material-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Manage NORM compliance and radiation safety for oil and gas operations.

## Description
This MCP server provides specialized tools for managing Naturally Occurring Radioactive Material (NORM) in oil and gas environments. It allows AI agents to perform critical safety tasks such as using `get_exposure_assessment` to calculate worker radiation doses, `get_handling_requirements` to identify necessary safety gear, `check_disposal_authorization` to verify legal disposal methods, and `evaluate_public_safety_impact` to assess environmental risks. It ensures all operations align with international radiation protection standards.


## Available Tools (4)
- **check_disposal_authorization**: Evaluates if a specific batch of NORM can be disposed of using a selected method
- **evaluate_public_safety_impact**: Assesses if the material poses a risk to the general public in the surrounding environment
- **get_exposure_assessment**: Determines the potential radiation dose for workers handling the material
- **get_handling_requirements**: Identifies the necessary safety protocols and equipment needed to work with a specific volume of NORM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Radioactive Material Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated radiation dose for a worker handling 50 units of NORM with a concentration of 10 and a handling time of 2 hours?"

**🤖 AI Agent:**
> The estimated radiation dose is 1000 units, and the protection level required is high.

---

**👤 You:**
> "Is it authorized to use a landfill for 5 units of NORM with a concentration of 2?"

**🤖 AI Agent:**
> Yes, disposal via landfill is authorized for this concentration level.

---

**👤 You:**
> "What are the handling requirements for 100 units of NORM at a concentration of 50?"

**🤖 AI Agent:**
> The required equipment includes lead-lined containers and specialized shielding, following the high-risk safety protocol.


## ❓ FAQ

**Q: How can I check if a disposal method is legal?**
You can use the `check_disposal_authorization` tool to verify if a specific concentration of NORM is permitted for your chosen disposal method.

**Q: What safety gear is needed for handling NORM?**
The `get_handling_requirements` tool will provide a specific list of required equipment and safety protocols based on the material's concentration and volume.

**Q: Can this tool assess worker safety?**
Yes, the `get_exposure_assessment` tool calculates the estimated radiation dose for workers to ensure they stay within occupational limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/radioactive-material-management](https://vinkius.com/en/ai-agent-connect/radioactive-material-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Radioactive Material Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `radioactive-material-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Radioactive Material Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "radioactive-material-management": {
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
