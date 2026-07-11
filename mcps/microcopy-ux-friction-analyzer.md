# Microcopy UX Friction Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microcopy-ux-friction-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Audit UX microcopy for clarity, friction, and actionability.

## Description
The Microcopy UX Friction Analyzer helps designers and writers identify linguistic barriers in user interfaces. Using tools like `evaluate_clarity_metrics`, `detect_linguistic_friction`, `verify_actionability`, `assess_reading_complexity`, and `check_element_redundancy`, this MCP server analyzes error messages, labels, and tooltips to reduce cognitive load. It detects jargon, identifies user-blaming language, checks for action verbs, and flags redundant text elements.


## Available Tools (5)
- **assess_reading_complexity**: Ensure microcopy aligns with the target demographic's reading proficiency
- **check_element_redundancy**: Prevent information overlap between different UI microcopy components
- **detect_linguistic_friction**: Identify if microcopy is blaming the user or has a tone mismatch
- **evaluate_clarity_metrics**: Determine how difficult a specific text string is to understand
- **verify_actionability**: Check if an error message or instruction provides a clear path forward


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microcopy UX Friction Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this error message for friction: 'You entered the wrong password.'"

**🤖 AI Agent:**
> The message contains blame language. A more neutral alternative is: 'Password does and not match our records.'

---

**👤 You:**
> "Is the text 'Please click the submit button to continue' actionable?"

**🤖 AI Agent:**
> Yes, the message is actionable because it contains the instruction verb 'click'.

---

**👤 You:**
> "Check if this label and input hint are redundant: Label: 'Email', Hint: 'Enter your email address'"

**🤖 AI Agent:**
> A redundancy score of 0.8 was detected because the hint repeats information found in the label.


## ❓ FAQ

**Q: What does the clarity metric measure?**
It calculates jargon density and average word length to determine how difficult a text string is to understand.

**Q: How can I detect user-blaming language?**
Use the `detect_linguistic_friction` tool to identify passive or accusatory phrasing in your error messages.

**Q: Can this tool check for redundant UI elements?**
Yes, the `check_element_redundancy` tool compares labels, input hints, and helper text to find semantic overlaps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microcopy-ux-friction-analyzer](https://vinkius.com/mcp/microcopy-ux-friction-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microcopy UX Friction Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microcopy-ux-friction-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microcopy UX Friction Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microcopy-ux-friction-analyzer": {
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
