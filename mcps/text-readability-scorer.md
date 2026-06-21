# Text Readability Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/text-readability-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate mathematically accurate readability metrics (Flesch-Kincaid, Gunning Fog, SMOG) for any text. Stop relying on AI 'feelings' — get exact US grade levels for SEO and compliance.

## Description
You ask your AI copywriter: 'Is this blog post easy to read?' It says 'Yes, it is very engaging!' Then you run it through a real SEO tool and it scores at a university reading level — killing your mobile bounce rate.

LLMs cannot accurately count syllables or calculate sentence complexity. This MCP uses the `text-readability` library to execute standard linguistic formulas, providing mathematical proof of how difficult your text is to read.

### The Superpowers

- **Flesch-Kincaid Grade Level:** The industry standard. Returns a number corresponding to the US grade level (e.g., 8.2 = 8th grade).
- **Flesch Reading Ease:** A 0-100 scale where higher is easier. Essential for broad audience copy.
- **Multiple Algorithms:** Also calculates Gunning Fog, Coleman-Liau, SMOG, and Automated Readability Index (ARI).
- **Consensus Evaluation:** Automatically aggregates all scores to give you a definitive target audience level.


## Available Tools
- **readability_scorer**: Essential for SEO, marketing, and legal compliance.

Calculate rigorous readability metrics for any text (Flesch-Kincaid, Gunning Fog, SMOG, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Text Readability Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this landing page copy. We need it to be at an 8th-grade reading level to maximize conversions."

**🤖 AI Agent:**
> Flesch-Kincaid Grade: 11.4 | Reading Ease: 42.1 | Consensus: 11th and 12th grade. Too complex. Needs simplification.

---

**👤 You:**
> "Our legal team says the new Terms of Service must be readable by a 6th grader. Verify the text."

**🤖 AI Agent:**
> Flesch-Kincaid Grade: 6.2 | Reading Ease: 78.5 | Meets compliance requirement for 6th-grade readability.

---

**👤 You:**
> "Check the SMOG Index and Gunning Fog for this medical article before we publish it."

**🤖 AI Agent:**
> SMOG: 14.2 | Gunning Fog: 15.8 | Highly academic. Requires college-level reading comprehension.


## ❓ FAQ

**Q: Why can't the LLM just estimate the reading level?**
Readability formulas (like Flesch-Kincaid) require exact mathematical counts of syllables per word and words per sentence. LLMs operate on sub-word tokens, not syllables, making them notoriously bad at these calculations. This engine uses deterministic linguistic math.

**Q: What is a good Flesch Reading Ease score for web content?**
For general consumer web content, aim for 60-70. This translates to an 8th-9th grade reading level, which is easily understood by 80% of adults. Legal or academic texts usually score in the 30s or lower.

**Q: Does this work for non-English text?**
The formulas (Flesch, Fog, SMOG) were developed and calibrated specifically for the English language based on English syllable structures. While the engine will calculate a score for other languages, the grade-level mapping is only statistically accurate for English.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/text-readability-scorer](https://vinkius.com/mcp/text-readability-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Text Readability Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `text-readability-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Text Readability Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "text-readability-scorer": {
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
