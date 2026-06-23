# Readability & SEO Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/readability-seo-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Audit text for SEO performance using Flesch-Kincaid, sentence density, and passive voice analysis.

## Description
The Readability & SEO Scorer MCP server provides a comprehensive audit of your content's linguistic structure. It calculates a customized Flesch-Kincaid Reading Ease score to determine how accessible your text is to readers. Beyond readability, the server uses `audit_density` to identify 'walls of text' by flagging overly long sentences and paragraphs that can hurt user engagement. Additionally, the `analyze_style` tool detects passive voice usage, helping you transform wordy prose into direct, engaging content. By integrating this server via Vinkius Edge, AI agents in Cursor, VS Code, or Claude Desktop can automatically evaluate text quality for optimal SEO performance.


## Available Tools (3)
- **audit_density**: Audit text for structural density issues
- **calculate_readability**: Calculate Flesch-Kincaid Reading Ease score
- **analyze_style**: Detect passive voice and analyze writing style


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Readability & SEO Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the readability score of this text: 'The quick brown fox jumps over the lazy dog.'"

**🤖 AI Agent:**
> The reading ease score for the provided text is 105.2, which falls into the 'very easy' complexity level.

---

**👤 You:**
> "Check this paragraph for structural density issues: 'This is a very long sentence that contains many words in order to test if the density audit tool can correctly identify it as a long sentence during the analysis process.'"

**🤖 AI Agent:**
> The audit identified 1 structural alert: The sentence exceeds the default word count threshold of 20 words.

---

**👤 You:**
> "Analyze this text for passive voice: 'The cake was eaten by the boy.'"

**🤖 AI Agent:**
> Detected 1 instance of passive voice. Suggestion: Use active voice, e.g., 'The boy ate the cake.'


## ❓ FAQ

**Q: How does the Flesch-Kincaid score work?**
The tool calculates a reading ease score based on the ratio of syllables to words and words to sentences. A higher score indicates easier-to-read text.

**Q: Can I detect long paragraphs?**
Yes, by using the `audit_density` tool, you can identify paragraphs that exceed character limits and sentences that are too long for optimal web reading.

**Q: Does it help with writing style?**
Yes, the `analyze_style` tool specifically looks for passive voice constructions and provides suggestions to make your writing more direct and engaging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/readability-seo-scorer](https://vinkius.com/mcp/readability-seo-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Readability & SEO Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `readability-seo-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Readability & SEO Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "readability-seo-scorer": {
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
