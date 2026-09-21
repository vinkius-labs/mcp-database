# Acupuncture Point Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/acupuncture-point-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Select optimal acupuncture point combinations based on symptoms and TCM diagnosis.

## Description
This MCP server provides clinical decision support for Traditional Chinese Medicine (TCM) practitioners. It allows AI agents to identify synergistic acupuncture point formulas using `select_point_formula` based on patient symptoms and diagnostic patterns. Practitioners can also use `get_needling_parameters` to determine precise needle depth and retention times, `get_treatment_schedule` to plan course frequency, and `validate_point_safety` to ensure point combinations are appropriate for specific patient profiles, such as pregnancy status.


## Available Tools (4)
- **get_needling_parameters**: Provides technical physical administration data for a specific set of points
- **get_treatment_schedule**: Determines the recommended frequency and duration of a treatment course
- **select_point_formula**: Finds the optimal set of acupuncture points for a specific clinical presentation
- **validate_point_safety**: Checks if a specific point combination is contraindicated for a patient's profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acupuncture Point Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a point formula for a patient with acute lower back pain and Liver Qi Stagnation for pain relief."

**🤖 AI Agent:**
> The recommended points for acute lower back pain with Liver Qi Stagnation are BL23, BL40, and LV3. These points work together to regulate Qi flow and alleviate local tension.

---

**👤 You:**
> "What is the recommended treatment schedule for a chronic headache condition?"

**🤖 AI Agent:**
> For chronic headache conditions, the recommended schedule is 2 sessions per week for a total of 10 sessions to achieve long-term regulation.

---

**👤 You:**
> "Is the combination of LI4 and LV3 safe for a pregnant patient?"

**🤖 AI Agent:**
> No, the combination is not safe. LI4 is strictly contraindicated during pregnancy.


## ❓ FAQ

**Q: How does the tool determine point combinations?**
The `select_point_formula` tool analyzes provided symptoms and TCM diagnoses to select a synergistic group of points that address both the root and manifestation of the condition.

**Q: Can I check if a point combination is safe for pregnant patients?**
Yes, the `validate_point_safety` tool checks point combinations against patient profiles, including pregnancy status, to identify contraindications.

**Q: Does this provide physical administration details?**
Yes, using `get_needling_parameters`, the tool provides specific needle depth ranges and recommended retention times for the selected points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/acupuncture-point-selector](https://vinkius.com/en/ai-agent-connect/acupuncture-point-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acupuncture Point Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acupuncture-point-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acupuncture Point Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acupuncture-point-selector": {
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
