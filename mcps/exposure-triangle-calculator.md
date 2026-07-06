# Exposure Triangle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exposure-triangle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate missing exposure parameters, ND filter compensation, and film reciprocity corrections.

## Description
The Exposure Triangle Calculator is a precision utility for photographers to maintain consistent light levels. Use `calculate_missing_parameter` to find the third variable (ISO, Aperture, or Shutter Speed) when two are known. The tool also provides `apply_nd_compensation` to adjust settings for Neutral Density filters, `get_film_correction` to handle film reciprocity failure in analog photography, and `generate_exposure_variations` to explore different aperture and shutter speed combinations that maintain the same exposure value.


## Available Tools (4)
- **generate_exposure_variations**: Generates a list of alternative aperture and shutter speed combinations for the same EV
- **get_film_correction**: Calculates the necessary shutter speed adjustment for film reciprocity failure
- **calculate_missing_parameter**: Calculates a missing exposure parameter (ISO, Aperture, Shutter Speed, or EV)
- **apply_nd_compensation**: g., "ND8").

Calculates the required exposure adjustments for an ND filter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exposure Triangle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am using ISO 400 and f/5.6. What should my shutter speed be for a sunny day?"

**🤖 AI Agent:**
> To maintain the same exposure, your shutter speed should be 1/250s.

---

**👤 You:**
> "I'm adding an ND8 filter to my current settings of f/8 and 1/60s. What are my new settings?"

**🤖 AI Agent:**
> With the ND8 filter, your adjusted settings should be f/5.6 and 1/15s to compensate for the 3 stops lost.

---

**👤 You:**
> "Show me different aperture and shutter speed options for f/4 at 1/100s."

**🤖 AI Agent:**
> Here are the variations: f/2.8 at 1/200s, f/5.6 at 1/50s, and f/8 at 1/25s.


## ❓ FAQ

**Q: How do I find the correct shutter speed if I know my aperture and ISO?**
You can use the `calculate_missing_parameter` tool. Simply provide your current aperture and ISO, and it will calculate the required shutter speed to maintain the same exposure.

**Q: Does this tool account for ND filters?**
Yes, the `apply_nd_compensation` tool allows you to input your base aperture and shutter speed along with an ND filter factor (like 'ND8') to calculate the necessary adjustments.

**Q: Can I use this for analog film photography?**
Absolutely. The `get_film_correction` tool specifically calculates the shutter speed extension needed to compensate for reciprocity failure in different film types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exposure-triangle-calculator](https://vinkius.com/mcp/exposure-triangle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exposure Triangle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exposure-triangle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exposure Triangle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exposure-triangle-calculator": {
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
