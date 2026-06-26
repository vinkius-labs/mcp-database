# Time Signature Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/time-signature-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate measure duration, rhythmic feeling, and polyrhythms for any time signature.

## Description
This MCP server provides a precise musical metric engine. Use `get_measure_duration` to find the exact duration of a measure in milliseconds, `analyze_meter_structure` to identify if a meter is Simple, Compound, or Add/Asymmetric, and `calculate_rhythmic_relationships` to discover possible polyrhythms and rhythmic equivalences based on your BPM and time signature.


## Available Tools (3)
- **analyze_meter_structure**: Analyze the rhythmic feeling and subdivision of a time signature
- **calculate_rhythmic_relationships**: Find polyrhythms and meter equivalences
- **get_measure_duration**: e.g., 4 for quarter note). Returns total ms and pulse unit name.

Calculate the duration of one measure in milliseconds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Time Signature Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long is one measure in 4/4 at 120 BPM?"

**🤖 AI Agent:**
> One measure at 120 BPM in 4/4 lasts 2000 milliseconds.

---

**👤 You:**
> "What is the rhythmic feeling of 6/8 time?"

**🤖 AI Agent:**
> The 6/8 time signature has a Compound metric feeling.

---

**👤 You:**
> "What polyrhythms can I play over 3/4?"

**🤖 AI Agent:**
> Possible polyrhythms for 3/4 include ratios like 2:3 or 3:2 relative to the pulse.


## ❓ FAQ

**Q: How do I calculate the duration of a measure?**
Use the `get_measure_duration` tool by providing the BPM, the numerator (beats per measure), and the denominator value (e.g., 4 for quarter notes).

**Q: Can this tool identify compound meters?**
Yes, the `analyze_meter_structure` tool will determine if your time signature is Simple, Compound, or Additive.

**Q: How do I find polyrhythms for a specific tempo?**
Use the `calculate_rhythmic_relationships` tool with your time signature parameters to see possible rhythmic ratios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/time-signature-calculator](https://vinkius.com/mcp/time-signature-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Time Signature Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `time-signature-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Time Signature Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "time-signature-calculator": {
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
