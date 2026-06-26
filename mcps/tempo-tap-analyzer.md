# Tempo Tap Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tempo-tap-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze rhythmic timing, BPM, and groove stability from tap sequences.

## Description
The Tempo Tap Analyzer is a specialized engine for musicians and musicologists to quantify musical groove and rhythm. By providing a series of millisecond timestamps, you can use `calculate_tempo_metrics` to derive average BPM and interval details, `analyze_timing_stability` to assess the precision (human vs. robotic feel) of a performance, and `identify_rhythmic_subdivision` to detect underlying patterns like Binary, Ternary, or Quaternary rhythms.


## Available Tools (3)
- **analyze_timing_stability**: Analyze the stability of a rhythmic sequence
- **identify_rhythmic_subdivision**: Detect the rhythmic pattern/subdivision
- **calculate_tempo_metrics**: g., [0, 500, 1000]). Returns average BPM and interval details.

Calculate BPM and intervals from tap timestamps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tempo Tap Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the BPM for these taps: [0, 500, 1000, 1500]"

**🤖 AI Agent:**
> The average BPM is 120. The intervals are all 500ms.

---

**👤 You:**
> "How stable is this rhythm: [480, 520, 490, 510]?"

**🤖 AI Agent:**
> The timing stability is high, indicating a very precise and robotic rhythm.

---

**👤 You:**
> "What subdivision is present in these intervals: [500, 750, 500, 750]?"

**🤖 AI Agent:**
> The detected subdivision is Ternary, with a high confidence score.


## ❓ FAQ

**Q: How do I calculate BPM from my taps?**
Use the `calculate_tempo_metrics` tool by providing an array of timestamps in milliseconds representing when each tap occurred.

**Q: How can I tell if my rhythm is 'human' or 'robotic'?**
Use the `analyze_timing_stability` tool. A high stability percentage indicates a robotic, metronomic feel, while lower stability suggests a more natural, human groove.

**Q: Can this tool detect triplets?**
Yes, by using `identify_rhythmic_subdivision`, the engine analyzes interval ratios to identify Ternary patterns, which include triplets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tempo-tap-analyzer](https://vinkius.com/mcp/tempo-tap-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tempo Tap Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tempo-tap-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tempo Tap Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tempo-tap-analyzer": {
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
