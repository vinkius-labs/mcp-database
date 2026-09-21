# Reflexology Zone Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reflexology-zone-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Maps reflexology zones to body organs to generate targeted treatment protocols.

## Description
This MCP connects AI agents to reflexology expertise. It uses specialized tools like `identify_target_zones` to map physical symptoms to specific anatomical reflex points on the hands or feet. Once zones are identified, the agent can use `calculate_treatment_parameters` to determine appropriate pressure and duration, and `generate_treatment_sequence` to create a structured clinical workflow. It also includes `verify_zone_safety` to ensure treatments are appropriate for the target organs and any known contraindications.


## Available Tools (4)
- **calculate_treatment_parameters**: Determines the physical application details (pressure and duration) for each identified zone
- **generate_treatment_sequence**: Organizes the identified zones into a logical, step-by-step clinical workflow
- **identify_target_zones**: Determines which specific reflex zones should be addressed based on reported symptoms and energy blockages
- **verify_zone_safety**: Validates that the requested treatment does not contraindicate specific physiological zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reflexology Zone Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have foot pain and digestive issues. Which reflex zones should I focus on?"

**🤖 AI Agent:**
> Based on your symptoms, the primary reflex zones to address are the digestive system areas located in the arch of the foot.

---

**👤 You:**
> "What is the recommended treatment sequence for hand reflexology targeting the head area?"

**🤖 AI Agent:**
> The sequence starts with preparatory clearing of the thumb base, followed by targeted stimulation of the head zones, and concludes with calming integration steps.

---

**👤 You:**
> "Can I use firm pressure on the kidney reflex zone if I have acute inflammation?"

**🤖 AI Agent:**
> No, acute inflammation is a contraindication that requires light pressure or avoidance of that specific zone to ensure safety.


## ❓ FAQ

**Q: How does the tool identify which areas to treat?**
The `identify_target_zones` tool analyzes the provided body part, symptoms, and energy blockages to find the corresponding reflex zones.

**Q: Can I customize the pressure used during treatment?**
Yes, you can specify a preference for light, medium, or firm pressure when using `calculate_treatment_parameters`.

**Q: Is the treatment sequence safe to follow?**
The `verify_zone_safety` tool checks the identified organs against any provided contraindications to ensure the protocol is safe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reflexology-zone-mapper](https://vinkius.com/en/ai-agent-connect/reflexology-zone-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reflexology Zone Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reflexology-zone-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reflexology Zone Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reflexology-zone-mapper": {
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
