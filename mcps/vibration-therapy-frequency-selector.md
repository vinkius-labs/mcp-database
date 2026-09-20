# Vibration Therapy Frequency Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vibration-therapy-frequency-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Determines optimal vibration therapy parameters based on clinical goals and patient safety.

## Description
This MCP server provides specialized tools for designing vibration therapy regimens. It calculates precise frequency, amplitude, duration, and rest intervals by analyzing the treatment goal, target anatomy, and patient health status. Use `get_therapy_protocol` to generate a complete regimen, `validate_safety_parameters` to ensure settings are within safe limits, `get_anatomical_tolerances` to check body part limits, and `calculate_rest_requirements` to determine necessary recovery times.


## Available Tools (4)
- **calculate_rest_requirements**: Determines the necessary recovery time based on the intensity of the session
- **get_anatomical_tolerances**: Retrieves the maximum safe operating limits for a specific body part
- **get_therapy_protocol**: Provides a complete, customized vibration therapy regimen based on specific clinical inputs
- **validate_safety_parameters**: Checks if a specific set of vibration parameters is safe for a given patient and body part


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vibration Therapy Frequency Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Provide a vibration therapy protocol for strength training on the quadriceps for a stable patient."

**🤖 AI Agent:**
> For strength training on the quadriceps, use a frequency of 45 Hz and an amplitude of 2.5 mm for 10 minutes, followed by a 5-minute rest interval.

---

**👤 You:**
> "What are the safety limits for the forearm in a patient with sensitive skin?"

**🤖 AI Agent:**
> The maximum safe frequency for the forearm is 35 Hz and the maximum amplitude is 1.5 mm for patients with high sensitivity.

---

**👤 You:**
> "Calculate the rest needed after a 15-minute circulation session."

**🤖 AI Agent:**
> A 15-minute circulation session requires a 3-minute rest interval to maintain optimal vascular stimulation.


## ❓ FAQ

**Q: How do I get a full therapy plan?**
You can use the `get_therapy_protocol` tool by providing the treatment goal, body part, and patient condition to receive a complete regimen.

**Q: Can I check if a specific frequency is safe?**
Yes, use the `validate_safety_parameters` tool to verify if your chosen frequency and amplitude are safe for the specific patient and body part.

**Q: How much rest is needed between sessions?**
The `calculate_rest_requirements` tool determines the necessary recovery time based on the intensity and duration of the vibration applied.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vibration-therapy-frequency-selector](https://vinkius.com/en/ai-agent-connect/vibration-therapy-frequency-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vibration Therapy Frequency Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vibration-therapy-frequency-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vibration Therapy Frequency Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vibration-therapy-frequency-selector": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
