# Defective Delivery Report MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/defective-delivery-report)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [e-commerce](../categories/e-commerce.md)

Generate factual defect reports and evidence-preservation plans for damaged deliveries.

## Description
This MCP server provides a suite of tools to handle delivery disputes. Use `generate_defect_report` to create structured, objective descriptions of product damage. Use `create_preservation_plan` to receive specific instructions on maintaining physical evidence. You can also use `create_submission_strategy` to follow seller-specific claim protocols and `analyze_liability_factors` to determine if the carrier, seller, or product is responsible for the issue.


## Available Tools (4)
- **create_preservation_plan**: Generates a list of actions to ensure physical evidence remains valid for a formal dispute
- **create_submission_strategy**: Develops a step-by-step guide for submitting the claim to the seller according to their specific protocols
- **generate_defect_report**: Creates a factual, structured description of the defect based on the provided evidence and order details
- **analyze_liability_factors**: Evaluates whether the fault likely lies with the carrier, the seller (packaging), or the product itself


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Defective Delivery Report** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a defect report for order #12345 where the box was crushed and the item inside is broken."

**🤖 AI Agent:**
> Defect Report ID: DR-98765. Summary: The external packaging was crushed upon arrival, resulting in a broken internal product component. Severity: High.

---

**👤 You:**
> "How do I submit a claim for order #54321 via the web portal?"

**🤖 AI Agent:**
> To submit your claim via the web portal for order #54321, follow these steps: 1. Log in to the seller's portal. 2. Navigate to 'My Orders'. 3. Select 'Report Issue'. 4. Upload the required photos and submit.

---

**👤 You:**
> "Analyze liability for order #11223 where the packaging was intact but the product failed."

**🤖 AI Agent:**
> The likely fault party is the Seller or Product Quality, as the packaging remained intact while the product was damaged.


## ❓ FAQ

**Q: How do I generate a formal report?**
Use the `generate_defect_report` tool with the order ID, damage photos, packaging notes, and a description of the defect.

**Q: Can I find out who is responsible for the damage?**
Yes, the `analyze_liability_factors` tool evaluates whether the fault lies with the carrier, the seller, or the product.

**Q: What should I do with the damaged packaging?**
Run the `create_preservation_plan` tool to get specific instructions on which items and packaging components you must keep to satisfy the seller's requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/defective-delivery-report](https://vinkius.com/en/ai-agent-connect/defective-delivery-report)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Defective Delivery Report** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `defective-delivery-report` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Defective Delivery Report** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "defective-delivery-report": {
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
