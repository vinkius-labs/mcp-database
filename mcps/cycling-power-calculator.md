# Cycling Power Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cycling-power-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Estimate cycling power requirements, FTP zones, and training stress.

## Description
A professional utility for cyclists to estimate physiological power requirements. Use `calculate_power_requirement` to determine the watts needed for specific speeds and gradients, accounting for aerodynamic drag (CdA) and rolling resistance. The `get_ftp_zones` tool converts FTP into seven actionable training intensity zones. For post-ride analysis, use `calculate_training_stress` to compute your Training Stress Score (TSS). You can also retrieve standardized aerodynamic coefficients using `get_positional_cda` for positions like tops, hoods, or aero.


## Available Tools (4)
- **calculate_power_requirement**: Calculate the power required to maintain a specific speed on given terrain
- **get_ftp_zones**: Convert FTP into training intensity zones
- **get_positional_cda**: Retrieve the CDA value for a specific riding posture
- **calculate_training_stress**: Calculate the Training Stress Score (TSS)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycling Power Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many watts do I need to ride at 30 km/h on a 5% gradient with a 75kg total weight, 0.01 resistance, and 0.035 CdA?"

**🤖 AI Agent:**
> You will need approximately 285.4 Watts to maintain that speed on a 5% gradient.

---

**👤 You:**
> "What are my training zones if my FTP is 250W?"

**🤖 AI Agent:**
> Your zones are: Zone 1 (125-150W), Zone 2 (150-175W), Zone 3 (175-200W), Zone 4 (200-225W), Zone 5 (225-237W), Zone 6 (237-250W), and Zone 7 (above 250W).

---

**👤 You:**
> "What is the CDA for the 'aero' position?"

**🤖 AI Agent:**
> The standardized aerodynamic drag area (CdA) for the aero position is 0.025.


## ❓ FAQ

**Q: How is the power requirement calculated?**
The `calculate_power_requirement` tool uses a physics model that sums the power needed to overcome gravity, aerodynamic drag (based on your CdA), and rolling resistance.

**Q: What are training zones?**
By using `get_ftp_zones`, you can see seven distinct power ranges relative to your FTP, helping you target specific physiological intensities during training.

**Q: Can I calculate TSS for a ride?**
Yes, the `calculate_training_stress` tool calculates your Training Stress Score based on duration, normalized power, and FTP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cycling-power-calculator](https://vinkius.com/mcp/cycling-power-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycling Power Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycling-power-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycling Power Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycling-power-calculator": {
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
