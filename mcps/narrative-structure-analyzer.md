# Narrative Structure Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/narrative-structure-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [linguistics](../categories/linguistics.md)

Detect storytelling frameworks, tension ratios, and compositional quality in long-form copy.

## Description
The Narrative Structure Analyzer connects AI agents to deep linguistic analysis of storytelling. Using tools like `analyze_framework_alignment`, `calculate_narrative_balance`, and `assess_compositional_quality`, it identifies if your text follows StoryBrand SB7, Hero's Journey, or Before-After-Bridge patterns. It provides concrete metrics on narrative tension, protagonist identity (customer vs. brand), sensory density, and pacing variance to help you optimize engagement.


## Available Tools (3)
- **analyze_framework_alignment**: Identifies which storytelling framework the text follows
- **assess_compositional_quality**: Calculates sensory density and pacing variance
- **calculate_narrative_balance**: Evaluates the tension-resolution ratio and protagonist identity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Narrative Structure Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for StoryBrand SB7 alignment: 'Meet John. He struggled with messy spreadsheets until he found our tool, which simplified his life.'"

**🤖 AI Agent:**
> Detected Framework: StoryBrand SB7. Completeness Score: 0.6. Stages present: Character, Problem, Guide, Plan.

---

**👤 You:**
> "What is the tension-resolution ratio for this paragraph: 'The storm raged, destroying everything in its path. Finally, the sun broke through the clouds and peace returned.'"

**🤖 AI Agent:**
> Tension-Resolution Ratio: 0.85. The text heavily emphasizes the problem stage.

---

**👤 You:**
> "Check the pacing of this narrative arc: 'Once upon a time, there was a small village. A dragon arrived suddenly and burned it all. The hero fought back bravely.'"

**🤖 AI Agent:**
> Pacing Variance Score: 0.42. Significant fluctuations in sentence length detected across the arc.


## ❓ FAQ

**Q: What storytelling frameworks can be detected?**
The tool identifies StoryBrand SB7, Hero's Journey, and Before-After-Bridge structures.

**Q: How do I measure the tension in my copy?**
Use the `calculate_narrative_balance` tool to find the ratio of problem-oriented word counts versus resolution-oriented segments.

**Q: Can this analyze sensory language?**
Yes, the `assess_compositional_quality` tool calculates a sensory density score based on concrete and sensory-driven language.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/narrative-structure-analyzer](https://vinkius.com/mcp/narrative-structure-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Narrative Structure Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `narrative-structure-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Narrative Structure Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "narrative-structure-analyzer": {
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
