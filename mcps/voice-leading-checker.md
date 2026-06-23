# Voice Leading Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/voice-leading-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze musical voice-leading integrity between chord voicings using classical harmonic principles.

## Description
The Voice Leading Checker is an analytical engine designed to evaluate the movement of musical notes across four distinct melodic ranges: Bass, Tenor, Alto, and Soprano (SATB). By using tools like `analyze_voice_conduction`, `check_voice_hierarchy`, and `evaluate_smoothness`, AI agents can detect harmonic errors such as parallel fifths, parallel octaves, voice crossing, and excessive melodic leaps. This MCP server provides direct access to precise musical analysis, returning violation details, quality scores, and suggested alternative voicings to ensure smooth and correct harmonic transitions.


## Available Tools (3)
- **analyze_voice_conduction**: Analytes the conduction between two chord voicings
- **check_voice_hierarchy**: Validates that voices are in correct ascending order
- **evaluate_smoothness**: Evaluates the smoothness of a musical transition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Voice Leading Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this transition is harmonically correct: Initial {bass: 36, tenor: 48, alto: 55, soprano: 67} to Target {bass: 39, tenor: 51, alto: 58, soprano: 70}."

**🤖 AI Agent:**
> The `analyze_voice_conduction` tool has analyzed the transition. No parallel fifths or octaves were detected, and the movement is smooth.

---

**👤 You:**
> "Evaluate the smoothness of a transition with 2 violations and a leap magnitude sum of 12."

**🤖 AI Agent:**
> Using `evaluate_smoothness`, the quality grade is determined based on the error count and leap magnitude provided.

---

**👤 You:**
> "Is this voicing valid: Bass 40, Tenor 38, Alto 50, Soprano 60?"

**🤖 AI Agent:**
> The `check_voice_hierarchy` tool indicates this is invalid because the Tenor pitch (38) is lower than the Bass pitch (40), violating the required ascending order.


## ❓ FAQ

**Q: How can an agent detect parallel fifths?**
Agents use the `analyze_voice_conduction` tool, providing initial and target voicings. The tool identifies when two voices move in the same direction while maintaining a perfect fifth interval.

**Q: What does `check_voice_hierarchy` do?**
The `check_voice_hierarchy` tool ensures that the pitch values for Bass, Tenor, Alto, and Soprano are in correct ascending order, preventing voice crossing errors.

**Q: Can I get suggestions for better voicings?**
Yes. When using `analyze_voice_conduction`, the tool returns a `suggested_voicing` object containing an alternative arrangement that resolves detected violations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voice-leading-checker](https://vinkius.com/mcp/voice-leading-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Voice Leading Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `voice-leading-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Voice Leading Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "voice-leading-checker": {
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
