# Muscle Energy Technique Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/muscle-energy-technique-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Generates precise Muscle Energy Technique (MET) protocols for clinical use.

## Description
This MCP server provides clinical decision support for therapists using Muscle Energy Technique (MET). It allows for the generation of structured protocols via `get_met_protocol`, verification of muscle suitability with `validate_muscle_eligibility`, calculation of physical load using `calculate_session_load`, and retrieval of manual cues through `get_technique_instructions`. The tool adapts contraction intensity and duration based on client tolerance to ensure safe and effective treatment.


## Available Tools (4)
- **get_met_protocol**: Generates a complete, structured MET session protocol based on clinical inputs
- **get_technique_instructions**: Provides verbal cues and manual positioning guidance for the therapist
- **validate_muscle_eligibility**: Checks if a specific muscle is suitable for the requested MET type
- **calculate_session_load**: Determines the cumulative physical load of the session to prevent over-treatment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Muscle Energy Technique Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a post-isometric protocol for the trapezius muscle with moderate client tolerance."

**🤖 AI Agent:**
> Protocol generated: Contraction Intensity: 50% MVC, Duration: 7 seconds, Repetitions: 3, Stretch Force: Moderate.

---

**👤 You:**
> "Is the hamstrings muscle eligible for reciprocal inhibition?"

**🤖 AI Agent:**
> Yes, the hamstrings are eligible for reciprocal inhibition techniques.

---

**👤 You:**
> "What are the verbal cues for a post-isometric technique?"

**🤖 AI Agent:**
> Verbal cues: 'Contract the muscle against my resistance, hold, and now relax into the stretch.'


## ❓ FAQ

**Q: How do I generate a full treatment protocol?**
You can use the `get_met_protocol` tool by providing the restricted muscle, the MET type, and the client's tolerance level.

**Q: Can I check if a muscle is safe for a specific technique?**
Yes, use `validate_muscle_eligibility` to check if a muscle group is suitable for post-isometric or reciprocal inhibition techniques.

**Q: How does the tool handle patient comfort?**
The tool uses the `clientTolerance` input to scale contraction intensity and stretch force, ensuring the protocol remains within safe limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/muscle-energy-technique-guide](https://vinkius.com/en/ai-agent-connect/muscle-energy-technique-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Muscle Energy Technique Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `muscle-energy-technique-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Muscle Energy Technique Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "muscle-energy-technique-guide": {
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
