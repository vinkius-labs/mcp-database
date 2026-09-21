# Stretch Duration Prescriber MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/stretch-duration-prescriber)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates personalized stretching protocols based on muscle group, flexibility, and goals.

## Description
This MCP server provides precise stretching prescriptions tailored to physiological needs. By analyzing muscle groups, flexibility levels, and specific training goals like recovery or flexibility gain, it calculates optimal hold times, sets, and session frequency. Use `prescribe_stretch_protocol` to generate a complete routine, `evaluate_muscle_suitability` to check safety for specific goals, `get_modality_recommendations` to choose between static and dynamic movements, and `calculate_session_intensity` to determine the correct tension level.


## Available Tools (4)
- **calculate_session_intensity**: Determines the recommended intensity/tension level for the stretch
- **evaluate_muscle_suitability**: Determines if a specific goal is appropriate for a given muscle group and flexibility level
- **get_modality_recommendations**: Suggests whether to use static or dynamic stretching based on the user's context
- **prescribe_stretch_protocol**: Generates a complete stretching routine for a specific muscle and goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stretch Duration Prescriber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a stretching protocol for my hamstrings. I have low flexibility and my goal is flexibility gain. I am 30 years old."

**🤖 AI Agent:**
> For your hamstrings with low flexibility aiming for flexibility gain, perform 3 sets of static stretches with a hold time of 45 seconds each. Repeat this routine 3 times per week.

---

**👤 You:**
> "I want to recover after a run. My goal is recovery, I have moderate flexibility, and I am 25."

**🤖 AI Agent:**
> For recovery, perform dynamic stretches for 10 minutes. This will help increase blood flow and regulate your nervous system.

---

**👤 You:**
> "Is it safe to try to gain flexibility in my hip flexors if my flexibility is low?"

**🤖 AI Agent:**
> Aggressive flexibility gain might be contraindicated for hip flexors at low flexibility levels; it is recommended to start with controlled movements.


## ❓ FAQ

**Q: How do I get a full stretching routine?**
You can use the `prescribe_stretch_protocol` tool by providing the target muscle, your flexibility level, your goal, and your age.

**Q: Can I check if a stretch is safe for my current flexibility?**
Yes, use the `evaluate_muscle_suitability` tool to determine if a specific goal is appropriate for your muscle group and mobility level.

**Q: What determines the intensity of the stretch?**
The `calculate_session_intensity` tool determines the recommended tension level based on your flexibility and training objective.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/stretch-duration-prescriber](https://vinkius.com/en/ai-agent-connect/stretch-duration-prescriber)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stretch Duration Prescriber** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stretch-duration-prescriber` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stretch Duration Prescriber** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stretch-duration-prescriber": {
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
