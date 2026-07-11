# Survey Question Bias Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/survey-question-bias-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nlp](../categories/nlp.md)

Detect linguistic bias and structural flaws in survey questions using advanced NLP techniques.

## Description
The Survey Question Bias Detector identifies methodological errors in surveys and NPS questions. Use tools like `scan_leading_language` to find loaded words, `check_conjunction_complexity` for double-barreled questions, and `verify_scale_symmetry` to ensure balanced response options. It also evaluates cognitive load via `evaluate_cognitive_load` and detects confusing negation patterns with `identify_negation_confusion`.


## Available Tools (5)
- **identify_negation_confusion**: , that might create double negatives.

Detect double negatives in a question
- **scan_leading_language**: s., "amazing", "must").

Detect biased or leading language in a survey question
- **verify_scale_symmetry**: Check if a response scale is balanced
- **check_conjunction_complexity**: Identify double-barreled questions
- **evaluate_cognitive_load**: Assess the complexity and length of a question


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Survey Question Bias Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is 'Don't you agree that our service is excellent?' biased?"

**🤖 AI Agent:**
> The question contains loaded language ('excellent') which indicates high bias severity.

---

**👤 You:**
> "Check if 'How satisfied are you with the food and service?' is double-barreled."

**🤖 AI Agent:**
> Yes, this question is double-barreled because it uses the conjunction 'and' to combine two distinct topics: food and service.

---

**👤 You:**
> "Evaluate the cognitive load of: 'In the event that you find yourself in a situation where the product fails to meet your expectations, how would you rate us?'"

**🤖 AI Agent:**
> The risk level is high due to the word count and complex sentence structure.


## ❓ FAQ

**Q: How does it detect leading language?**
The `scan_leading_language` tool compares your text against a lexicon of loaded words to identify potential bias.

**Q: Can I check for double-barreled questions?**
Yes, use the `check_conjunction_complexity` tool to find conjunctions like 'and' or 'or' that merge multiple concepts.

**Q: Does it support NPS scales?**
Yes, use `verify_scale_symmetry` to check if your response labels are balanced and include a neutral midpoint.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/survey-question-bias-detector](https://vinkius.com/mcp/survey-question-bias-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Survey Question Bias Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `survey-question-bias-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Survey Question Bias Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "survey-question-bias-detector": {
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
