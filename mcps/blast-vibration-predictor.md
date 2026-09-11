# Blast Vibration Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/blast-vibration-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict ground vibration intensity and regulatory compliance from blasting events.

## Description
This MCP server provides specialized tools for blasting engineering. It allows AI agents to predict Peak Particle Velocity (PPV) using square root scaling, assess structural risks based on frequency content, and validate compliance with USA and European regulatory standards. Use `calculate_ppv` to model vibration intensity, `analyze_frequency_risk` to evaluate structural safety, and `check_compliance` to ensure legal adherence to vibration limits.


## Available Tools (4)
- **analyze_frequency_risk**: Determines if the vibration frequency poses a risk to structures
- **calculate_ppv**: Predicts the Peak Particle Velocity (PPV) for a blasting event
- **check_compliance**: Validates if the predicted vibration meets regulatory safety limits
- **simulate_attenuation_profile**: Provides a range of potential PPV values based on varying geological conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blast Vibration Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the PPV for a 50kg charge at 100m distance with a site condition factor of 1.2."

**🤖 AI Agent:**
> The predicted Peak Particle Velocity (PPV) is 12.45 mm/s with a scaled distance of 14.43.

---

**👤 You:**
> "Is a vibration of 15 mm/s compliant with USA regulations?"

**🤖 AI Agent:**
> No, the predicted PPV of 15 mm/s exceeds the USA residential threshold of 12.5 mm/s.

---

**👤 You:**
> "What is the risk level for a 20 mm/s vibration at 5 Hz?"

**🤖 AI Agent:**
> The risk level is High because low frequency vibrations at this PPV can cause significant structural damage.


## ❓ FAQ

**Q: How is the vibration intensity calculated?**
The intensity is calculated using the `calculate_ppv` tool, which applies square root scaling based on charge weight, distance, and geological attenuation factors.

**Q: Can I check if my blast meets legal requirements?**
Yes, the `check_compliance` tool validates predicted PPV against regulatory thresholds for the USA and Europe.

**Q: How does ground type affect the prediction?**
Different ground types are modeled using site condition factors. You can use `simulate_attenuation_profile` to see how varying geological conditions impact the predicted vibration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/blast-vibration-predictor](https://vinkius.com/en/ai-agent-connect/blast-vibration-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blast Vibration Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blast-vibration-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blast Vibration Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blast-vibration-predictor": {
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
