# Surf Coaching Certification Pathway Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-coaching-certification-pathway-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Maps professional development roadmaps for surf coaches by analyzing credentials and career goals.

## Description
This MCP server provides a structured way for surf coaches to navigate their professional growth. By connecting to various international governing bodies, it allows AI agents to calculate specific certification requirements, identify experience gaps, and generate step-by-step career roadmaps. Use `calculate_coaching_pathway` to build a complete development plan or `analyze_experience_gap` to see exactly what is needed for a specific tier.


## Available Tools (4)
- **calculate_coaching_pathway**: Generates a step-by-step roadmap from current status to career goal
- **analyze_experience_gap**: Identifies the specific deficiencies preventing a coach from reaching the next tier
- **get_available_organizations**: Lists all coaching organizations supported by the system
- **get_certification_details**: Retrieves the specific requirements for a single certification within an organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Coaching Certification Pathway Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 12 months of experience and a Level 1 certification. What is my path to becoming a Professional Coach in the International organization?"

**🤖 AI Agent:**
> To reach the Professional Coach level, you first need to complete the Level 2 certification, which requires 24 total months of experience. Your current roadmap includes: 1. Level 2 Certification (requires 12 more months of experience).

---

**👤 You:**
> "What am I missing to get the Advanced Instructor certification in the USA organization?"

**🤖 AI Agent:**
> You are currently missing the 'Safety Specialist' certification and 6 months of additional coaching experience to qualify for the Advanced Instructor level.

---

**👤 You:**
> "List all the coaching organizations available."

**🤖 AI Agent:**
> The supported organizations are: International Surf Association (Global), USA Surf Academy (USA), and EuroSurf (Europe).


## ❓ FAQ

**Q: How do I know which certifications I need?**
You can use the `analyze_experience_gap` tool to identify exactly which certifications or months of experience are missing to reach your target level.

**Q: Can I plan a full career path?**
Yes, the `calculate_coaching_pathway` tool generates a complete, step-by-step roadmap from your current status to your ultimate career goal.

**Q: What organizations are supported?**
You can call `get_available_organizations` to see a full list of the coaching organizations currently supported by this server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-coaching-certification-pathway-mapper](https://vinkius.com/en/ai-agent-connect/surf-coaching-certification-pathway-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Coaching Certification Pathway Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-coaching-certification-pathway-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Coaching Certification Pathway Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-coaching-certification-pathway-mapper": {
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
