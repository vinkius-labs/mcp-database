# CRISPR Guide Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crispr-guide-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [genetics](../categories/genetics.md)

Design optimal CRISPR guide RNAs by analyzing PAM sites, efficiency, and off-target risks.

## Description
This MCP server provides a specialized toolset for CRISPR-Cas9 genome editing design. It allows AI agents to identify valid PAM sites using `find_pam_sites`, generate candidate sequences with `design_grna_sequences`, predict effectiveness via `evaluate_on_target_efficiency`, and mitigate unintended cleavage risks with `assess_off_target_risk`. It is designed to help researchers balance high on-target efficiency with minimal off-target effects.


## Available Tools (4)
- **assess_off_target_risk**: Predicts the danger of unintended cleavage by searching the genome for similar sequences
- **design_grna_sequences**: Generates candidate guide RNA sequences based on identified target locations and PAM sites
- **evaluate_on_target_efficiency**: Calculates the predicted effectiveness of specific guide sequences at their intended target
- **find_pam_sites**: g., "NGG").

Identifies all valid locations within a target gene where a PAM sequence exists to allow Cas9 binding


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CRISPR Guide Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all NGG PAM sites in the sequence ATGCGGATGCGG."

**🤖 AI Agent:**
> Found PAM sites at positions 4 and 10 with sequence NGG.

---

**👤 You:**
> "Design gRNA sequences for the target sequence GCTAGCTAGCTAGCTAGCTA with PAM sites at 5 and 15."

**🤖 AI Agent:**
> Generated 2 candidate guides: GCTAGCTAGCTAGCTAGCTAG (pos 5, score 0.85) and TAGCTAGCTAGCTAGCTAGC (pos 15, score 0.78).

---

**👤 You:**
> "What is the off-target risk for the guide sequence GCTAGCTAGCTAGCTAGCTA in the provided genome?"

**🤖 AI Agent:**
> The risk profile shows 0 potential off-target sites with significant mismatch counts in the seed region.


## ❓ FAQ

**Q: How do I identify valid target locations?**
You can use the `find_pam_sites` tool by providing the target DNA sequence and the required PAM motif, such as NGG.

**Q: Can I check for off-target risks?**
Yes, the `assess_off_target_risk` tool predicts the danger of unintended cleavage by searching the provided genome reference for similar sequences.

**Q: How is guide efficiency calculated?**
The `evaluate_on_target_efficiency` tool calculates scores based on nucleotide composition and the position of nucleotides relative to the PAM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crispr-guide-designer](https://vinkius.com/ai-agent-connect/crispr-guide-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CRISPR Guide Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crispr-guide-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CRISPR Guide Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crispr-guide-designer": {
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
