# Sample Offset Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sample-offset-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media-production](../categories/media-production.md)

Convert between milliseconds and exact audio samples for precise DAW alignment.

## Description
The Sample Offset Calculator is a specialized tool for digital audio engineers. It provides high-precision conversions between time in milliseconds and discrete audio sample counts. Using tools like `ms_to_samples`, `samples_to_ms`, and `verify_alignment`, you can ensure perfect rhythmic accuracy and phase alignment in your Digital Audio Workstation (DAW). This is critical for preventing timing drift when working with standard sample rates such as 44.1kHz, 48kHz, and 96kHz.


## Available Tools (3)
- **ms_to_samples**: Convert milliseconds to audio samples
- **samples_to_ms**: Convert audio samples to milliseconds
- **verify_alignment**: Verify if a sample count aligns with millisecond boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sample Offset Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many samples are in 500ms at a 48kHz sample rate?"

**🤖 AI Agent:**
> At a sample rate of 48000 Hz, 500 milliseconds corresponds to exactly 24,000 samples.

---

**👤 You:**
> "Convert 12000 samples to milliseconds at 44100 Hz."

**🤖 AI Agent:**
> 12,000 samples at 44100 Hz is approximately 272.11 milliseconds.

---

**👤 You:**
> "Does 44100 samples at 48kHz align perfectly with a millisecond boundary?"

**🤖 AI Agent:**
> No, 44,100 samples at 48,000 Hz results in 918.75 ms, meaning there is a drift of 0.75 ms.


## ❓ FAQ

**Q: What sample rates are supported?**
The calculator supports industry-standard rates: 44100 Hz, 48000 Hz, and 96000 Hz.

**Q: How does `verify_alignment` work?**
The `verify_alignment` tool checks if a specific sample count corresponds exactly to a whole number of milliseconds. If there is a fractional remainder, it calculates the `driftMs` value.

**Q: Can I use this for 96kHz audio?**
Yes, the tool is designed for high-resolution production and supports 96000 Hz.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sample-offset-calculator](https://vinkius.com/mcp/sample-offset-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sample Offset Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sample-offset-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sample Offset Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sample-offset-calculator": {
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
