# Subtitle Readability Pacer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/subtitle-readability-pacer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Calculate optimal subtitle block distribution and timing based on speaking rate.

## Description
The Subtitle Readability Pacer is a calculation engine designed to prevent reading fatigue by ensuring subtitles do not move faster than the human eye can process. Using tools like `calculate_speaking_rate`, `check_readability_risk`, and `generate_subtitle_blocks`, it analyzes text density and duration to maintain optimal viewing comfort. The system enforces a strict 15 Characters Per Second (CPS) threshold and ensures no subtitle block exceeds 42 characters per line or two lines in total, mathematically slicing segments into timestamped blocks that match the original duration.


## Available Tools (3)
- **check_readability_risk**: Assess the readability risk of a subtitle segment
- **calculate_speaking_rate**: Calculate characters per second (CPS) for a segment
- **generate_subtitle_blocks**: Generate split subtitle blocks based on character limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subtitle Readability Pacer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the speaking rate for a segment with 300 characters and a duration of 10 seconds."

**🤖 AI Agent:**
> The speaking rate is 30.0 characters per second (CPS).

---

**👤 You:**
> "Is a segment with 100 characters and 10 seconds duration at risk of being unreadable?"

**🤖 AI Agent:**
> No, the risk level is Low because the rate is 10 CPS, which is below the 15 CPS threshold.

---

**👤 You:**
> "Generate subtitle blocks for a segment of 120 characters lasting 8 seconds."

**🤖 AI Agent:**
> The segment has been split into 2 blocks: Block 1 (0-4000ms, 60 chars) and Block 2 (4000-8000ms, 60 chars).


## ❓ FAQ

**Q: How does the tool determine if a subtitle is readable?**
The tool uses `check_readability_risk` to evaluate the Characters Per Second (CPS). If the rate exceeds 15 CPS, it flags a high risk level and suggests fragmentation.

**Q: Can I split long segments into multiple blocks?**
Yes, the `generate_subtitle_blocks` tool automatically decomposes heavy segments into multiple timestamped blocks that satisfy character and duration constraints.

**Q: What are the character limits per line?**
To prevent eye strain, the engine ensures no single line exceeds 42 characters and no block contains more than two lines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/subtitle-readability-pacer](https://vinkius.com/mcp/subtitle-readability-pacer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subtitle Readability Pacer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subtitle-readability-pacer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subtitle Readability Pacer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subtitle-readability-pacer": {
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
