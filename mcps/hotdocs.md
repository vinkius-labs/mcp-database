# HotDocs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hotdocs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate document assembly via HotDocs Advance — list templates, create work items, conduct interviews, and generate documents directly from any AI agent.

## Description
Connect your **HotDocs Advance** tenancy to any AI agent and take full control of your document automation workflows through natural conversation.

### What you can do

- **Template Discovery** — List all template packages and their versions available in your HotDocs tenancy
- **Work Item Management** — Create, inspect, and manage work items that hold interview data and assembled documents
- **Interview Sessions** — Initialize interview sessions programmatically for interactive data collection
- **Automated Document Assembly** — Inject answers via XML and trigger document generation without manual UI interaction
- **Document Retrieval** — List and download assembled documents (PDFs, Word docs) directly from the agent
- **Validation & Auditing** — Check unanswered variables, list work items by date range or user, and audit assembly history

### How it works

1. Subscribe to this server
2. Enter your HotDocs Advance tenancy, API client name, service principal name, and password
3. Start automating your document workflows from Claude, Cursor, or any MCP-compatible client

No more repetitive clicking through the HotDocs web interface. Your AI acts as a dedicated document automation specialist.

### Who is this for?

- **Legal Teams** — instantly generate contracts, agreements, and legal forms by providing case details in natural language
- **HR Departments** — automate offer letters, employment contracts, and policy documents at scale
- **Financial Services** — assemble loan applications, compliance forms, and client onboarding documents rapidly
- **Operations & Compliance** — batch-generate standardized documents and audit interview completeness across teams


## Available Tools (14)
- **complete_assembly**: This processes all collected answers and assembles the final documents based on the template configuration.
After calling this, the assembled documents become available for download via list_documents and get_document_content.
You must have already created a work item, created a version/session, and provided answers (via interview or update_answers).
The workItemId and versionId must match an existing work item and its version.

Complete document assembly for a work item version
- **create_interview_session**: This endpoint prepares the system to collect answers for the template variables.
The response contains interview data needed to render the HotDocs interview UI.
Use this before displaying the interview to the user or before assembling documents.
The versionId should be unique for each interview session (e.g., v1, v2, or a UUID).

Create a new interview session for a work item
- **create_work_item**: A work item is associated with a specific template package and holds answers provided during interviews.
You must provide a unique workItemId (alphanumeric identifier you choose) and optionally a templatePackageId.
The workItemId becomes the reference for all subsequent operations (interview, assembly, download).
IMPORTANT: workItemId must be unique and URL-safe (letters, numbers, hyphens only).

Create a new work item in HotDocs Advance
- **get_auth_token**: This is primarily a utility function for debugging authentication issues.
The token is used internally by all other tools automatically.
If other tools fail with auth errors, verify your credentials are correct.

Get a fresh HotDocs API access token
- **get_document_content**: Use this to download the final generated document (PDF, Word, etc.) after assembly is complete.
You need the workItemId and the documentId (obtained from list_documents).
The response includes the document content and a download URL for direct access.

Download/get content of an assembled document
- **get_template_package**: Use the template package ID obtained from list_template_packages.
This helps understand the template structure before creating work items.

Get details of a specific template package
- **get_unanswered_variables**: This shows which template variables were not provided answers during the interview process.
Useful for validating interview completeness before or after document assembly.
Requires the workItemId and documentId (from list_documents).
The response includes the list of unanswered variables and assembly results.

Get unanswered variables from an assembled document
- **get_work_item**: Use this to inspect a work item before or after 
conducting interviews or assembling documents. The workItemId is the unique identifier you 
assigned when creating the work item.

Get details of a specific work item
- **list_documents**: After completing assembly, this shows all generated documents with their IDs, names, and metadata.
Use the document IDs returned here to download individual documents via get_document_content.
Each document entry includes filename, creation date, and assembly results information.

List all assembled documents for a work item
- **list_template_versions**: Each template can have multiple versions over time. This shows version history 
and helps identify which version is currently live/active.
Use the package_id from list_template_packages to query versions.

List all versions of a template package
- **list_template_packages**: Template packages define the structure of documents that can be assembled. 
Each package contains interview questions and document output configurations.
Use this to discover what templates are available for document assembly.
The response includes package IDs which are required for creating work items.

