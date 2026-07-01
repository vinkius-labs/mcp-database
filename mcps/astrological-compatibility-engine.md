# Astrological Compatibility Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/astrological-compatibility-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze zodiac compatibility using elemental and modal synergy.

## Description
This MCP server provides a deep analytical engine for evaluating astrological connections. By processing sun, moon, and ascendant signs, it calculates multi-dimensional compatibility scores across love, communication, values, and attraction. Use `lookup_sign_properties` to find zodiac attributes, `analyze_elemental_synergy` to check elemental bonds, or `generate_compatibility_report` for a full relationship assessment.


## Available Tools (3)
- **generate_compatibility_report**: Returns multi-dimensional scores and summary.

Generates a full astrological compatibility report
- **lookup_sign_properties**: g., "Aries"). Returns element and modality.

Retrieves elemental and modal attributes for a zodiac sign
- **analyze_elemental_synergy**: Returns affinity score and interaction type.

Evaluates relationship between two elements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Astrological Compatibility Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the elemental synergy between Fire and Water?"

**🤖 AI Agent:**
> The interaction between Fire and Water is classified as Challenging, with a lower affinity score due to their opposing natures.

---

**👤 You:**
> "Check the compatibility of an Aries Sun with a Leo Sun."

**🤖 AI Agent:**
> The compatibility between Aries and Leo is high, showing strong synergy in Love (95), Communication (85), Values (70), and Attraction (90) due to their shared Fire element.

---

**👤 You:**
> "What are the properties of the sign Taurus?"

**🤖 AI Agent:**
> Taurus belongs to the Earth element and possesses a Fixed modality.


## ❓ FAQ

**Q: What zodiac signs are supported?**
The engine supports all twelve zodiac signs: Aries, Taurus, Gemini, Cancer, Leo, Virgo, Libra, Scorpio, Sagittarius, Capricorn, Aquarius, and Pisces.

**Q: How is the compatibility score calculated?**
Scores are derived from elemental affinities (e.g., Fire/Air) and modal interactions (Cardinal, Fixed, Mutable) between the provided planetary placements.

**Q: Can I include Moon or Ascendant signs?**
Yes, while Sun signs are the primary driver, providing Moon and Ascendant signs allows for a more nuanced and accurate compatibility report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/astrological-compatibility-engine](https://vinkius.com/mcp/astrological-compatibility-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Astrological Compatibility Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `astrological-compatibility-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Astrological Compatibility Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "astrological-compatibility-engine": {
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
