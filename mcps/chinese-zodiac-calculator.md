# Chinese Zodiac Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chinese-zodiac-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Discover your Chinese zodiac animal, element, and astrological compatibility.

## Description
The Chinese Zodiac Calculator connects AI agents to the ancient wisdom of the 12-year zodiac cycle. Using tools like `get_zodiac_details`, `check_compatibility`, and `get_animal_profile`, you can uncover the specific animal, element (Wood, Fire, Earth, Metal, or Water), and polarity (Yin/Yang) associated with any birth year. It also provides deep insights into personality traits and how different signs interact through astrological harmony or clashes.


## Available Tools
- **get_animal_profile**: s. Monkey, Rat, etc.) to see its characteristics.

Get detailed profile for a specific zodiac animal
- **check_compatibility**: Check astrological compatibility between two years
- **get_zodiac_details**: Get detailed astrological profile for a birth year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chinese Zodiac Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my zodiac sign if I was born in 1990?"

**🤖 AI Agent:**
> In 1990, your Chinese zodiac animal is the Horse, with the Metal element and Yang polarity.

---

**👤 You:**
> "Are a Dragon and a Rat compatible?"

**🤖 AI Agent:**
> The relationship between the Dragon and the Rat is typically highly compatible due to their harmonious alignment in the zodiac cycle.

---

**👤 You:**
> "Tell me about the Tiger animal profile."

**🤖 AI Agent:**
> The Tiger is known for its strength and bravery, but may face challenges with impulsiveness. Compatible signs include Horse and Dog.


## ❓ FAQ

**Q: What information can I get for a specific birth year?**
By using the `get_zodiac_details` tool, you can retrieve the zodiac animal, the associated element, the polarity (Yin or Yang), and a list of key personality traits for that year.

**Q: How does the compatibility tool work?**
The `check_compatibility` tool compares two birth years to determine if the relationship is Highly Compatible, Neutral, or a Clash based on traditional zodiac groupings.

**Q: Can I learn more about a specific animal?**
Yes, the `get_animal_profile` tool provides a deep dive into an animal's strengths, weaknesses, and compatible or incompatible signs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chinese-zodiac-calculator](https://vinkius.com/mcp/chinese-zodiac-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chinese Zodiac Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chinese-zodiac-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chinese Zodiac Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chinese-zodiac-calculator": {
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