List all available template packages in HotDocs Advance
- **list_work_items_by_date**: This is optimized for 
date-based filtering and auditing. Both fromDate and toDate are required for this tool.
Use ISO 8601 date format (e.g., 2024-01-01 or 2024-01-01T00:00:00 for datetime).
This is useful for generating reports on document assembly activity over time periods.

List work items filtered by a specific date range
- **list_work_items**: You can filter by user ID 
and/or date range to find specific work items. Leave all parameters empty to list all work items.
This is useful for auditing, tracking progress, or finding existing work items to continue working on.
Date format should be ISO 8601 (e.g., 2024-01-15 or 2024-01-15T10:30:00).

List work items with optional filters
- **update_answers**: The answer_xml parameter must contain valid HotDocs answer XML format that matches the template variables.
This is useful for automated/batch document assembly where you already have the data.
You can call this multiple times to incrementally add answers.
Answer XML format example: <AnswerSet><A v="VariableName"><V>Answer Value</V></A></AnswerSet>

Update answers for a work item using XML answer format


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HotDocs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available template packages in my HotDocs tenancy."

**🤖 AI Agent:**
> I've fetched your template packages. You currently have 3 template packages available: 'Employment Contract Template' (ID: emp-ctr-001), 'NDA Template' (ID: nda-std-002), and 'Service Agreement Template' (ID: svc-agr-003). Which template would you like to use for document assembly?

---

**👤 You:**
> "Create a new work item 'contract-2024-001' using the employment contract template and assemble a document with these details: employee name is John Smith, position is Software Engineer, start date is March 1st 2024, salary is $95,000."

**🤖 AI Agent:**
> I've completed the full document assembly workflow:
1. Created work item 'contract-2024-001' successfully
2. Injected the employee data as answer XML
3. Completed document assembly

The document is now ready. I found 1 assembled document: 'Employment_Contract_John_Smith.docx' (Document ID: doc-789456). Would you like me to download it for you?

---

**👤 You:**
> "Show me all work items created in the last 30 days and check if there are any unanswered variables in the documents."

**🤖 AI Agent:**
> I found 8 work items created in the date range 2024-03-08 to 2024-04-07. Checking documents for unanswered variables... I noticed 2 work items have incomplete interviews with unanswered variables: 'contract-2024-005' has 3 unanswered variables (emergency_contact, benefits_selection, stock_options) and 'nda-2024-012' has 1 unanswered variable (jurisdiction_state). Would you like me to provide the details of these unanswered variables?


## ❓ FAQ

**Q: What credentials do I need to connect HotDocs Advance to this MCP server?**
You need four pieces of information: (1) your **Tenancy Moniker** (the subdomain in your HotDocs URL, e.g., 'mycompany' from mycompany.hotdocsadvance.com), (2) the **API Client Display Name** you created in Manage API Credentials, (3) the **Service Principal Name** you added to that client, and (4) the **Service Principal Password** (which is shown only once during creation). All of these are obtained from the HotDocs Advance Auth portal.

**Q: Can I assemble documents automatically without going through the interview UI?**
Yes! Use the `create_work_item` tool to initialize a work item, then use `update_answers` to inject your data as HotDocs answer XML, and finally call `complete_assembly` to trigger document generation. This fully automated bypasses the interactive interview UI entirely, perfect for batch processing or integrating with external data sources.

**Q: How do I find and download documents that have already been assembled?**
Use the `list_documents` tool with your workItemId to see all assembled documents and their IDs. Then use `get_document_content` with the workItemId and documentId to retrieve the actual file content. The response includes both the raw content and a direct download URL for easy access to your PDFs or Word documents.

**Q: What is a work item and why is it important?**
A work item is a unique container in HotDocs Advance that holds interview answers, template associations, and assembled documents for a specific case. Think of it as a 'file folder' for each document automation request. It's identified by a unique ID you assign (like 'contract-john-doe-2024') and persists all data so you can revisit, update, and reassemble documents at any time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hotdocs](https://vinkius.com/mcp/hotdocs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HotDocs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hotdocs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HotDocs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotdocs": {
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
