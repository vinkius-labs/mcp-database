# Dialogue Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dialogue-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [writing](../categories/writing.md)

Analyze manuscript text to determine the distribution of dialogue versus narration.

## Description
This MCP server provides tools for authors and editors to analyze the composition of their manuscripts. By specifying custom quotation delimiters, you can use `analyze_manuscript_text` to calculate the exact percentage of dialogue versus narration. You can also use `get_manuscript_summary` to check if a text is dialogue-heavy, `find_dialogue_segments` to locate specific spoken parts, and `validate_delimiter_pairs` to ensure your parsing characters are logically sound.


## Available Tools (4)
- **find_dialogue_segments**: 
- **get_manuscript_summary**: 
- **validate_delimiter_pairs**: 
- **analyze_manuscript_text**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dialogue Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text: He said, "Hello!" She replied, "Hi there." How much is the dialogue ratio?"

**🤖 AI Agent:**
> The dialogue ratio is 50%. There are 4 dialogue words and 4 narration words.

---

**👤 You:**
> "Is this text dialogue-heavy? Text: "Wait!" he shouted. "No way!" she yelled."

**🤖 AI Agent:**
> Yes, the text is dialogue-heavy as the dialogue makes up more than half of the total word count.

---

**👤 You:**
> "Find all the dialogue segments in: The cat sat. 'Meow,' said the cat. 'Purr,' it added."

**🤖 AI Agent:**
> The dialogue segments are: 'Meow' (1 word) and 'Purr' (1 word).


## ❓ FAQ

**Q: How do I define my quotation marks?**
You provide the specific characters used as start and end delimiters in the tool inputs. For example, use double quotes (") for standard English text.

**Q: Can I use non-standard symbols for dialogue?**
Yes, as long as the delimiters are distinct and follow an alternating pattern, you can use any character or string to mark dialogue.

**Q: What is considered a 'word' in the analysis?**
A word is defined as any sequence of characters separated by whitespace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dialogue-ratio-calculator](https://vinkius.com/en/ai-agent-connect/dialogue-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dialogue Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dialogue-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dialogue Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dialogue-ratio-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
