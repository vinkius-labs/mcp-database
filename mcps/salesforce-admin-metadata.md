# Salesforce Admin & Metadata MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-admin-metadata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage users, explore object schemas, monitor org limits, search metadata, execute Apex, and audit profiles through natural conversation.

## Description
The **Salesforce Admin** toolkit for AI agents.

### What you can do
- **Users** — List and search active users with profiles and roles
- **Objects** — List all objects, describe schemas with field details
- **Limits** — Monitor API calls, storage, and rate limits
- **Metadata** — Search Apex classes, triggers, flows via Tooling API
- **Apex** — Execute anonymous Apex code
- **Profiles** — List security profiles

### Who is this for?
- **Admins** — Manage 20+ orgs from one conversation
- **Consultants** — Explore client orgs instantly
- **Architects** — Understand data models in seconds


## Available Tools
- **sf_describe_object**: Returns every field with: API name, label, data type (string/number/date/reference/picklist/boolean), whether required or nullable, max length, reference target objects (for lookups), and picklist values (for picklist fields). Essential for understanding the data model before creating or querying records. Use when the user asks "what fields does Account have?" or needs to know valid picklist values.

Describe the full schema of a Salesforce object — all fields, data types, relationships, picklist values, and validation rules
- **sf_execute_apex**: Returns compilation success/failure, execution result, and debug logs. Use for admin tasks (data cleanup, batch operations), testing hypotheses, or running one-off scripts. CAUTION: this executes real code on the org — can modify data. Example: System.debug('Hello World');

Execute anonymous Apex code on the Salesforce org for admin tasks, data fixes, testing, or one-off operations
- **sf_org_limits**: Returns current usage vs. maximum for: daily API calls, data storage, file storage, SOQL queries, DML operations, email invocations, and more. Flags any limits below 10% remaining. Use for capacity monitoring, API governance, or when the user asks about org health and limit consumption.

Get API and storage usage limits for the Salesforce org — current consumption vs. maximum for API calls, storage, and more
- **sf_list_objects**: Returns all objects with their API name, label, whether they are queryable, createable, and custom. Includes standard objects (Account, Contact, Lead, Opportunity, Case), custom objects (ending in __c), and managed package objects. Essential for data model discovery: "what objects are available?", "do we have a custom invoices object?"

List all queryable and createable objects in the Salesforce org — standard, custom, and managed package objects
- **sf_list_profiles**: Returns profile name, description, user type, and license type. Profiles control what users can see and do in Salesforce — they define object permissions, field-level security, and page layouts. Use when the user asks about permissions, needs to audit access levels, or wants to understand the security model.

List Salesforce profiles (permission sets) with name, description, and user type for access control auditing
- **sf_list_users**: Returns user name, email, profile name, role name, user type (Standard/Chatter/etc.), and last login date. Use when the user asks about team members, needs user IDs for record assignment, wants to audit active accounts, or check last login dates for license management.

List active Salesforce users with their profile, role, email, user type, and last login date for team management
- **sf_search_metadata**: Supported objects: ApexClass, ApexTrigger, CustomField, ValidationRule, Flow, FlowDefinition, CustomObject, etc. Example: SELECT Id, Name, Body FROM ApexClass WHERE Name LIKE '%Account%'. Use when the user asks about code, automations, custom fields, or configuration metadata in the org.

Search Salesforce metadata via the Tooling API — find Apex classes, triggers, custom fields, validation rules, flows, and more
- **sf_search_users**: Returns user name, email, username, profile, role, and login info. Use to find a specific person in the org, look up who owns a record, or get user IDs for API operations.

Search Salesforce users by name, email, or username to find specific team members or administrators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Admin & Metadata** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Describe the Opportunity object schema"

**🤖 AI Agent:**
> 📋 **Opportunity** — 42 fields
| Field | Type | Required |
|---|---|---|
| Name | string | ✅ |
| Amount | currency | ❌ |
| StageName | picklist | ✅ |
| CloseDate | date | ✅ |
| AccountId | reference | ❌ |

---

**👤 You:**
> "Check our API limits"

**🤖 AI Agent:**
> 📊 **Org Limits**
| Limit | Remaining | Status |
|---|---|---|
| DailyApiRequests | 14,200/15,000 | ✅ OK |
| DailyBulkV2QueryJobs | 98/100 | ⚠️ LOW |
| DataStorageMB | 450/500 | ✅ OK |

---

**👤 You:**
> "List all Apex classes containing Account"

**🤖 AI Agent:**
> 🔍 Found 5 Apex classes:
1. AccountTriggerHandler
2. AccountService
3. AccountValidator
4. AccountBatchUpdate
5. AccountTestFactory


## ❓ FAQ

**Q: Can I execute Apex code?**
Yes — execute anonymous Apex. Returns compilation status, success/failure, and any exception details.

**Q: What metadata can I search?**
ApexClass, ApexTrigger, CustomField, ValidationRule, Flow, and more via the Tooling API SOQL.

**Q: How do org limits work?**
Shows remaining vs max for API calls, storage, daily queries, email limits, and more. Flags items below 10%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-admin-metadata](https://vinkius.com/mcp/salesforce-admin-metadata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce Admin & Metadata** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `salesforce-admin-metadata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce Admin & Metadata** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce-admin-metadata": {
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
