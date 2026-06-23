# Emotion Wheel Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emotion-wheel-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [psychology](../categories/psychology.md)

Map raw text descriptions to Plutchik's Wheel of Emotions, identifying intensity and emotional families.

## Description
The Emotion Wheel Classifier connects AI agents to the psychological depth of Plutchik's model. Use `analyze_text_emotion` to transform unstructured text into specific emotional nodes, intensities (Low, Medium, High), and families. You can also use `get_emotion_spectrum` to see how an emotion evolves in strength or `explore_emotional_dyad` to calculate the complex emotions resulting from combining two primary states.


## Available Tools (3)
- **explore_emotional_dyad**: Calculate the resulting complex emotion from two primary emotions
- **get_emotion_spectrum**: Show the progression of a specific emotion
- **analyze_text_emotion**: Analyze raw text to identify emotion, intensity, and family


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emotion Wheel Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I feel extremely happy and full of energy!"

**🤖 AI Agent:**
> The `analyze_text_emotion` tool identifies the primary emotion as Joy with a High intensity level.

---

**👤 You:**
> "I am slightly afraid of the dark."

**🤖 AI Agent:**
> The `analyze_text_emotion` tool identifies the primary emotion as Fear with a Low intensity level.

---

**👤 You:**
> "What happens if I combine Joy and Trust?"

**🤖 AI Agent:**
> Using `explore_emotional_dyad` with Joy and Trust results in the complex emotion of Love.


## ❓ FAQ

**Q: How does the tool identify emotions?**
The `analyze_text_emotion` tool interprets the weight and descriptors in your text to map it to a specific node on Plutchik's wheel, determining intensity levels like Low or High.

**Q: Can I see the progression of an emotion?**
Yes, using `get_emotion_spectrum`, you can retrieve the three-tier intensity names (Low, Medium, High) for any primary emotion.

**Q: What are emotional dyads?**
Dyads are complex emotions formed by combining two primary ones. The `explore_emotional_dyad` tool calculates the resulting state and its complexity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emotion-wheel-classifier](https://vinkius.com/mcp/emotion-wheel-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emotion Wheel Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emotion-wheel-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emotion Wheel Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emotion-wheel-classifier": {
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
