# Singlish Authenticity Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singlish-authenticity-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze the linguistic authenticity of Singlish text using particle density and syntax patterns.

## Description
This MCP server provides a deterministic engine to evaluate how authentic Singlish text is. It analyzes the frequency and variety of core particles like 'lah', 'leh', and 'lor', and calculates a density score. Use `analyze_singlish_composition` for a full statistical breakdown, `check_usage_saturation` to detect if the usage is 'try-hard', or `validate_syntax_patterns` to identify specific idiomatic constructions like 'Can or not?'.


## Available Tools (3)
- **check_usage_saturation**: Specifically identifies if the Singlish usage is perceived as "overused" or "try-hard"
- **analyze_singlish_composition**: Provides a high-level statistical breakdown of Singlish usage in a given text
- **validate_syntax_patterns**: Checks if the text contains specific, recognizable Singlish grammatical patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singlish Authenticity Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text: 'Can or not? I don't know leh.'"

**🤖 AI Agent:**
> { "particleCounts": { "lah": 0, "leh": 1, "lor": 0, "meh": 0, "mah": 0, "sia": 0, "liao": 0 }, "particleDensity": 0.14, "authenticityScore": 85, "detectedConstructions": ["Can or not?"] }

---

**👤 You:**
> "Is this text overused: 'Lah lah lah lah lah!'"

**🤖 AI Agent:**
> { "isOverused": true, "density": 0.83 }

---

**👤 You:**
> "Check the syntax of 'Never mind lah'."

**🤖 AI Agent:**
> { "patternsFound": ["Never mind lah"], "patternCount": 1 }


## ❓ FAQ

**Q: What is considered an authentic Singlish density?**
An optimal density for natural Singlish is between 0.1 and 0.3. If the density exceeds 0.5, the text is flagged as 'overused' or 'try-hard'.

**Q: How does the authenticity score work?**
The score is a weighted metric based on particle variety and whether the density falls within the natural 0.1 to 0.3 range.

**Q: Can I check for specific grammatical patterns?**
Yes, you can use `validate_syntax_patterns` to detect idiomatic structures like 'Can or not?' or 'Never mind lah'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singlish-authenticity-scorer](https://vinkius.com/ai-agent-connect/singlish-authenticity-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singlish Authenticity Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singlish-authenticity-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singlish Authenticity Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singlish-authenticity-scorer": {
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
