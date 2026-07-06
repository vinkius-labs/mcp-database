# FOIA.gov (Freedom of Information) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/foiagov-freedom-of-information)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access US government FOIA data — list agency components, retrieve request forms, and fetch annual reports directly from FOIA.gov.

## Description
Connect to the **FOIA.gov** API to streamline access to Freedom of Information Act data. This MCP server allows AI agents to navigate the complex structure of US government agencies and their specific FOIA requirements through natural conversation.

### What you can do

- **Agency Discovery** — List all FOIA agency components and filter by specific fields like titles and abbreviations.
- **Component Details** — Fetch deep metadata for specific agency components using their unique UUIDs.
- **Request Forms** — Retrieve the exact structure and fields required for FOIA request forms for any specific component.
- **Annual Reports** — Access NIEM-standard XML annual reports for agencies by year to analyze transparency metrics.

### How it works

1. Subscribe to this server
2. Enter your FOIA.gov API Key
3. Start querying government transparency data from your AI assistant

### Who is this for?

- **Journalists & Researchers** — quickly identify which agency components handle specific types of records.
- **Legal Professionals** — automate the retrieval of request form structures to ensure compliance with agency-specific requirements.
- **Data Analysts** — pull annual report data in XML format for large-scale transparency analysis.


## Available Tools (4)
- **list_agency_components**: Supports JSON API sparse fieldsets and includes.

List all FOIA agency components
- **get_agency_component_request_form**: Fetch the FOIA request form structure for a specific component
- **get_agency_component**: Fetch a specific agency component by UUID
- **get_annual_report_xml**: Fetch an agency annual report in XML format


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FOIA.gov (Freedom of Information)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all FOIA agency components and include their parent agency names."

**🤖 AI Agent:**
> I've retrieved the list of agency components. There are several hundred components across departments like the DOJ, DOD, and DHS. Would you like to filter this list by a specific keyword or agency abbreviation?

---

**👤 You:**
> "Get the FOIA request form structure for the agency component with UUID '654321-abc-...'."

**🤖 AI Agent:**
> I have the form structure for that component. It requires fields such as 'Description of Records', 'Fee Waiver Request', and 'Expedited Processing'. I can provide the specific JSON schema for these fields if you need to build a submission.

---

**👤 You:**
> "Fetch the 2021 annual report XML for the DOJ."

**🤖 AI Agent:**
> I've successfully retrieved the 2021 Annual FOIA Report for the Department of Justice in XML format. The report includes detailed statistics on requests received, processed, and pending, as well as processing times.


## ❓ FAQ

**Q: How can I find the specific requirements for filing a FOIA request with an agency?**
You can use the `get_agency_component_request_form` tool with the agency's UUID. It will return the full structure of the form, including all required fields and instructions.

**Q: Is it possible to list all sub-components of a major government agency?**
Yes. Use `list_agency_components` and you can include the parent agency information to filter or identify all components belonging to a specific department.

**Q: Can I access the raw annual transparency reports for data analysis?**
Absolutely. The `get_annual_report_xml` tool allows you to fetch the official NIEM-standard XML reports for any agency and year (e.g., DOJ, 2021).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foiagov-freedom-of-information](https://vinkius.com/mcp/foiagov-freedom-of-information)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FOIA.gov (Freedom of Information)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foiagov-freedom-of-information` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FOIA.gov (Freedom of Information)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foiagov-freedom-of-information": {
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
