# Body Scrub Duration Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/body-scrub-duration-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized body scrub session protocols based on skin sensitivity and goals.

## Description
This MCP server provides professional guidance for body exfoliation sessions. It uses specialized tools like `get_scrub_protocol` to generate complete session plans, including pressure guidance, area-specific timings, and rinse temperatures. You can also use `validate_scrub_parameters` to ensure a specific scrub type is safe for your skin sensitivity, or `get_area_specific_guidance` for localized instructions on specific body regions.


## Available Tools (4)
- **get_area_specific_guidance**: Provides localized instructions for a single body area within a session
- **get_scrub_protocol**: Generates a complete, personalized session plan for a body scrub
- **lookup_scrub_properties**: Retrieves the physical characteristics of a specific scrub type
- **validate_scrub_parameters**: Checks if a specific combination of inputs is safe and physically viable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Body Scrub Duration Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to do a sugar scrub on my arms and legs. My skin is sensitive and I want hydration."

**🤖 AI Agent:**
> For a sugar scrub on your arms and legs with sensitive skin, use light pressure. Recommended duration: Arms: 3 minutes, Legs: 5 minutes. Use lukewarm water for rinsing and apply moisturizer immediately after drying.

---

**👤 You:**
> "Is a salt scrub safe for highly sensitive skin on my torso?"

**🤖 AI Agent:**
> No, a salt scrub is too abrasive for highly sensitive skin and may cause irritation.

---

**👤 You:**
> "What are the properties of a coffee scrub?"

**🤖 AI Agent:**
> A coffee scrub typically has a medium grit level, a low hydration factor, and is best suited for normal to oily skin types.


## ❓ FAQ

**Q: How do I know if a scrub is safe for my skin?**
You can use the `validate_scrub_parameters` tool to check if your chosen scrub type is safe for your specific skin sensitivity level.

**Q: Can I get a full plan for my entire session?**
Yes, the `get_scrub_protocol` tool generates a complete plan including pressure, timing for each area, and rinse temperature.

**Q: Does it provide instructions for specific body parts?**
Yes, `get_area_specific_guidance` provides localized instructions, including recommended duration and intensity for specific regions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/body-scrub-duration-guide](https://vinkius.com/en/ai-agent-connect/body-scrub-duration-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Body Scrub Duration Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `body-scrub-duration-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Body Scrub Duration Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "body-scrub-duration-guide": {
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
