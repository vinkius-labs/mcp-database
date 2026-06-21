# FDA Drug Labels (openFDA) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fda-drug-labels-openfda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access official FDA drug labels and structured product labeling (SPL) data via openFDA.

## Description
Connect your AI agent to the official **openFDA** database to retrieve comprehensive drug label information and structured product labeling (SPL) data through natural conversation.

### What you can do

- **Label Search** — Search through thousands of prescription and over-the-counter (OTC) drug labels using brand names, generic names, or specific warnings.
- **Market Analysis** — Count unique values for fields like manufacturer names to understand the competitive landscape of specific medications.
- **Detailed Metadata** — Access precise information including active ingredients, dosage forms, indications, and usage instructions.
- **Advanced Filtering** — Use Lucene query syntax to filter results by effective time, product type, or specific FDA identifiers.

### How it works

1. Subscribe to this server
2. Enter your openFDA API Key
3. Start querying drug information directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Professionals** — quickly retrieve drug warnings and label information without navigating complex government portals.
- **Researchers & Analysts** — perform market analysis by counting manufacturers and tracking new drug label submissions.
- **Developers** — integrate real-time, official FDA data into health-tech applications and research tools.


## Available Tools
- **count_drug_labels**: Count unique values of a field in FDA drug labels
- **search_drug_labels**: Use the search parameter to filter by fields like openfda.brand_name, warnings, etc.

Search FDA drug labels (SPL format)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FDA Drug Labels (openFDA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for FDA drug labels for 'Tylenol' and show the warnings."

**🤖 AI Agent:**
> I've found the labels for Tylenol. The warnings section includes information about liver warning (acetaminophen), allergy alert, and directions for use. Would you like the full text of the 'warnings' field?

---

**👤 You:**
> "Count the unique manufacturers for drugs with the brand name 'Advil'."

**🤖 AI Agent:**
> Based on the openFDA data, there are several unique manufacturer entries associated with 'Advil', including 'GlaxoSmithKline Consumer Healthcare Holdings (US) LLC' and 'Pfizer Consumer Healthcare'.

---

**👤 You:**
> "Find the 5 most recent drug labels for 'Amoxicillin'."

**🤖 AI Agent:**
> I've retrieved the 5 most recent labels for Amoxicillin, sorted by effective time. The latest updates come from manufacturers like 'Aurobindo Pharma Limited' and 'Teva Pharmaceuticals USA, Inc.'.


## ❓ FAQ

**Q: Can I search for a specific drug brand like 'Advil'?**
Yes! Use the `search_drug_labels` tool with a search parameter like `openfda.brand_name:"Advil"`. The agent will return the official SPL data including warnings and ingredients.

**Q: How can I find out how many different manufacturers produce a specific generic drug?**
You can use the `count_drug_labels` tool. Set the `count` parameter to `openfda.manufacturer_name.exact` and use the `search` parameter to filter by the generic name.

**Q: Is it possible to sort results by the most recent label updates?**
Yes. When using `search_drug_labels`, you can provide a `sort` parameter such as `effective_time:desc` to see the most recently updated labels first.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fda-drug-labels-openfda](https://vinkius.com/mcp/fda-drug-labels-openfda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FDA Drug Labels (openFDA)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fda-drug-labels-openfda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FDA Drug Labels (openFDA)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fda-drug-labels-openfda": {
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
