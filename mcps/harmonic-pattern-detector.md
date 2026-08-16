# Harmonic Pattern Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harmonic-pattern-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify Gartley, Butterfly, Bat, and Crab patterns using Fibonacci ratios.

## Description
This MCP server provides deterministic detection of harmonic price patterns. It uses precise Fibonacci retracement and extension ratios to identify Gartley, Butterfly, Bat, and Crab structures. Use `detect_patterns` to scan price pivots for completed patterns, `get_pattern_details` to retrieve specific Potential Reversal Zone (PRZ) boundaries and target levels, or `validate_pivot_sequence` to extract candidate points from raw price data.


## Available Tools (3)
- **detect_patterns**: Scan a sequence of price pivots to identify any completed harmonic patterns
- **get_pattern_details**: Retrieve deep technical specifications for a specific detected pattern
- **validate_pivot_sequence**: Verify if a raw sequence of price points can form the basis of a harmonic pattern


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harmonic Pattern Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you detect any harmonic patterns in these pivots: [{"price": 100, "timestamp": 1}, {"price": 150, "timestamp": 2}, {"price": 125, "timestamp": 3}, {"price": 140, "timestamp": 4}, {"price": 110, "timestamp": 5}]?"

**🤖 AI Agent:**
> A Gartley pattern has been detected with a valid ratio within the 2% tolerance.

---

**👤 You:**
> "What are the target levels for this detected Bat pattern?"

**🤖 AI Agent:**
> The target levels for the Bat pattern are $115.50 (TP1) and $122.00 (TP2).

---

**👤 You:**
> "Check if this price series has enough points for pattern detection: [10, 12, 11, 13, 12, 14, 13]"

**🤖 AI Agent:**
> The sequence is valid and contains 4 potential pivot points.


## ❓ FAQ

**Q: How do I detect a pattern?**
You can use the `detect_patterns` tool by providing a JSON string of pivot objects containing price and timestamp.

**Q: What patterns are supported?**
The server supports Gartley, Butterfly, Bat, and Crab patterns.

**Q: How is the Potential Reversal Zone (PRZ) calculated?**
The PRZ is calculated based on the convergence of the D point extension and the final leg's retracement, which you can retrieve using `get_pattern_details`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harmonic-pattern-detector](https://vinkius.com/mcp/harmonic-pattern-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harmonic Pattern Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `harmonic-pattern-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harmonic Pattern Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harmonic-pattern-detector": {
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
