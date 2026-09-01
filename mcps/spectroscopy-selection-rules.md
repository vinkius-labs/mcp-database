# Spectroscopy Selection Rules MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/spectroscopy-selection-rules)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Determines spectroscopic selection rules and transition moments for quantum states.

## Description
This MCP server provides tools to analyze quantum state transitions. It determines if a transition is allowed or forbidden based on parity and angular momentum conservation. Users can use `analyze_transition_possibility` to check multipole expansion validity, `calculate_transition_moment` to find transition strength, `list_forbidden_transitions` to identify prohibited paths, and `validate_quantum_state` to ensure physical correctness of quantum numbers.


## Available Tools (4)
- **validate_quantum_state**: Checks the physical validity of a single quantum state definition
- **analyze_transition_possibility**: Determines if a transition between two specific quantum states is allowed or forbidden under different multipole expansions
- **calculate_transition_moment**: Computes the strength of the transition between two states
- **list_forbidden_transitions**: Identifies which transitions from a given state are forbidden within a specific set of allowed multipole types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spectroscopy Selection Rules** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the transition from a state with n=2, l=0 to n=2, l=1 allowed?"

**🤖 AI Agent:**
> Yes, the transition is allowed under electric dipole (E1) rules as it satisfies the parity change requirement.

---

**👤 You:**
> "Calculate the transition moment for an E1 transition between the provided states."

**🤖 AI Agent:**
> The calculated transition moment is 0.85, which is classified as a Strong transition.

---

**👤 You:**
> "List all forbidden transitions from the ground state to the following target states."

**🤖 AI Agent:**
> The transition to the state with l=0 is forbidden due to parity conservation violation.


## ❓ FAQ

**Q: How do I check if a transition is allowed?**
You can use the `analyze_transition_possibility` tool by providing the initial and final state quantum numbers as JSON strings.

**Q: Can I calculate the strength of an E1 transition?**
Yes, use the `calculate_transition_moment` tool and specify 'E1' as the multipole type.

**Q: How can I verify my quantum numbers are physically valid?**
The `validate_quantum_state` tool checks if your quantum numbers obey standard physical constraints like $l < n$.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/spectroscopy-selection-rules](https://vinkius.com/ai-agent-connect/spectroscopy-selection-rules)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spectroscopy Selection Rules** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spectroscopy-selection-rules` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spectroscopy Selection Rules** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spectroscopy-selection-rules": {
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
