# Multi-Policy Overlap Map MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/multi-policy-overlap-map)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Identify overlapping and distinct insurance benefits from multiple policies.

## Description
This MCP server provides specialized tools for insurance claim triage. It maps incident descriptions against verbatim policy benefit lists to identify exact overlaps and unique coverage. Use `find_benefit_overlaps` to detect shared benefits, `generate_contact_plan` to prioritize insurers, `generate_document_request_list` to identify required paperwork, and `summarize_coverage_gap` to find uncovered elements.


## Available Tools (4)
- **generate_document_request_list**: Produces a list of required policy documents
- **find_benefit_overlaps**: Identifies shared and unique benefits based on the incident description
- **generate_contact_plan**: Creates an ordered list of insurance providers to notify
- **summarize_coverage_gap**: Identifies elements in the incident not covered by any policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-Policy Overlap Map** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find overlaps for an incident involving 'Broken Arm' with policies containing ['Broken Arm', 'Medical Care'] and ['Broken Arm', 'Dental']."

**🤖 AI Agent:**
> The overlapping benefit is 'Broken Arm', which is present in both policies.

---

**👤 You:**
> "Generate a contact plan for the following overlap analysis: { "overlaps": [ { "term": "Emergency Room Visit", "policy_ids": [1, 2] } ] }"

**🤖 AI Agent:**
> Priority 1: Policy 1 and Policy 2 should be contacted first due to the overlapping 'Emergency Room Visit' benefit.

---

**👤 You:**
> "What documents are needed for an overlap of 'Dental Cleaning' in policy 3?"

**🤖 AI Agent:**
> The required document for policy 3 is the Dental Cleaning coverage statement.


## ❓ FAQ

**Q: How does the tool determine if a benefit is overlapping?**
A benefit is considered overlapping if its exact term exists in more than one policy list provided to `find_benefit_overlaps`.

**Q: Does the tool interpret policy language?**
No. The tool follows a strict matching rule and only identifies matches based on verbatim terms found in the policy lists.

**Q: How can I see what is not covered?**
You can use the `summarize_coverage_gap` tool to identify elements in the incident description that do not have a verbatim match in any policy list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/multi-policy-overlap-map](https://vinkius.com/en/ai-agent-connect/multi-policy-overlap-map)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-Policy Overlap Map** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multi-policy-overlap-map` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-Policy Overlap Map** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-policy-overlap-map": {
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
