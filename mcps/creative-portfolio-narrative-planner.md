# Creative Portfolio Narrative Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creative-portfolio-narrative-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [portfolio-management](../categories/portfolio-management.md)

A strategic planning tool that transforms creative works into a cohesive professional narrative.

## Description
This MCP server provides a suite of strategic tools to help creators build professional portfolios. Use `plan_portfolio_narrative` to generate a high-level strategic blueprint, `validate_rights_compliance` to ensure legal readiness, `develop_captions` for tailored descriptive tasks, and `generate_publication_checklist` for a final verification before going public. It connects your creative history to your professional future.


## Available Tools (4)
- **generate_publication_checklist**: Produces a final verification list to ensure the portfolio is ready for public viewing
- **validate_rights_compliance**: Checks if the planned publication strategy respects the legal constraints of the individual works
- **plan_portfolio_narrative**: Generates the high-level strategic blueprint for a professional portfolio
- **develop_captions**: Generates specific descriptive tasks and directions for individual work captions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creative Portfolio Narrative Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan my portfolio. My goal is to become a Senior Art Director, and I want to show my technical mastery and emotional impact."

**🤖 AI Agent:**
> To achieve your goal of becoming a Senior Art Director, we will group your works into three chapters: Technical Precision, Emotional Resonance, and Commercial Versatility. This structure will highlight your core strengths while demonstrating your readiness for leadership roles.

---

**👤 You:**
> "Check if I can publish my recent photography series on my personal website."

**🤖 AI Agent:**
> Based on the metadata provided, your photography series is under FullOwnership, meaning you are fully compliant to publish it on your personal website.

---

**👤 You:**
> "I need help writing captions for my new illustration set. The tone should be minimalist and the audience is high-end gallery owners."

**🤖 AI Agent:**
> For your minimalist illustration set, focus on brevity and negative space. Use keywords like 'essence', 'form', and 'subtlety' to appeal to gallery owners.


## ❓ FAQ

**Q: How do I create a strategic plan for my portfolio?**
You can use the `plan_portfolio_narrative` tool by providing your chosen works, career goals, and target audience to generate a cohesive blueprint.

**Q: Can this tool help with legal compliance?**
Yes, the `validate_rights_compliance` tool checks if your publication strategy respects the legal constraints of your individual works.

**Q: How do I ensure my captions match my brand voice?**
The `develop_captions` tool generates specific instructions for writing captions that incorporate your preferred voice and audience profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creative-portfolio-narrative-planner](https://vinkius.com/en/ai-agent-connect/creative-portfolio-narrative-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creative Portfolio Narrative Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creative-portfolio-narrative-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creative Portfolio Narrative Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creative-portfolio-narrative-planner": {
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
