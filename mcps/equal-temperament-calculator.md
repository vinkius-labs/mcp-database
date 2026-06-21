# Equal Temperament Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/equal-temperament-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate MIDI frequencies, interval deviations, and tuning system comparisons.

## Description
A mathematical engine for musical acoustics. Use `generate_midi_frequency_log` to get a full list of MIDI frequencies, `calculate_interval_deviations` to find cents deviation from Just Intonation, and `compare_tuning_supports` to analyze differences between Pythagorean, Meantone, and Equal systems.


## Available Tools (3)
- **calculate_interval_deviations**: Calculates deviations from Just Intonation
- **generate_midi_frequency_log**: Generates a MIDI frequency log
- **compare_tuning_systems**: Compares different tuning systems


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Equal Temperament Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a frequency log for A4 at 440Hz."

**🤖 AI Agent:**
> The MIDI frequency log has been generated, containing all 128 notes from C-1 to G9 based on a 440Hz reference.

---

**👤 You:**
> "How much does the Pythagorean system deviate from Just Intonation for a perfect fifth?"

**🤖 AI Agent:**
> The deviation for a perfect fifth in the Pythagorean system is approximately 2.3 cents compared to its pure ratio.

---

**👤 You:**
> "Compare tuning systems using 440Hz as reference."

**🤖 AI Agent:**
> The comparison report shows the trade-offs between Pythagorean, Meantone, and Equal temperament regarding interval purity.


## ❓ FAQ

**Q: What is the range of MIDI notes covered?**
The engine covers all 128 MIDI notes, from C-1 to G9.

**Q: Can I use a custom reference pitch?**
Yes, you can provide any positive frequency in Hz as the `referencePitch` for all tools.

**Q: How are deviations calculated?**
The `calculate_interval_deviations` tool compares the selected tuning system against pure Just Intonation ratios and returns the result in cents.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/equal-temperament-calculator](https://vinkius.com/mcp/equal-temperament-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Equal Temperament Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `equal-temperament-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Equal Temperament Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "equal-temperament-calculator": {
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
