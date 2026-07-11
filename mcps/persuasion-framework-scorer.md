# Persuasion Framework Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/persuasion-framework-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Scans copy for structural and persuasive patterns using Cialdini's principles and copywriting frameworks.

## Description
The Persuasion Framework Scorer analyzes text to detect the presence and strength of Cialdini's six principles: reciprocity, scarcity, authority, consistency, liking, and social proof. It also identifies classic copywriting frameworks such as AIDA, PAS, BAB, and FAB by calculating per-stage completeness scores. Additionally, it counts urgency/scarcity trigger phrases and evaluates Call-to-Action (CTA) strength by analyzing verb strength, specificity, and friction words. Use `analyze_cialdini` to find psychological triggers, `identify_framework` for structural analysis, `evaluate_cta` for CTA optimization, and `detect_urgency` to identify FOMO elements.


## Available Tools (4)
- **detect_urgency**: Detect urgency triggers in text
- **analyze_cialdini**: Analyze text for Cialdini principles of persuasion
- **evaluate_cta**: Evaluate the effectiveness of a Call to Action (CTA)
- **identify_framework**: Identify copywriting frameworks like PAS, AIDA, BAB, or FAB


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Persuasion Framework Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this ad copy for persuasion principles: 'Limited time only! Our expert-backed formula is used by thousands. Grab yours now before stocks run out!'"

**🤖 AI Agent:**
> Detected Principles: Scarcity ('Limited time only!', 'before stocks run out!'), Social Proof ('used by thousands'), and Authority ('expert-backed').

---

**👤 You:**
> "What framework is used in this text: 'Struggling with back pain? Our ergonomic chair fixes your posture instantly. Experience comfort today.'"

**🤖 AI Agent:**
> The text follows the PAS (Problem, Agitation, Solution) framework.

---

**👤 You:**
> "Evaluate this CTA: 'Click here to buy.'"

**🤖 AI Agent:**
> CTA Score: Low. Issues detected: Low verb strength and high friction due to lack of specificity.


## ❓ FAQ

**Q: What copywriting frameworks can be identified?**
The tool identifies common frameworks including AIDA (Attention, Interest, Desire, Action), PAS (Problem, Agitation, Solution), BAB (Before, After, Bridge), and FAB (Features, Advantages, Benefits).

**Q: How does the tool evaluate a Call to Action?**
By using `evaluate_cta`, the tool analyzes your text for verb strength, specificity of the offer, and the presence of friction words that might prevent conversion.

**Q: Can it detect psychological triggers?**
Yes, the `analyze_cialdini` tool specifically scans for the six principles of persuasion: reciprocity, scarcity, authority, consistency, liking, and social proof.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/persuasion-framework-scorer](https://vinkius.com/mcp/persuasion-framework-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Persuasion Framework Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `persuasion-framework-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Persuasion Framework Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "persuasion-framework-scorer": {
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
