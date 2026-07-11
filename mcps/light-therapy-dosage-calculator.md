# Light Therapy Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/light-therapy-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates precise light therapy dosages for blue and red light treatments.

## Description
The Light Therapy Dosage Calculator provides exact exposure durations, energy density, and safety protocols for LED-based photobiomodulation. Using tools like `compute_exposure_metrics` and `lookup_device_specs`, it calculates optimal treatment time in minutes based on device irradiance and target dose. It also includes critical safety checks via `validate_treatment_safety` to alert users about eye protection needs and contraindications.


## Available Tools (4)
- **generate_treatment_schedule**: Provides a recurring frequency recommendation
- **compute_exposure_metrics**: Calculates required treatment duration and energy density
- **lookup_device_specs**: Retrieves technical specifications for a known light therapy device
- **validate_treatment_safety**: Evaluates a planned treatment against safety protocols


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Light Therapy Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the specs for the 'Pro-Panel X1' device?"

**🤖 AI Agent:**
> The Pro-Panel X1 operates in the 630-660nm range with an irradiance of 50 mW/cm2 and a beam area of 100 cm2.

---

**👤 You:**
> "Calculate treatment time for 5 mW/cm2 irradiance and 5 J/cm2 target dose."

**🤖 AI Agent:**
> To achieve a dose of 5 J/cm2 at 5 mW/cm2, you need an exposure time of 1000 seconds, which is approximately 16.67 minutes.

---

**👤 You:**
> "Is it safe to use 450nm light if I have photosensitivity?"

**🤖 AI Agent:**
> The safety check indicates that for a dose of 2 J/cm2 at 450nm, you should be aware of potential contraindications if photosensitivity is listed.


## ❓ FAQ

**Q: How do I find my device's specifications?**
You can use the `lookup_device_specs` tool by providing the exact name of your device from our catalog to retrieve its wavelength and irradiance.

**Q: Does the calculator account for distance?**
Yes, when using `compute_exposure_metrics`, you can provide the distance from the device to adjust the effective irradiance.

**Q: Can it check for safety risks?**
Absolutely. The `validate_treatment_safety` tool checks your planned wavelength and dose against known contraindications and eye protection requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/light-therapy-dosage-calculator](https://vinkius.com/mcp/light-therapy-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Light Therapy Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `light-therapy-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Light Therapy Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "light-therapy-dosage-calculator": {
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
