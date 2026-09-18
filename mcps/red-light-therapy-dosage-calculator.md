# Red Light Therapy Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/red-light-therapy-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate precise photobiomodulation parameters including exposure time, frequency, and energy delivery.

## Description
This MCP server provides clinical-grade calculation tools for photobiomodulation (PBM) therapy. It allows AI agents to determine optimal treatment protocols by analyzing device specifications and physiological goals. Users can use `calculate_exposure_parameters` to find the exact duration and frequency needed for specific outcomes like skin health or muscle recovery. The server also includes `verify_device_safety` to ensure irradiance levels remain within safe physiological limits, `calculate_total_session_energy` for precise Joule measurement, and `estimate_depth_penetration` to predict how deeply light will reach based on wavelength.


## Available Tools (4)
- **calculate_exposure_parameters**: 
- **calculate_total_session_energy**: 
- **estimate_depth_penetration**: 
- **verify_device_safety**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Red Light Therapy Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 660nm red light device with an irradiance of 50 mW/cm2. I want to treat a 10cm2 area on my face for skin health. How long should my session be?"

**🤖 AI Agent:**
> For a 660nm wavelength at 50 mW/cm2 targeting skin health over a 10cm2 area, you should perform a session for 4 minutes, 3 times per week.

---

**👤 You:**
> "Is it safe to use a device with 150 mW/cm2 irradiance at 850nm wavelength?"

**🤖 AI Agent:**
> The device is safe to use. To maintain safety, it is recommended to keep a minimum distance of 15cm from the target area.

---

**👤 You:**
> "How much total energy will I deliver if I use my 700nm light at 30 mW/cm2 for 5 minutes on a 5cm2 area?"

**🤖 AI Agent:**
> The total energy delivered during this session will be 4.5 Joules.


## ❓ FAQ

**Q: How do I know if my device is safe to use?**
You can use the `verify_device_safety` tool. By providing the wavelength and the maximum irradiance of your device, the tool will check if the power density is within safe physiological limits.

**Q: Can I calculate how long a session should last?**
Yes. The `calculate_exposure_parameters` tool calculates the required exposure time in minutes based on your device's irradiance, the treatment area, and your specific goal (skin, recovery, or mood).

**Q: How deep will the light penetrate my skin?**
The `estimate_depth_penetration` tool provides a penetration tier (Superficial, Medium, or Deep) based on the wavelength of the light you are using.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/red-light-therapy-dosage-calculator](https://vinkius.com/en/ai-agent-connect/red-light-therapy-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Red Light Therapy Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `red-light-therapy-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Red Light Therapy Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "red-light-therapy-dosage-calculator": {
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
