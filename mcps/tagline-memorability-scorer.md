# Tagline Memorability Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tagline-memorability-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze taglines for phonetic, rhythmic, and structural memorability.

## Description
The Tagline Memorability Scorer evaluates the linguistic strength of slogans. Using tools like `analyze_phonetic_features` and `calculate_memorability_score`, it detects alliteration, rhyme, and optimal word counts to predict consumer recall and impact.


## Available Tools (4)
- **analyze_phonetic_features**: Detect recurring sounds in a tagline
- **analyze_rhythm_and_meter**: Examine cadence and syllable distribution
- **calculate_memorability_score**: Calculate a unified memorability metric
- **analyze_structural_pattern**: Evaluate linguistic construction and length


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tagline Memorability Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the tagline 'Just Do It' for memorability."

**🤖 AI Agent:**
> The tagline 'Just Do It' has a word count of 3, which is within the optimal range. The score is high due to its imperative structure and brevity.

---

**👤 You:**
> "Check the phonetic features of 'Peter Piper picked a peck of pickled peppers'."

**🤖 AI Agent:**
> Alliteration is detected with repeated 'p' sounds. Assonance is also present.

---

**👤 You:**
> "What is the rhythm pattern for 'Think Different'?"

**🤖 AI Agent:**
> The syllable count is 3, and the rhythmic pattern is irregular.


## ❓ FAQ

**Q: What can this tool analyze?**
It analyzes phonetic features, rhythm, structural patterns, and provides a final memorability score.

**Q: Does it support different languages?**
The analysis is optimized for English taglines to ensure accurate syllable and rhyme detection.

**Q: How do I use the scoring feature?**
Use the `calculate_memorability_score` tool with your tagline as input to get a unified metric.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tagline-memorability-scorer](https://vinkius.com/mcp/tagline-memorability-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tagline Memorability Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tagline-memorability-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tagline Memorability Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tagline-memorability-scorer": {
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
